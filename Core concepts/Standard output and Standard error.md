```bash
#! /bin/bash

ls -la 1>output.txt 2>error.txt
```

+ In this, we aim to print the output of the command `ls -la` to a text file. If the output is correct, then it will follow the path `1`, that is, it will send the output to the file named `output.txt`. If the output is incorrect or if there is an error (for example, if we use a wrong or incorrect command like `ls +la`), then the code will follow the pathe `2` that is, it will send the output to the file named `error.txt`.
+ If we remove `2` and only keep `1`, then the correct output will be saved to the text file and the incorrect output will be printed right then and there in the terminal.  And if we remove  `1` and only keep `2`, the the incorrect output will be saved to the text file and the correct output will be printed right then and there in the terminal.
+ 