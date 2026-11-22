# 🔊 Ustawiacz Głośników AR

Aplikacja AR (WebXR) pokazuje w prawdziwym pokoju, gdzie postawić każdy głośnik kina domowego (2.0 – 7.1.4, kąty wg schematów Dolby).
Działa na **telefonie z Androidem (Chrome + ARCore)** i na **Meta Quest 3** (przeglądarka Questa). Po pierwszym otwarciu działa **offline**.

## Uruchomienie (z samego telefonu)
1. Na GitHubie utwórz nowe repozytorium, np. `glosniki-ar` (publiczne).
2. **Add file → Upload files** i wrzuć: `index.html`, `sw.js`, `manifest.json`, `icon-192.png`, `icon-512.png`.
3. **Settings → Pages → Branch: main / (root) → Save**.
4. Po ok. minucie aplikacja jest pod adresem `https://mlynek1111.github.io/glosniki-ar/`.

## Użycie
- **Telefon:** Start AR → poruszaj powoli telefonem, aż pojawi się celownik → tapnij telewizor → tapnij podłogę pod miejscem siedzenia.
- **Quest 3:** celuj kontrolerem, spust = wybierz, grip = cofnij. Z konfiguracją przestrzeni aplikacja widzi ściany i przysuwa do nich głośniki, które wypadłyby za ścianą.
- **Plan z góry** na stronie startowej działa na każdym urządzeniu (także iPhone/PC).

## Skanowanie pokoju
- Quest 3: używa ścian i mebli z systemowej konfiguracji przestrzeni (WebXR `plane-detection`).
- Android: ARCore sam wykrywa podłogę i ściany przy ruchu kamerą (`hit-test`).
