# hippolog
Mobiele logboek-app voor leerlingen op stage: uren, taken en notities per dag, alles op je eigen toestel. Exporteer naar markdown en laat een AI-tool naar keuze je weekverslag schrijven. Eén HTML-bestand, geen server, geen accounts. A Dutch-language work log for students on placement.

Gemaakt voor mijn dochter, die drie dagen per week op een paardenbedrijf werkt.

**Live:** [hippolog.net](https://hippolog.net)

<img width="2880" height="2160" alt="hero_hippolog_github" src="https://github.com/user-attachments/assets/4addc34c-aace-48a0-a199-68ecbe061836" />

## Wat het doet

- Eén dag per scherm, met een groen vinkje of rood vraagteken of die dag al ingevuld is
- Standaarduren per weekdag, maar elke dag blijft invulbaar
- Aanpasbare takenlijst: groepen en taken toevoegen, hernoemen, verwijderen en verslepen
- Autosave, met alleen een melding als het misloopt
- Backup naar `.md` en terug importeren
- Volgt licht en donker van het toestel, werkt offline, kan op het beginscherm

## Het .md bestand

Backup én invoer voor het weekverslag. De leerling voegt het toe aan ChatGPT, Gemini of Claude met de prompt die in de app staat, onder Instellingen. Eén bestand mag een heel schooljaar bevatten.

```markdown
## 2026-09-09 (woensdag)
- Uren: 08:00 - 16:00
- Notitie: Twee paarden gelongeerd en de piste gesleept.

### Paarden
- [x] Hooi geven
- [ ] Wassen
```

Dezelfde parser schrijft en leest dit formaat.

## Technisch

Eén bestand, `index.html`. CSS, JavaScript en de iconen zitten erin. Geen libraries, geen build, geen tracking. Gegevens in `localStorage` onder `hippolog.v1`. Zelf hosten doe je door `index.html` ergens neer te zetten.

Het versienummer staat onderaan de instellingen, in de vorm `v2026.09.07 22:16`.

## Licentie

MIT, je krijgt de vrije teugels. De app is niet aan paarden gebonden: wie stage loopt in een garage of een keuken zet er gewoon andere taken in.
