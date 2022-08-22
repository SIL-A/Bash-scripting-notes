```bash
#! /bin/bash

arr=('hi' 'hello' 'little' 'betty' 'bought' 'cake' 'newly' 'ordered' 'from' 'new' 'york')

echo ${arr[1]}

echo ${arr[@]}

echo ${#arr[@]}
```

+ The `@` symbol is used when we want to print the entire array.
+ The `#` symbol is used when we want to print the length of the array.