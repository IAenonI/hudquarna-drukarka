# Checklist - sprawdzenie schematu połączeniowego

## Zasilanie

- [ ] Czy zasilacz 12 V zasila tylko obwody, które faktycznie są na 12 V?
- [ ] Czy silnik 550 ma osobny bezpiecznik?
- [ ] Czy przetwornice 5 V/6 V mają odpowiedni zapas prądu?
- [ ] Czy wszystkie moduły mają wspólną masę tam, gdzie wymaga tego sygnał sterujący?
- [ ] Czy przewody mają sensowny przekrój dla prądu silnika?
- [ ] Czy kondensator przy zasilaniu silnika jest poprawnie dobrany i spolaryzowany?
- [ ] Czy 230 V jest fizycznie odseparowane i zabezpieczone?

## ESP32-S3 i logika

- [ ] Czy piny użyte do sterowania MOSFET/serwami nie konfliktują z bootstrappingiem ESP32?
- [ ] Czy poziomy logiczne są 3.3 V zgodne z ESP32?
- [ ] Czy wejścia czujników mają poprawne zasilanie i masę?
- [ ] Czy czytnik kart ma właściwy interfejs i poziomy napięć?

## MOSFET / silnik 550

- [ ] Czy MOSFET jest logic-level i otwiera się przy 3.3 V?
- [ ] Czy jest dioda/zabezpieczenie przeciw przepięciom indukcyjnym?
- [ ] Czy PWM nie będzie powodował resetów ESP32?
- [ ] Czy radiator lub margines prądowy MOSFET jest wystarczający?

## Serwa klapek

- [ ] Czy serwa mają osobne zasilanie 5 V/6 V z odpowiednim prądem?
- [ ] Czy sygnał z ESP32 ma wspólną masę z zasilaniem serw?
- [ ] Czy zakres ruchu klapek nie blokuje mechanicznie serw?

## Test bezpieczeństwa przed pierwszym uruchomieniem

- [ ] Test ciągłości GND.
- [ ] Test braku zwarcia między V+ i GND.
- [ ] Pierwsze uruchomienie z ograniczeniem prądu lub bez obciążenia.
- [ ] Test każdego modułu osobno.
- [ ] Dopiero na końcu test całego układu.
