## While loop

```bash
#! /bin/bash

count=1

while (( $count < 10 ))
do
	echo $count
	count=$(( count + 1 ))
done
```

+ You know what a while loop is.

## Until loop

```bash
#! /bin/bash

count=1

until (( $count > 10 ))
do
	echo $count
	count=$(( count + 1 ))
done
```

+ The until loop is kind of like the opposite of while loop. A while loop continues until the given condition is proved false but in a until loop, the loop continues until the given condition is proved true,
+ The last iteration is the until loop is pretty tricky for me. So should dive into that later.

## For loop
``` bash
#! /bin/bash

for (( i=0;i<=10;i++))
do
	echo $i
done
```

+ You know what a for loop is and how it works.

### Common notes for all loops:
+ `continue` and `break` statements work in bash as they are intended in other programming languages.
