# Podstawy DNS


1. **_record MX_** - rekord MX (Mail eXchange) - rekord wskazujący nazwę serwera obsługującego pocztę elektroniczną lub nazwę domeny (o ile strona internetowa i poczta elektroniczna utrzymywane są na tym samym serwerze).


2. **_record SOA_** - Rekord SOA - rekord SOA (Start Of Authority) - rekord zawierający główny serwer DNS oraz m.in. adres e-mail administratora domeny oraz numer seryjny domeny.Przykład wartości rekordu: ns1.nazwa.pl. biuro.nazwa.pl. 2008133200 28800 7200 604800 86400
```
MacBook-Pro-Szymon:~ szymondutka$ dig SOA google.com
google.com.		60	IN	SOA	ns3.google.com. dns-admin.google.com. 166177602 900 900 1800 60
```


3. **_record TXT_** - pole tekstowe
```
MacBook-Pro-Szymon:~ szymondutka$ dig google.com TXT
google.com.		1981	IN	TXT	"v=spf1 include:_spf.google.com ~all"
```


4. **_record NS_** - Adres serwera DNS
```
MacBook-Pro-Szymon:~ szymondutka$ dig e.pl NS
e.pl.			86400	IN	NS	dns2.lerkins.com.
e.pl.			86400	IN	NS	dns.lerkins.com.
```


5. **_TTL (Time to Live)_** - określa "czas życia" pakietu danych lub innych danych (np. rekordu DNS), stosowany w sieciach komputerowych.
```
MacBook-Pro-Szymon:~ szymondutka$ dig  +noall +answer @ns1.google.com www.google.com
www.google.com.		300	IN	A	216.58.214.228
```


6. **_+noall / +all_** - słuzy do pokazywania lub chowania pasa z informacjami np z dig google.com
```
PRZYKŁAD 1:
+ALL

MacBook-Pro-Szymon:~ szymondutka$ dig +all linguahouse.com

; <<>> DiG 9.8.3-P1 <<>> +all linguahouse.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 32078
;; flags: qr aa rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 2, ADDITIONAL: 2

;; QUESTION SECTION:
;linguahouse.com.		IN	A

;; ANSWER SECTION:
linguahouse.com.	300	IN	A	130.211.12.55

;; AUTHORITY SECTION:
linguahouse.com.	300	IN	NS	dns2.lerkins.com.
linguahouse.com.	300	IN	NS	dns.lerkins.com.

;; ADDITIONAL SECTION:
dns.lerkins.com.	1800	IN	A	195.46.43.194
dns2.lerkins.com.	1800	IN	A	195.46.43.195

;; Query time: 8 msec
;; SERVER: 195.46.43.195#53(195.46.43.195)
;; WHEN: Wed Aug 23 14:34:59 2017
;; MSG SIZE  rcvd: 126





PRZYKŁAD 2:
+NOALL

MacBook-Pro-Szymon:~ szymondutka$ dig  +noall  @ns1.google.com www.google.com
```


7. **_DHCP (Dynamic Host Configuration Protocol)_** - umozliwia przydzielanie adresów oraz innych elementów konfiguracjii.
```
DHCP option 50: 192.168.1.100 requested
Klient prosi serwer o przydzielenie danego adres IP
```


8. **_ARP_** - protokół sieciowy umożliwiający mapowanie logicznych adresów warstwy sieciowej 






