# Portal dydaktyczny – dr inż. Paweł Strączyński

Statyczna strona przygotowana do publikacji w GitHub Pages. Nie wymaga serwera, bazy danych ani instalacji bibliotek.

## Publikacja na GitHub Pages

1. Utwórz publiczne repozytorium `<twoj-login>.github.io` na GitHubie.
2. Wgraj **zawartość** tego folderu do katalogu głównego repozytorium (plik `index.html` musi leżeć w katalogu głównym, a nie dodatkowym podfolderze).
3. Wybierz `Settings → Pages → Build and deployment → Deploy from a branch → main → /(root)` i kliknij `Save`.
4. Odwiedź `https://<twoj-login>.github.io/`.

## Jak zmienić przedmioty

W pliku `assets/data.js` zmień tablicę `subjects`. Każdy przedmiot ma identyfikator `id`, skrót `code`, tytuł `title`, opis `description`, zakładki `tabs` i listę materiałów `materials`.

Przedmioty zostały uaktualnione zgodnie ze zrzutem ekranu planu zajęć przesłanym 1.11.2026. Podział na wykłady i laboratoria odzwierciedla rodzaje zajęć z obrazu; treści materiałów są na razie pustymi pozycjami, nie gotowymi plikami.

## Jak udostępnić PDF

1. Wgraj plik np. do `materialy/socr/wyklady/wyklad_01.pdf`.
2. W `assets/data.js` zmień lub dodaj wpis:

```js
{ category:'Wykłady', title:'Wykład 1 — Wprowadzenie', description:'Prezentacja PDF', type:'PDF', published:true, path:'materialy/socr/wyklady/wyklad_01.pdf' }
```

3. Zapisz zmiany w GitHub. Przycisk `Pobierz` będzie widoczny automatycznie.

Pliki z `published:false` pozostają oznaczone jako „W przygotowaniu” i nie udają istniejących materiałów.

## Co można zmienić

- Kolory i układ: `assets/style.css`
- Przedmioty, ogłoszenia i materiały: `assets/data.js`
- Nazwa i opis strony: `index.html`
- Nawigacja i mechanizmy wyszukiwania: `assets/app.js`

## Uwaga

GitHub Pages jest stroną publiczną. Nie zamieszczaj ocen, danych osobowych, materiałów poufnych ani innych plików wymagających logowania. Przy użyciu cudzych materiałów respektuj prawa autorskie.
