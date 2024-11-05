```ch bash                                                                                                         simple.sh                                                                                                                
#!/bin/bash


# variable
name="Swapno Mondol"
#echo $name


# function that says hello and prient what we pass
hello() {
        echo "hello, $1"
}

#hello "world"


# take input, this will automatically echo name
#read name
#echo $name


# basic if else
echo "Enter a number:"
read number
if [ $number -gt 10 ]; then
    echo "The number is greater than 10."
else
    echo "The number is 10 or less."
fi


# loops
#!/bin/bash
for i in 1 2 3 4 5; do
    echo "Number: $i"
done


#while loop
#!/bin/bash
count=1
while [ $count -le 5 ]; do
    echo "Count: $count"

```
    count=$((count + 1))
done


