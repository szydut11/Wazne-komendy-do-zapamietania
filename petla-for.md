# wszystko o pętli **_for_**

1. Pętla for jak nazwa sama wskazuje słuzy do powtazania jakiejs okreslonej czynnosci lub zadanego zadania 
```
#!/bin/bash

for x in {1..2}; do
  mkdir ${x}
  echo "tworzenie katalogu 1"
  echo "tworzenie katalogu 2"
  cd ${x}
  echo "wchodze do katalogu 1"
  echo "wychodze z katalogu 2"
  for y in {1..2}; do
      touch ${y}.txt
  echo "tworze plik 1"
  echo "tworze plik 2"
  done
  cd ..
  echo "wychodze z katalogu 1"
  echo "wychodze z katalogu 2"
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