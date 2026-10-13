# ćw. 1
Wypróbowane komendy:
- starwars - odtwarza film "Star Wars" jako animację tekstową ASCII
- 2048 - uruchamia grę 2048 
- pong - uruchamia grę w ping-ponga

Za wszystkie te rzeczy możę odpowiadać Web albo aplikacja.
Zmieniło się to, że nie trzeba się uczyć komend na pamięć, nie trzeba
znać interfejsów tesktowych i pojawiły się interfejsy graficzne.

# ćw. 2
| żądanie | metoda | ścieżka | kod | 3 nagłówki + co znaczą |
| --- | --- | --- | --- | --- |
| info.cern.ch | GET | / | 200 OK | Server: Apache - program, który obsługuje żądania |
| github.com | HEAD | / | 301 Moved Permanently | Location: https://github.com/ - adres, pod którym zasób jest dostępny |
| nie-ma-takiej | HEAD | /nie-ma-takiej | 404 Not Found | Connection: close - informacja, że serwer zamyka połączenie siciowe po wysłaniu odpowiedzi

github.com odpowiada inaczej niż info.cern.ch, ponieważ GitHub wymusza szyfrowanie danych, więc kiedy chcemy przejść na niego bez szyfrowania (http zamiast https), odrzuca połączenie i wskazuje adres z szyfrowaniem.

# ćw. 3
| pomiar | info.cern.ch | spacejam.com/1996 | onet.pl |
| --- | --- | --- | --- |
| liczba żądań | 1 | 18 | 332 |
| przesłane dane | 0,88 kB | 234,9 kB | 5,51 MB |
| czas ładowania | 292 ms | 1,83 s | 3,64 s |
| elementy DOM | 16 | 119 | 1547 |
| najcięższy plik (typ) | document | js | jpg |

Starsze strony internetowe były lżejsze i składały się z mniejszej liczby zasobów. W przypadku spacejam, skrypt js stanowi ponad połowę całkowitej wagi strony. Duży przeskok pod względem liczby żądań i ilości przesłanych danych widać na przykładzie onetu - portal ładuje duże ilości kodu JavaScript, obrazków, reklam, itp.

Strony internetowe wyewoluowały z prostych plików tekstowych w złożone aplikacje.