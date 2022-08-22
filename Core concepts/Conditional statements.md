## If, Elif and Else
```bash
#! /bin/bash

count=100

if (( $count > 110 ))
then
	echo "Condition is true"
elif (( $count == 100 ))
then
	echo "The value of count is exactly 100"
else
	echo "Condition is false"
fi
```

+ The conditional statements in bash have the following syntax:
	+ ```if (( condition ))
	    then
		    <DO WHAT YOU WNAT TO DO>
		else
			<DO WHAT YOU WNAT TO DO>
		fi```

+ The `fi` means finish (or atleast thats what I like to think).
+ In bash, like normal programming languages, `AND` is denoted by `&&` , `OR` by `||` . But out cant use the words  `AND` and `OR` themselves. You have to use their given symbols or the specific characters assigned to them.

+ In bash, different brackets mean different things for conditional statments
	+ `[]` is synonymous with the `test` command. Basically it can work with strings and not do arithmetic operations like `>`, `<`, `>=`, etc.
	+ `[[]]` is just the upgraded version of `[]` and it does basically the same thing.
	+ `(())` is used to work with numbers and arithmetic operations.
	+ `()` is used to run a command. if the command runs successfully, the if statement is executed and if not, the control falls to the next elif or else statements.


## Case
```bash
#! /bin/bash

arr=('hi' 'hello' 'little' 'betty' 'bought' 'cake' 'newly' 'ordered' 'from' 'new' 'york')
case $1 in
	${arr[0]})
		echo "SELECTED 'hi'";;
	${arr[1]})
		echo "SELECTED 'hello'";;
	${arr[2]})
		echo "SELECTED 'little'";;
	${arr[3]})
		echo "SELECTED 'betty'";;
	${arr[4]})
		echo "SELECTED 'bought'";;
	${arr[5]})
		echo "SELECTED 'cake'";;
	*)
		echo "SELECTED SOMETHING ELSE";;
esac
```

+ I think it is self explanatory if you know hat case does. 
+ The last `*)` is for everything else.