# Brief przeniesiony z PDF

Źródło: `docs/attachments/Hudquarna-drukarka.pdf`.

## Strona 1 - elementy do ewentualnego podłączenia w przyszłości

W PDF są linki do małych ekranów/modułów z AliExpress. Sens projektowy: zostawić miejsce i możliwość późniejszego podłączenia ekranu lub panelu informacyjnego.

**Do doprecyzowania:**
- czy ekran ma pokazywać status drukarki,
- czy ma pokazywać VOC/stan wentylacji,
- czy ma służyć do sterowania manualnego.

## Strona 3 - research integracji z drukarką

Drukarka: **Artillery Sidewinder X4 Pro**.  
Slicer: **Orca Slicer**.  
Interfejs kontroli: **Fluidd** dostępny z przeglądarki po IP w sieci lokalnej.

Cel researchu:
- komunikacja z drukarką,
- odczyt stanu drukarki,
- znalezienie sposobu, aby drukarka lub środowisko druku udostępniało informację o typie używanego filamentu.

## Strona 5 - założenia obudowy / wymiary

- szerokość około **59 cm**,
- głębokość około **59 cm**,
- górny moduł około **12 cm**,
- wysokość całkowita około **184 cm**,
- sekcja górna około **75 cm**,
- sekcja dolna około **74 cm**.

## Strony 6, 8, 9 - układ wentylacji, VOC i serw

Założenia z rysunków:
- wyciąg powietrza typu **airsuck 2000** na górze,
- klapki sterowane serwami,
- czujnik VOC w komorze,
- płytka prototypowa z ESP32 i komponentami w górnej części,
- zasilacze i przedłużacz uporządkowane w osobnej przestrzeni.

## Strona 7 - ekstraktor / silnik / sterowanie

W projekcie ma być użyta zmodyfikowana wersja ekstraktora **airsuck 2000**.  
Silnik: typ **550**, odzyskany ze starej wiertarki akumulatorowej.  
Sterowanie prędkością: **PWM przez MOSFET**.  
Zasilanie: zasilacz opisany jako **180 W / 12 V**, ale ze względu na charakterystykę tanich zasilaczy potrzebny może być duży kondensator, aby start silnika był stabilny.

## Strona 11 - schemat połączeniowy

W schemacie pojawiają się m.in.:
- ESP32-S3,
- czujnik VOC,
- czytnik kart,
- przekaźnik/moduł z pinami Common/Ground/Start,
- silnik 550,
- bezpieczniki,
- zasilacz 12 V,
- zasilacz 20 V,
- przetwornice 5 V i 6 V,
- serwa/klapki.

Kolory przewodów z opisu:
- zielony - sygnał,
- czerwony - napięcie,
- czarny - ziemia/GND.

## Strona 12 - najbliższy zakres prac

Zadania dla osoby projektującej:
- zaprojektować płytkę perforowaną,
- sprawdzić i poprawić schemat połączeniowy.

Zadania po stronie budowy:
- dokończenie budowy obudowy,
- transport do Wrocławia,
- ponowne składanie we Wrocławiu.
