## Getting input through arguments using `$`
```bash
#! /bin/bash

first=$1
second=$2
third=$3

echo $first
echo $second
echo $third
```

+ The numbers after the `$` symbol indicate the order of the input /arguments provided.
+ If `$0` is used, then the script name used to run it (for example `./helloworld.sh`) is also taken as input since it is the zeroth argument.
 

## Getting Standard input using `stdin`
```bash
#! /bin/bash

while read line
do
	echo $line
done < ${1:-/dev/stdin}
```

+ The `stdin` is used to read lines from a file just like in python. 
+ The `/dev/stdin` is actually an inbuilt script used just for this purpose. 
+ In this program, we read the individual lines of the file and the `echo` them out. 

## Getting input from user in interactive shells
```bash
#! /bin/bash

echo 'Enter 1st string'
read str1
echo 'Enter 2nd string'
read str2

if [ $str1 == $str2 ]
then
	echo "String 1 is equal to String 2"
else
	echo "String 1 is not equal to String 2"
fi
```

+ As you can see, we have used the `read` command to get the input from the user interactively.