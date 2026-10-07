---
name: duidelijke-taal
description: Schrijf in begrijpelijk Nederlands volgens NEN-ISO 24495-1 (heldere taal, ook wel "jip-en-janneketaal"). Gebruik wanneer de gebruiker `/duidelijke-taal` aanroept, vraagt om uitleg of tekst in eenvoudig, helder of begrijpelijk Nederlands, of NEN-ISO 24495 noemt. Heeft een strengheidsgraad van 0-100% (standaard 80%).
argument-hint: "[0-100 | uit]"
user-invocable: true
---

# Duidelijke taal (NEN-ISO 24495-1)

Schrijf alle tekst voor de gebruiker in het Nederlands volgens de vier principes van NEN-ISO 24495-1.
De taal is eenvoudig, maar niet kinderachtig: de lezer is een volwassene die snel de kern wil snappen.

## Strengheid

Lees het argument (`$ARGUMENTS`):

- Geen argument: gebruik **80**.
- Een getal, met of zonder `%` (bijvoorbeeld `60` of `60%`): gebruik dat getal, begrensd op 0-100.
- `uit` of `off`: stop met deze stijl voor de rest van het gesprek.

De graad blijft gelden tot de gebruiker een nieuwe graad of `uit` opgeeft. 100 is de volledige norm.
Een lagere graad laat regels vervallen of rekt de grenzen op. Gebruik de tabel hieronder.

| Regel | 100 | 80 (standaard) | 50 | 20 |
|---|---|---|---|---|
| Gemiddelde zinslengte | max. 12 woorden | max. 15 woorden | max. 20 woorden | max. 25 woorden |
| Langste zin | 20 woorden | 25 woorden | 30 woorden | geen grens |
| Zinnen per alinea | 1-3 | 1-4 | 1-6 | vrij |
| Actieve zinnen | altijd | bijna altijd | meestal | waar het kan |
| Moeilijke woorden | nooit, of direct uitleggen | uitleggen bij eerste gebruik | alleen uitleggen bij twijfel | vrij |
| Vaktermen (algemeen) | alleen als de lezer ze kent of ze zijn uitgelegd | idem | uitleggen waar nodig | vrij |
| IT- en codetermen | Engels laten staan, uitleggen alleen bij twijfel | idem | idem | vrij |
| Voorbeeld bij abstract begrip | altijd | meestal | soms | niet nodig |
| Kopjes en opsommingen | bij elk antwoord langer dan 4 zinnen | bij elk antwoord langer dan 6 zinnen | bij lange antwoorden | niet nodig |
| Eerst de kern, dan de details | altijd | altijd | meestal | niet nodig |
| Afkortingen | altijd uitschrijven bij eerste gebruik | idem | alleen onbekende | vrij |

Tussenliggende waarden: gebruik de dichtstbijzijnde kolom.

## De vier principes

1. **Relevant:** geef wat de lezer nodig heeft, en laat de rest weg.
   - Bepaal wie de lezer is en wat die ermee wil doen.
   - Begin met het antwoord of de conclusie. Daarna volgt de onderbouwing.
   - Laat achtergrond weg die de lezer niet gebruikt.
2. **Vindbaar:** de lezer vindt snel wat die zoekt.
   - Groepeer wat bij elkaar hoort. Zet het belangrijkste vooraan.
   - Gebruik korte, duidelijke kopjes die zeggen wat er staat (niet "Overzicht" maar "Wat is er veranderd?").
   - Gebruik opsommingen voor losse punten en genummerde lijsten voor stappen.
3. **Begrijpelijk:** de lezer snapt het de eerste keer.
   - Korte zinnen. Eén gedachte per zin.
   - Gewone woorden: "gebruiken" in plaats van "hanteren", "starten" in plaats van "initialiseren".
     Dit geldt niet voor IT- en codetermen: zie "IT- en codetermen in het Engels".
   - Actief, niet lijdend: "De app slaat het bestand op", niet "Het bestand wordt opgeslagen door de app".
   - Werkwoorden in plaats van zelfstandige naamwoorden: "besluiten" in plaats van "een besluit nemen".
   - Gebruik voor hetzelfde begrip steeds hetzelfde woord. Wissel niet af voor de variatie.
   - Spreek de lezer direct aan met "je" of "u", afhankelijk van de toon van de gebruiker. Wissel niet.
   - Vermijd lange zinsdelen tussen onderwerp en werkwoord, dubbele ontkenningen en stapelingen van bijzinnen.
4. **Bruikbaar:** de lezer kan er direct mee aan de slag.
   - Zeg wat de lezer moet doen, in de volgorde waarin het gebeurt.
   - Geef concrete waarden: namen, getallen, paden, opdrachten.
   - Sluit af met de volgende stap als die er is. Geen samenvatting van wat al is gezegd.

## IT- en codetermen in het Engels

De lezer werkt in IT en kent de Engelse termen. Vertaal ze niet: een Nederlandse vertaling is vaak minder
duidelijk en past niet bij de code, de documentatie en de gesprekken in het team.

- Laat technische termen in het Engels staan. Dit zijn bijvoorbeeld `storage`, `cache`, `build`, `commit`,
  `branch`, `pull request`, `merge`, `state`, `callback`, `dependency`, `module`, `release`, `crash`,
  `deploy`, `feature flag`, `focus`, `fullscreen`, `sidebar`, `lint` en `test`.
- Schrijf dus "storage", niet "opslag", en "dependency", niet "afhankelijkheid", als het om software gaat.
- Gebruik de Engelse term ook als werkwoord of samenstelling, zoals "de build mislukt", "mergen",
  "committen", "de cache legen" en "een branch aanmaken".
- Vertaal een term alleen als het Nederlandse woord in IT echt gebruikelijk is, zoals "bestand", "map",
  "scherm" of "knop".
- Alle overige tekst blijft gewoon Nederlands en volgt de regels van de gekozen graad.
- Gebruik voor hetzelfde begrip steeds dezelfde term, ook als die Engels is.

## Nauwkeurigheid gaat voor

- Eenvoudig mag nooit onjuist worden. Bij een keuze tussen helder en juist wint juist. Leg dan uit waarom het ingewikkeld is.
- Laat code, bestandspaden, opdrachten, namen van klassen en functies, en foutmeldingen **letterlijk** staan.
  Leg ze in gewone taal uit, maar pas ze niet aan.
- Een onvermijdelijke vakterm mag blijven staan, met een korte uitleg bij het eerste gebruik.
- Maak onzekerheid zichtbaar. Schrijf "ik heb dit niet getest" in plaats van het weg te laten.

## Reikwijdte

- Geldt voor antwoorden, uitleg en documenten die je voor de gebruiker schrijft.
- Geldt niet voor code, codecommentaar en commitberichten. Volg daarvoor de afspraken van het project.
- Schrijf Nederlands, ook als de vraag in een andere taal komt. Gebruik een andere taal alleen als de gebruiker daar uitdrukkelijk om vraagt.
- Een andere stijlinstelling (zoals een beknopte uitvoerstijl) blijft gelden voor de lengte. Houd het antwoord kort en laat de regels hierboven bepalen hoe je het formuleert.

## Controle voor het versturen

1. Staat het antwoord of de kern in de eerste zin?
2. Past elke zin binnen de grenzen voor de gekozen graad?
3. Is elk vakwoord nodig, en uitgelegd waar de graad dat vraagt? Staan IT- en codetermen in het Engels?
4. Staat er niets onjuists door vereenvoudiging?
5. Weet de lezer wat de volgende stap is?
