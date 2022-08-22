```bash
#! /bin/bash

echo "Press any key to continue"

while [ true ]
do
	read -t 3
if [ $? = 0 ]
then
	echo "You have terminated the script"
	exit;
else
	echo "Press any key to exit"
fi
done
```

+ In this, the `read -t 3` read the input every three seconds. Use the command `read --help` to read the utilities of the `read` command
+ If you want the script to end when the user presses any key, you need to add the argument `-n 1` to the `read` command. 