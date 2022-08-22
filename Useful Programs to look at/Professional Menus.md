```bash
#! /bin/bash

cars=('BMW' 'TESLA' 'SUZUKI' 'TOYOTA' 'MAHINDRA')

for (( i=0;i<5;i++ ))
do
	echo "Press $(( $i+1 )) to select ${cars[$i]}"
done


select car in BMW TESLA SUZUKI TOYOTA MAHINDRA
do
	case $car in
		BMW)
			echo "You have selected $car";;
		TESLA)
			echo "You have selected $car";;
		SUZUKI)
			echo "You have selected $car";;
		TOYOTA)
			echo "You have selected $car";;
		MAHINDRA)
			echo "You have selected $car";;
		*)
			echo "Please select correctly";;
	esac
done
```

+ The `select` statement is the most important thing here which does all the magic.