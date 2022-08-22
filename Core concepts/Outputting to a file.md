```bash
#! /bin/bash

echo "Outputting to a file. This will be the first line" > output.txt
echo "Outputting to a file. This will be the second line" >> output.txt
```

+ In this, the `>` is used to clear the existing data in the file `output.txt` (if the file does not exist, a new one is created) and add the new one which we want. 
+ The `>>` symbol is used to append our data to the existing data present already in the file. 
