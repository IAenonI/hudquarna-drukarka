# Plan testów

## Testy modułowe

### VOC

- [ ] Czujnik odpowiada po uruchomieniu.
- [ ] Odczyt zmienia się po ekspozycji na zmianę jakości powietrza.
- [ ] Odczyt jest stabilny po nagrzaniu/ustabilizowaniu.

### Serwa klapek

- [ ] Klapka otwiera się i zamyka bez blokowania.
- [ ] Serwo nie buczy po dojściu do końca zakresu.
- [ ] Po restarcie układ wraca do bezpiecznej pozycji.

### Silnik 550 / airsuck

- [ ] Start przy niskim PWM.
- [ ] Start przy docelowym PWM.
- [ ] Brak resetów ESP32 przy starcie silnika.
- [ ] MOSFET się nie przegrzewa.
- [ ] Zasilacz 12 V nie zapada się pod obciążeniem.

### Integracja z drukarką

- [ ] ESP32 lub pośrednik pobiera status drukarki.
- [ ] Odczyt typu filamentu działa na realnym pliku z Orca Slicer.
- [ ] Brak danych nie zatrzymuje krytycznych funkcji bezpieczeństwa.

## Test końcowy

- [ ] Uruchomienie całego systemu.
- [ ] Test przez minimum 30 minut.
- [ ] Zdjęcia i logi z testu dodane do `docs/tests/results/`.
