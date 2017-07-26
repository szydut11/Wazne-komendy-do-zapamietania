# bash komendy

1. **_cd_** - za pomoca tej komendy wchodzimy do jakiegos katalogu
```
pc44:nowy szymondutka$ cd wianki
pc44:wianki szymondutka$ ls
20170624_222309.jpg	20170624_225741.jpg	20170624_225837.jpg	20170624_225937.jpg	20170624_230322.jpg
20170624_222313.jpg	20170624_225749.jpg	20170624_225859.jpg	20170624_225953.mp4	20170624_230324.jpg
20170624_223415.jpg	20170624_225806.jpg	20170624_225900.jpg	20170624_230003.jpg	20170624_230347.jpg
20170624_225615.mp4	20170624_225808.jpg	20170624_225901(0).jpg	20170624_230005.jpg	20170624_230403.jpg
20170624_225729.mp4	20170624_225809.jpg	20170624_225901.jpg	20170624_230020.jpg	20170624_230453.jpg
20170624_225731.jpg	20170624_225812.jpg	20170624_225903.jpg	20170624_230024.jpg	20170715_131847.jpg
20170624_225733.jpg	20170624_225822.jpg	20170624_225907.jpg	20170624_230034.jpg	20170715_132205.jpg
20170624_225734.jpg	20170624_225827.jpg	20170624_225923.jpg	20170624_230035.jpg
20170624_225735.jpg	20170624_225829.jpg	20170624_225933.jpg	20170624_230200.mp4
20170624_225737.jpg	20170624_225835.jpg	20170624_225935.jpg	20170624_230243.jpg
pc44:wianki szymondutka$
```
2. **_ls_** - pokazuje nam liste wszystkich katalogow i plikow jakie posiadamy aktualnie
```
pc44:wianki szymondutka$ ls
20170624_222309.jpg	20170624_225741.jpg	20170624_225837.jpg	20170624_225937.jpg	20170624_230322.jpg
20170624_222313.jpg	20170624_225749.jpg	20170624_225859.jpg	20170624_225953.mp4	20170624_230324.jpg
20170624_223415.jpg	20170624_225806.jpg	20170624_225900.jpg	20170624_230003.jpg	20170624_230347.jpg
20170624_225615.mp4	20170624_225808.jpg	20170624_225901(0).jpg	20170624_230005.jpg	20170624_230403.jpg
20170624_225729.mp4	20170624_225809.jpg	20170624_225901.jpg	20170624_230020.jpg	20170624_230453.jpg
20170624_225731.jpg	20170624_225812.jpg	20170624_225903.jpg	20170624_230024.jpg	20170715_131847.jpg
20170624_225733.jpg	20170624_225822.jpg	20170624_225907.jpg	20170624_230034.jpg	20170715_132205.jpg
20170624_225734.jpg	20170624_225827.jpg	20170624_225923.jpg	20170624_230035.jpg
20170624_225735.jpg	20170624_225829.jpg	20170624_225933.jpg	20170624_230200.mp4
20170624_225737.jpg	20170624_225835.jpg	20170624_225935.jpg	20170624_230243.jpg
```
3. **_ls ?_** - wyswielta całą zawartosc katalogu ktory ma jedna litere, cyfre itp.
```
pc44:nowy szymondutka$ ls
1		2		drukarka	klawiatura	komputer	monitor		mysz
pc44:nowy szymondutka$ ls ?
1	2
```
4. **_rm ?_** - kasuje wszystkie pliki ktore maja wlasnie jedna litere, cyfre itp
```
pc44:nowy szymondutka$ ls
1		2		drukarka	klawiatura	komputer	monitor		mysz
pc44:nowy szymondutka$ rm ?
pc44:nowy szymondutka$ l
-bash: l: command not found
pc44:nowy szymondutka$ ls
drukarka	klawiatura	komputer	monitor		mysz
```
5. **_ls (plik)_** - wyszukuje danego pliku o jakiejs nazwie
```
pc44:nowy szymondutka$ ls
drukarka	klawiatura	komputer	monitor		mysz
pc44:nowy szymondutka$ ls klawiatura
klawiatura
```
6. **_ls ????d.txt_** - wyszukuje i pokazuje wszystkie pliki o nazwie konczacej sie na d i ktore maja piec liter, cyfr
```
pc44:nowy szymondutka$ ls ???d.txt
czad.txt	dddd.txt	word.txt
``` 
7. **_ls world.???_** -wyszukuja i wyswielaja wszystkie pliki ktore maja rozszerzenie na trzy litery np txt, jpg,mov,doc itp
```
pc44:nowy szymondutka$ ls world.???
world.doc	world.jpg	world.txt
``` 
8. **_clear_** - czysci nasza tablice
```
pc44:nowy szymondutka$ clear
pc44:nowy szymondutka$





```
9. **_ls ???.txt_** - wyswietla wszystkie pliki ktore maja trzy litery i rozszerzenie .txt
```
pc44:nowy szymondutka$ ls ???.txt
cos.txt
kon.txt
ccc.txt
cdn.txt
```
10. **_ls *.txt_** - pokazuje wszystkei pliki ktore maja koncowke txt w danym katalogu
```
pc44:nowy szymondutka$ ls *.txt
cos.txt		dddd.txt	mysz.txt	word.txt
czad.txt	miód.txt	nowy.txt	world.txt
```
11. **_ls w*.txt kilka pilkow_** - wyszukuje i wyswietla wszystkie pliki o poczatku na w i rozszerzeniu .txt
```
pc44:nowy szymondutka$ ls w*.txt
wiele.txt	witam.txt	word.txt	world.txt	wracam.txt
```
12. **_ls w*??.txt_** - szuka i wyswietla pliki o pocztaku w na trzy litery lub liczby i roszerzeniu .txt
```
pc44:nowy szymondutka$ ls w*??.txt
wiele.txt	witam.txt	word.txt	world.txt	wracam.txt
```
13. **_ls *w??.txt_** - ta komenda wyswietla nam w ty przypadku obraz/y ktory/e ma/ja poczatek i koniec nieznany natomiast w srodku jest litera w i rozszerzenie .txt 
```
pc44:nowy szymondutka$ ls *o??.txt
miód.txt	nowy.txt	word.txt
```
14. **_cp *.txt ../copies_** - tworzy kopie plikow txt 
```
```
15. **_rm ../copies_** -  usuwa wszystkie pliki z kopii txt
```
```
16. **_alpha alnum digit lower upper_** - ustawia pliki w kolejnosci alfabetycznej, alfanumerycznej, wedlug liczby , malejaco ,rosnaco
```
```
17. **_ls [[:digit:]]nowy_** - ukalda pliki wedlug kolejnosci liczbowej
```
pc44:nowy szymondutka$ ls [[:digit:]]nowy
ls: [[:digit:]]nowy: No such file or directory
pc44:nowy szymondutka$ ls
cos.txt		drukarka	komputer	mysz		wiele.txt	word		world.jpg
czad.txt	flame.txt	miód.txt	mysz.txt	witam		word.txt	world.txt
dddd.txt	klawiatura	monitor		nowy.txt	witam.txt	world.doc	wracam.txt
```
18. **_ls [[:upper:]]*_** - uklada pliki rosnaco
```
pc44:nowy szymondutka$ ls [[:upper:]]nowy
ls: [[:upper:]]nowy: No such file or directory
pc44:nowy szymondutka$ ls
cos.txt		drukarka	komputer	mysz		wiele.txt	word		world.jpg
czad.txt	flame.txt	miód.txt	mysz.txt	witam		word.txt	world.txt
dddd.txt	klawiatura	monitor		nowy.txt	witam.txt	world.doc	wracam.txt
```
19. **_ls [[:alpha:]]*_** - ukalda pliki w kolejnosci alfabetycznej
```
pc44:nowy szymondutka$ ls [[:alpha:]]nowy
ls: [[:alpha:]]nowy: No such file or directory
pc44:nowy szymondutka$ ls
cos.txt		drukarka	komputer	mysz		wiele.txt	word		world.jpg
czad.txt	flame.txt	miód.txt	mysz.txt	witam		word.txt	world.txt
dddd.txt	klawiatura	monitor		nowy.txt	witam.txt	world.doc	wracam.txt
```

20. **_ls [1f]*_** - wyswietla pliki ktore zawiraja w nazwie jedno f 
```
pc44:nowy szymondutka$ ls [1f]*
flame.txt
```
21. **_ls [2f]_** - wyswietla pliki ktore maja 2f w nazwie
```
pc44:nowy szymondutka$ ls [2f]*
flame-fire.txt
```
22. **_ls [wp][io][r123]*_** - 
``` 
pc44:nowy szymondutka$ ls [wp][io][r123]*
word		word.txt	world.doc	world.jpg	world.txt
```


