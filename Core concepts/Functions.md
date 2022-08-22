```bash
#! /bin/bash

function hello()
{
	echo 'Hello World'
}

hello
```
+ This is an example of a simple function. But it can get complex very quick. 

For example

```bash
#! /bin/bash

function hello()
{
	for (( i=0;i<(( $1+1 ));i++ ))
	do
		echo $i
	done
}

inp=$1
hello $inp
```

+ In this, the `$1` in the function solely represents the 1st argument to the function and not the entire program. That's why we are able to use `$1` with different uses inside and outside the function.



+ When the function is called, it's local variables become global, meaning, their values can be accessed from outside the function. This is why there is not `return` in bash (to my knowlwdge), because it is not needed.