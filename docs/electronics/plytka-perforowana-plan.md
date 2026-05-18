# Plan płytki perforowanej

## Cel

Zaplanować ułożenie ESP32-S3, złącz, przewodów sygnałowych i zasilających tak, aby dało się łatwo serwisować układ i ograniczyć ryzyko zwarć.

## Bloki na płytce

1. **ESP32-S3** - centrum sterowania.
2. **Wejścia czujników** - VOC, ewentualnie czytnik kart.
3. **Wyjścia sterujące** - MOSFET/PWM, serwa klapek, przekaźnik/start.
4. **Złącza zasilania** - 5 V, 6 V, 12 V, GND.
5. **Złącza serwisowe** - piny do pomiaru napięć i debugowania.

## Zasady layoutu

- Linie prądowe silnika prowadzić poza cienkimi ścieżkami/perforacją, najlepiej osobnymi przewodami.
- Sygnały niskonapięciowe prowadzić osobno od przewodów silnika.
- Opisać każde złącze na płytce i w dokumentacji.
- Dodać miejsce na odłączenie modułów bez lutowania całego układu.
- Zostawić zapas na przyszły ekran/panel.

## TODO

- [ ] Narysować top-view płytki.
- [ ] Rozpisać złącza: nazwa, napięcie, pinout.
- [ ] Zweryfikować prądy każdego bloku.
- [ ] Dodać zdjęcie gotowej płytki po montażu.
