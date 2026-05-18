# Hudquarna / drukarka - centrum projektu

Repozytorium do prowadzenia prac nad obudową/układem sterowania dla drukarki **Artillery Sidewinder X4 Pro** z integracją przez **Fluidd**, układem wentylacji/wyciągu powietrza, czujnikiem VOC, serwami klapek oraz elektroniką na ESP32-S3.

## Jak pracujemy w repo

- **Postęp dzienny:** wpisy w `progress/YYYY-MM-DD.md`.
- **Roadmapa:** `roadmap/ROADMAP.md` oraz GitHub Issues/Project.
- **Zadania:** GitHub Issues, startowe zadania są opisane w `data/seed-issues.json` i utworzone jako issues.
- **Pliki:** wrzucamy do `docs/attachments/`, a zdjęcia/schematy/linki opisujemy w dzienniku dnia.
- **Decyzje techniczne:** zapisujemy w `decisions/ADR-000-template.md` i kolejnych ADR-ach.
- **Dokumentacja:** `docs/brief-from-pdf.md`, `docs/electronics/`, `docs/mechanics/`, `docs/integration/`, `docs/tests/`.

## Najbliższe priorytety

1. Sprawdzić i poprawić schemat połączeniowy.
2. Zaprojektować płytkę perforowaną z ESP32-S3 i resztą komponentów.
3. Zbadać komunikację z drukarką przez Fluidd/Klipper/Moonraker i ustalić, jak odczytać typ filamentu.
4. Uporządkować zasilanie: 12 V silnik 550, 20 V zasilacz, przetwornice 5 V/6 V, bezpieczniki, kondensator.
5. Przygotować testy: VOC, serwa klapek, PWM/MOSFET, bezpieczeństwo elektryczne.

## Struktura

```text
.
├── README.md
├── BACKLOG.md
├── CHANGELOG.md
├── data/seed-issues.json
├── decisions/
├── docs/
│   ├── brief-from-pdf.md
│   ├── electronics/
│   ├── integration/
│   ├── mechanics/
│   └── tests/
├── progress/
├── roadmap/
└── scripts/
```

## Codzienny workflow

1. Wybierz issue z boarda.
2. Dodaj lub edytuj pliki w `docs/`.
3. Dopisz wpis w `progress/YYYY-MM-DD.md`.
4. Zrób commit z krótkim opisem.
5. Przesuń issue na GitHub Project.
