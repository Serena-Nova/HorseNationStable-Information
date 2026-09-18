# Horse Nation Stalmanagement

E�n bestand (`index.html`) — geen build nodig, werkt direct via GitHub Pages.
Dit vervangt de losse Kladblok-app: alles zit nu in één app, met twee tabbladen.

## Zetten op GitHub Pages
1. Maak een nieuwe repository aan (bijv. `Horse-nation-stalmanagement`) op je `serena-nova` account.
2. Upload `index.html` en `.nojekyll` naar de `main` branch (root van de repo).
3. Ga naar **Settings → Pages**, kies branch `main` / map `/ (root)`, sla op.
4. Na een minuutje staat je app op `https://serena-nova.github.io/Horse-nation-stalmanagement/`.

Let op: dit is een NIEUWE, LEGE stamboom-database (de losse Horse-stamboom-app blijft
gewoon bestaan op zijn eigen URL, met al je oude stambomen erin — die zijn hier nog niet
overgezet). Je Kladblok-gegevens (paarden, groepen, legenda, kleuren) staan er wel meteen in,
want die komen automatisch uit je vorige Kladblok-versie mee als je 'm in dezelfde browser opent.
Zet je oude Kladblok-versie dus niet weg voor je hebt gecontroleerd dat deze nieuwe versie
alles goed heeft overgenomen.

## De twee tabbladen
- **Kladblok** — precies wat je al had: groepen, kleuren, status-iconen, enz. Nieuw:
  elk paard heeft nu ook een "Vader" en "Moeder" veld (voor de Stamboom-tab) en optionele
  S/D/G-invulvelden.
- **Stamboom** — nieuw. Zoek een paard, vul de vader/moeder in (met auto-aanvullen uit je
  hele database, stal + extern), en zie de stamboom als boomstructuur. Voeg externe paarden
  toe (paarden die niet in jouw stal staan) via "+ Extern paard toevoegen". Onderaan zit een
  inteelt-check (COI): vul een hengst en merrie in en zie het inteeltpercentage over 4
  generaties, met welke voorouders ze delen.

## Wat er (nog) niet in zit t.o.v. je oude Stamboom-app
Bewust weggelaten om dit stap 1 behapbaar te houden — kan later alsnog toegevoegd worden:
- De sleepbare whiteboard-weergave (nu een boomstructuur in plaats van kaartjes die je verschuift)
- Automatische kleur per paard in de stamboomweergave
- De "beste combinaties"-scanner
- Bulk-import, zoom, "losse paarden"-archief

## Werking
- Alles wordt automatisch bewaard in de browser (localStorage) — geen account nodig.
- Onderaan de Kladblok-tab: **Exporteer JSON** (neemt Kladblok + Stamboom-data mee) en
  **Importeer JSON** voor een back-up.
