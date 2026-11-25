# QUIZ MOW – Quizy i testy wiedzy

Uruchom: https://jarekdymek.github.io/Konkursy/

Wersja 1.0: 80 pytań konkursu „W blasku świętych – w drodze do Betlejem”, po 20 w czterech działach. Pytania ćwiczeniowe, nie oficjalne pytania organizatora.

## Obsługa
- Strzałki góra/dół: wybór; prawo, OK lub zielony: zatwierdzenie.
- 1–4: bezpośrednia odpowiedź. Żółty: powtórz lektora. Niebieski: przełącz lektora. Czerwony: menu.
- Opcjonalne zatwierdzanie po 5 sekundach od zmiany zaznaczenia.
- Na telefonie i komputerze: dotyk, mysz lub klawiatura.
- Test pilota i dźwięku w menu głównym; dostępność zdarzeń klawiszy zależy od TV.

## Lektor
Polskie nagrania MP3 generowane bez płatnego API przez eSpeak NG, workflow .github/workflows/quiz-audio.yml. Alternatywnie używana jest synteza systemowa, jeżeli przeglądarka ją udostępnia. Nagrania są dzielone na pytania, odpowiedzi, litery i komunikaty, aby kolejność odpowiedzi mogła być losowa.

## Aktualizacje
Baza znajduje się w bloku JSON o identyfikatorze bank w index.html. Pierwsza odpowiedź w każdym wierszu jest poprawna; aplikacja losuje jej pozycję. Obecne 4 działy mają po 20 pytań. Po zmianie struktury bazy należy odpowiednio zmienić logikę działów i generator audio. Po wygenerowaniu nowych plików audio przez GitHub Actions należy zainicjować publikację Pages (np. zwykłym commitem dokumentacji), gdyż commit wykonany przez GITHUB_TOKEN może nie wyzwolić publikacji ze źródłowej gałęzi.

Dotychczasowy plik Konkurs na 2.html pozostaje bez zmian.
