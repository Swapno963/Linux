```ch bash
#!/bin/bash

echo "Enter the directory you want to back up:"
read dir
echo "Enter the destination path for the backup:"
read dest

# Check if the source directory exists
if [ ! -d "$dir" ]; then
    echo "Error: The directory $dir does not exist."
    exit 1
fi

# Check if the destination directory exists, and create it if not
if [ ! -d "$dest" ]; then
    echo "Destination directory does not exist. Creating it..."
    mkdir -p "$dest"
fi

backup_name="$(basename "$dir")_backup_$(date +%Y%m%d).tar.gz"
tar -czvf "$dest/$backup_name" "$dir"
echo "Backup of $dir completed at $dest/$backup_name"
```


### for To extract the entire archive:
-x: Extracts the contents.
-z: Unzips the .gz compressed file.
-v: Shows progress in the terminal (optional).
-f: Specifies the filename.

```ch bash
tar -xzvf backup_name.tar.gz
```
