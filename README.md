# Algoritmelab – VG1 IM

En interaktiv, pedagogisk simulering av et anbefalingssystem, laget for undervisning om medievaner, algoritmer og personalisering.

## Publiser på GitHub Pages

1. Opprett et nytt GitHub-repository, for eksempel `algoritmelab`.
2. Last opp `index.html`, `style.css` og `app.js` til roten av repositoryet.
3. Åpne **Settings → Pages**.
4. Velg **Deploy from a branch**, `main` og `/ (root)`, og lagre.
5. Etter publisering åpner du adressen GitHub Pages viser.

Du kan også teste nettsiden lokalt ved å åpne `index.html` i nettleseren.

## Undervisningsforslag (25–35 min)

- 5 min: Forklar begrepene anbefalingssystem, personalisering og brukerdata.
- 7 min: Forsøk A. Velg én kategori og gi den positive signaler; bruk negative eller nøytrale signaler på andre kategorier. Minst 15 handlinger.
- 7 min: Forsøk B. Gi positive signaler til flere kategorier. Minst 15 handlinger.
- 5 min: Sammenlign resultatene (CSV kan åpnes i regneark).
- 5–10 min: Diskuter hvorfor modellen også anbefaler nye temaer, og hvordan algoritmer kan påvirke medievaner.

## Viktig om modellen

Det finnes 30 fiktive videoer fordelt på seks kategorier. Handlingssignalene er: hopp over −1, se ferdig +2, lik +3, ikke interessert −3. Ved neste anbefaling velges kategori 65 % av gangene etter vekt `max(1, 3 + interessepoeng)` og 35 % av gangene tilfeldig (utforsking). Deretter velges en tilfeldig usett video fra kategorien. Resultatene vil variere mellom forsøk, også med like handlinger.

Dette er **ikke** en kopi av TikTok, YouTube eller andre plattformers anbefalingsalgoritmer. Virkelige systemer bruker langt flere signaler og mer komplekse modeller.

## Personvern og teknikk

Nettsiden er statisk, uten kontoer, cookies, analyseverktøy eller eksterne API-er. Data holdes bare i minnet i den åpne fanen, og CSV lastes ned lokalt. Ingen informasjon sendes til en server av applikasjonen.
