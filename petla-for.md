# wszystko o pętli **_for_**

1. Pętla for jak nazwa sama wskazuje słuzy do powtazania jakiejs okreslonej czynnosci lub zadanego zadania 
```
#!/bin/bash

for x in {1..100}; do
  mkdir ${x}
  echo "tworzenie katalogu ${x}"

  cd ${x}
  echo "wchodze do katalogu ${x}"

  for y in {1..100}; do
      touch ${y}.txt
  echo "tworze plik ${y}"
  done

  cd ..
  echo "wychodze z katalogu ${x}"
done
```


2. Są trzy przykłady petli for

*podobna do języka C 
```
#!/bin/sh

for (( i=1; $i <= 10; i++ )) ; do
       echo " Iteracja nr: $i"
done
```
```
#!/bin/sh

for i in `seq 1 10`
do
       echo "Iteracja nr: $i"
done
```

*bashowa
```
for x in jeden dwa trzy ; do
    echo "To jest $x"
done
```


3. jest bardzo przydatna poniewaz nie musimy robic kilka razy tych samych rzeczy tylko wystarczy ze zrobimy to raz za pomoca petli
