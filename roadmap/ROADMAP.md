# Roadmapa projektu

## Faza 0 - uporządkowanie projektu

**Cel:** jedno miejsce do śledzenia plików, progresu, decyzji i zadań.

- [x] Przenieść brief z PDF do repo.
- [x] Dodać miejsce na dziennik prac.
- [x] Dodać startowy backlog.
- [x] Utworzyć startowe GitHub Issues.
- [ ] Utworzyć GitHub Project/board i podpiąć issue.

## Faza 1 - research komunikacji z drukarką

**Cel:** ustalić, jak pobierać informacje z Artillery Sidewinder X4 Pro / Fluidd / Orca Slicer.

- [ ] Sprawdzić API / endpointy Fluidd/Klipper/Moonraker.
- [ ] Ustalić źródło informacji o typie filamentu.
- [ ] Zapisać minimalny protokół wymiany danych ESP32 <-> system drukarki.
- [ ] Udokumentować ograniczenia i ryzyka.

## Faza 2 - elektronika i bezpieczeństwo

**Cel:** poprawny, bezpieczny schemat zasilania i sterowania.

- [ ] Zweryfikować schemat połączeniowy.
- [ ] Zaprojektować płytkę perforowaną.
- [ ] Dobrać bezpieczniki i przekroje przewodów.
- [ ] Zweryfikować MOSFET/PWM dla silnika 550.
- [ ] Zweryfikować przetwornice 5 V/6 V i wspólną masę.
- [ ] Zaplanować test startu silnika z kondensatorem.

## Faza 3 - mechanika / obudowa / przepływ powietrza

**Cel:** domknąć układ obudowy, klapek, VOC i wyciągu.

- [ ] Dokończyć dokumentację obudowy.
- [ ] Sprawdzić pozycję czujnika VOC.
- [ ] Przetestować klapki sterowane serwami.
- [ ] Sprawdzić montaż airsuck 2000.

## Faza 4 - testy integracyjne

**Cel:** test całego układu przed oddaniem projektu.

- [ ] Test elektroniki bez silnika.
- [ ] Test silnika i MOSFET pod obciążeniem.
- [ ] Test VOC i automatyki klapek.
- [ ] Test działania przy drukowaniu.
- [ ] Dokumentacja końcowa.
