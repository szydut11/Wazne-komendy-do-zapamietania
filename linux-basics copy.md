# virtualbox i iterm
komendy których się nauczyłem dzięki tym lekcjom


1. su  -  jest to komenda dzięki której mozemy zmienić uzytkownika na serwerze 
```
szydut22@user2:~$ su user1
Password:
user1@user2:/home/szydut22$
```


2. chown - dzięki niemu mozemy zmienic własciciela pliku
```
chown szydut22 nowy
```


3. chmod - dzięki niemu zmieniamy uprawnienia pliku
```
szydut22@user2:~$ ls -l
total 16
-rwxr----- 1 szydut22 szydut22   1 Jul  5 12:14 etc.save
--w------T 1 szydut22 szydut22  42 Jul  5 11:24 nowy
-rw-rw-r-- 1 szydut22 szydut22  20 Jul  5 16:02 plik1
-rw-rw-r-- 1 szydut22 szydut22 153 Jul  5 12:13 polecenia wazne
szydut22@user2:~$ chmod 1000 plik1
szydut22@user2:~$ ls -l plik1
---------T 1 szydut22 szydut22 20 Jul  5 16:02 plik1
```



4. sh - jest to powłoka w linuxie




5. echo"$SHELL " - słuzy nam do sprawdzenia na jakiej powłoce jesteśmy
```
szydut22@user2:~$ echo $SHELL
/bin/bash
```



6. cat np plik1 lub plik2 - wyświetli nam zawartość pliku 
```
szydut22@user2:~$ cat plik1
nowy ciekawy folder
```


7. kolejnym przykładem na cat jest cat /home/(nazwa użytkownika)/jakiś stworzony przez nas plik
```
szydut22@user2:~$ cat /home/szydut22/plik1
nowy ciekawy folder

```  


8. pwd-pokazuje w hakim pliku jestem
```
szydut22@user2:~$ pwd
/home/szydut22
```


9. touch- pozwala na zmianę daty ostatnich zmian które zapisaliśmy w pliku nano czyli np w komendzie nano etc /linux/user/(stworzony przez nas plik)
```
szydut22@user2:~$ touch plik1
szydut22@user2:~$ ls -l
total 24
-rw-rw-r-- 1 szydut22 szydut22   7 Jul  5 16:13 etc
-rwxr----- 1 szydut22 szydut22   1 Jul  5 12:14 etc.save
--w------T 1 szydut22 szydut22  42 Jul  5 11:24 nowy
---------T 1 szydut22 szydut22  20 Jul  5 16:29 plik1
-rw-rw-r-- 1 szydut22 szydut22   1 Jul  5 16:14 plik2
-rw-rw-r-- 1 szydut22 szydut22 153 Jul  5 12:13 polecenia wazne
```


10. head i tail - służą one do podejrzenia pliku
```
szydut22@user2:~$ head nowy.txt
przykladowy tekst w przykładowym miejscu

szydut22@user2:~$ tail.txt
tail.txt: command not found
```


11. Adduser - słuzy do dodania nowego uzytkownika
```
zydut22@ubuntu:~$ sudo adduser user2
Adding user `user2' ...
Adding new group `user2' (1001) ...
Adding new user `user2' (1001) with group `user2' ...
Creating home directory `/home/user2' ...
Copying files from `/etc/skel' ...
Enter new UNIX password:
Retype new UNIX password:
passwd: password updated successfully
Changing the user information for user2
Enter the new value, or press ENTER for the default
	Full Name []: user1
	Room Number []: 111
	Work Phone []:
	Home Phone []:
	Other []:
Is the information correct? [Y/n] yes
```


12. passwd - pozwala na zmianę hasła użytkownika
```
szydut22@user2:~$ passwd
Changing password for szydut22.
(current) UNIX password:
Enter new UNIX password:
Retype new UNIX password:
passwd: password updated successfully
```


13. logout i exit - umozliwiaj nam wulogowanie z serweru np. linux
```
szydut22@user2:~$ exit
logout
Connection to 192.168.56.102 closed.
MacBook-Pro-Szymon:~ szymondutka$
```

14. Mamy takze róznego rodzaju katalogi takie jak np:
* /bin - pliki binarne
* /dev - są w nim przechowywane pliki przy starcie sytemu
* /etc - sa to wszystkie pliki konfiguracyjne typu hasło, nazwa uzytkownika
* /home - sa tu przechowywane wszystkie pliki uzytkownika


