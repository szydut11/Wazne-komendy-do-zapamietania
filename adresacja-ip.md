# Wszystko o adresacji ip


1. **_Na podstawie adresu ip odbywa sie dostarczanie danych np z jaednego komputera o danym ip do drugiego komputera tez o jakims numerze ip_**

2. **_adres ip jest to logiczny adres interfesu sieciowego urzadzenia pracujacego w danej sieci. Takimi urzadzeniami moga byc np._**
* komputer
* router
* lub jakis punkt dostepowy

   **_wszystko to co zostalo przeze mnie wymienione sa to inaczej hosty_**

3. **_Interfejsem sieciowym np w komputerze jest karta sieciowa_**


4. **_serwer moze wytwarzac wiecej niz jeden nr. ip . Gdy np. ma dwie karty sieciowe inaczej (interfejsy) moze np za pomoca jednego z nich laczyc sie z kompterami w sieci LAN czyli sieci lokalnej a drugim do łaczenia sie z siecia rozlegla lub bezposrednio z internetem jest to podobna zasada dzialania jak u naszych domowych routerów._**


5. **_Adres ip składa sie z czterech oktetów  czego jeden oktet przyjmuje wartosc od 0 do 255 i takie adresy sa tylko poprawne._**


6. **_193.184.102.165_**  z czego
* pierwsza czesc czyli  193.184.102 sa adresem sieci w jakim pracuje komputer 
* drugie czyli ostatni oktet taki jak 165 to adres hosta 

7. **_maska podsieci_** - maska musi zaczynac sie od ciagu jedynek natomiast pomiedzy tymi jedynkami nie moze znalezc sie 0 poniewaz wtedy nie mozemy sie dowiedziec ktora czesc nalezy do maski a ktora do hosta 

8. **_adresowania klasowe i bezklasowe_**

* adresowanie klasowe wymaga uzycia podzialu na zdefiniowane klasy takie jak A B C D E okreslaa one liczbe mozliwych do zaadresowania sieci i ich hostow 

  * za pomoca klasy A mozemy tworzyc rozległe sieci gdzie mozna zaadresowac ok 16 000 000 hostow .Posiada ona domyslnie maske 255.0.0.0 czyli pierwczy zawiera adres sieci a reszta adres hostów 

  * klasa B zostala stworzona do adresowania srednich i duzych ilosci hostow czyli do ok 60 000 

  * Klasa C blok klasy C został domyslnie stworzony do obslugiwania malych rodzajow sieci.

  * Adresy klasy D to adresy tzw. grypowe

  * Natomiats adresy klasy E to tzw. adresy eksperymentalne ta klasa czyli E nie jest  do adresowania hostow agencja IANA wykorzystuje je tylko dla swojego uzytku.

* aderswoanie bezklasowe mozemy nazwac bardziej elastycznym czyli ze mozemy sami ustalac liczbe klas lub hostów do zaadresowania za pomoca wlasnie masek podsieci dxzieki niom beddziemy mogli podzielic adresy na podsieci

8. **_Dobrze jest tez wiedziec jak mozna obliczyc_**
* adres sieci.
* adres rozgloszeniowy.
* oraz liczbe hostow z adresem pierwszego i ostatniego.

9. **_Adresy publiczne stosowane w sieciach rozległych czyli takie gdzie kazdy komputer na calym globie ma przyznany inny adres i sa to adresy unikatowe takie jak adresy prywatne czyli np w sieci lokalnej LAN kazdy komputer ma przypisany inny adres natomiast w potem w innej sieci LAN moze on sie powtorzyc_**

10. **_adres intenetowy otrzymujemy o naszego providera czyli dostawcy internetu natomiast potem ten jeden adres jest roprowadzany do wszystkich komputerow za pomoca usługi NAT ( Network Adress Translation) słuzy ona do tego iz tłumaczy adresy prywatne na publiczne lub odwrotnie. Natomiast w sieci inni widza nas pod tym adresem ktory przypisany nam zostal przez providera mozna to sprawdzic na stronie_**

###      http://www.moje-ip.eu/

11. **_adresacja bezklasowa c.d.n maska_**
```
maska : 255.255.255.0 /24
11111111.11111111.11111111.00000000 

pierwsze trzy oktety czyli same jedynki to siec natomiast 0 to hosty. Jezeli chcemy podzielic taki adres na dwie logiczne podsiecito musimy z czesci hosta oddac 1 bit do czesci sieciowej wtedy nasza maska bedzie wygladac tak :

Maska 255.255.255.128 /25 
11111111.11111111.11111111.10000000 

Kolejna maska to 255.255.255.198 /26
11111111.11111111.11111111.11000000

tak wiec w pierwszym wypadku powstanie 1 siec w drugim dwie podsieci a w trzecim juz 4 dlaczego 4 a nie 3 w ostatnim przykaldzie a dlatego ze potega liczby 2 nigdy nie da nam nieparzystej liczby 
```
# ogólny wzór na ten przyklad to 2^n gdzie n= liczbie oddanych bitow z czesci hosta czy li w ostatnim przykladzie mamy dwie 1 czyli bedzie 2^2 =4 (podsieci)

12. **_VLSM uzywamy gdzy zmieniamy dlugosc maski tak aby uwzglednic zapotrzebowanie na liczbe hostow w podsieci_**
```
Maska 255.255.255.0 /24

11111111.11111111.11111111.00000000 daje 1 siec a 254 hosty 

Maska 255.255.255.128 /25 

11111111.11111111.11111111.10000000 daje nam 2 podsieci po 126 hostow 

natomiast gdzy dodamy jeszcze jedna jedynke w drugim przypadku bedziemy mogli podzielic tego hosta na dwa mniejsze

Maska 255.255.255.192 /26

11111111.11111111.11111111.11000000 i wtedy da nam to 4 podsieci po 62 hosty

podsiec 1 ma 126 hostow natomiast drugq podsiec podzielilismy na dwie wiec druga i trzecia beda po 62 hosty i po tym wszystkim mozemy zabrac sie za obliczenie adresow sieci, rozgloszeniowych, pierwszego i ostatniego hosta  
```

13. **_Adresy prywatne_** Adresy prywatne nie są routowane w Internecie, co oznacza, że mogą się powtarzać w różnych sieciach.
 * A	10.0.0.0 - 10.255.255.255
 * B	172.16.0.0 - 172.31.255.255
 * C	192.168.0.0 - 192.168.255.255
