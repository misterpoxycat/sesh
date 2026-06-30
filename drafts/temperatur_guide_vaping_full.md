# 🌬️ Guide til temperaturer og effekter ved vaping af cannabis
*(Optimeret til XMAX V3 Pro med kapsel — Beregnet til forsknings- og undervisningsbrug i jurisdiktioner hvor cannabis er lovligt.)*

> **Vigtigt juridisk & etisk forbehold:** Dette dokument er udarbejdet udelukkende til **forskning, undervisning og harm-reduktion** i jurisdiktioner, hvor indholdet er lovligt. Det er **ikke** en opfordring til ulovlig aktivitet. Undersøg altid lokale love og regler, og søg sundhedsfaglig rådgivning ved behandlings-/medicinsk brug.

---

## Indholdsfortegnelse
1. Forståelse af setup (XMAX V3 Pro + kapsel)
2. Cannabinoider — temperaturer og effekter
3. Terpener — temperaturer, aroma og virkning
4. Temperaturzoner og session-flow
5. Temperaturkort (tekst-visualisering)
6. Effektmatrix (kombinationer af stoffer + terpener)
7. Metode & noter (hvordan disse intervaller er estimeret)
8. Referencer & videre læsning
9. MyST/Jupyter Book-visningsnoter

---

## 1) Forståelse af setup (XMAX V3 Pro + kapsel)
- XMAX V3 Pro er en hybrid (konduktion + konvektion). Brug af **metal-dosing-kapsel** ændrer varmeoverførsel: kapslen fungerer som varmebuffer og kan skabe et varmetab imellem den angivne enhedstemperatur og den faktiske urte-temperatur.
- I praksis ses ofte at den reelle urtetemperatur er **10–15 °C lavere** end den indstillede temperatur på enheden ved brug af kapsel. Når tabellen nedenfor angiver "Justeret (kapsel)" er dette allerede indregnet.

**Kort metode-note:** "Reel fordampning" er litteratur-baserede estimeringer for hvor forbindelse begynder at frigives; "Justeret til XMAX V3 Pro med kapsel" er et konservativt skøn +10–15 °C.

---

## 2) Cannabinoider — temperaturer og effekter (justeret til XMAX V3 Pro med kapsel)

| Cannabinoid | Reel fordampning (°C) | Justeret til XMAX V3 Pro med kapsel (°C) | Effekt / high |
|-------------:|:---------------------:|:----------------------------------------:|:-------------|
| **CBG**      | ~125 °C               | **135–145 °C**                            | Mild energi, fokus; forstadie for andre cannabinoider |
| **THC (Δ9)** | ~157 °C               | **165–175 °C**                            | Psykoaktiv, eufori, kreativ "head-high" |
| **CBD**      | ~160–180 °C           | **170–190 °C**                            | Ikke-psykoaktiv; balance, angstreduktion, kropsro |
| **CBN**      | ~185 °C               | **195–205 °C**                            | Nedbrydningsprodukt af THC; sedativ, kropslig effekt |
| **THCV**     | ~220 °C               | **230–240 °C**                            | Stimulerende, appetitmodulerende (sjældnere) |

> Bemærk: De angivne intervaller er estimater med usikkerhed. Prøve-til-prøve variation forekommer pga. matrix-effekter, fugtighed, partikelstørrelse og device-variation.

---

## 3) Terpener — temperaturer, aroma og virkning (justeret til kapsel)

| Terpen | Normal fordampning (°C) | Justeret (kapsel) (°C) | Aroma | Typisk virkning |
|--------|:-----------------------:|:----------------------:|:-----:|:---------------|
| **Pinene**      | ~155 °C | **165–170 °C** | Fyrretræ | Fokus, klarhed, modvirker hukommelsespåvirkning |
| **Myrcen**      | ~166 °C | **175–180 °C** | Jordet, moskus | Muskelafslappende, can fremme "couch-lock" |
| **Limonen**     | ~176 °C | **185–190 °C** | Citrus | Opløftende, antidepressiv, energigivende |
| **Linalool**    | ~198 °C | **205–215 °C** | Lavendel | Beroligende, angstdæmpende |
| **Caryophyllen**| ~200 °C | **210–220 °C** | Krydret, peber | Anti-inflammatorisk, CB2-interaktioner |

> Terpener har ofte relativt smalle aktive vinduer — høje temperaturer kan hurtigt reducere aroma (termisk nedbrydning).

---

## 4) Temperaturzoner (anbefalede forsknings-/observationszoner, justeret til kapsel)
> Brug som analytisk ramme for observationer; giv altid konkrete målinger, datapunkter og usikkerhedsintervaller i din dokumentation.

| Zone | Enhedsindstilling (°C) | Cirka reel urte-temp (°C) | Karakteristik |
|------|-----------------------:|:-------------------------:|:--------------|
| Klar & kreativ | **170–180 °C** | ~160–170 °C | Primært THC + tidlige terpener (pinene) — let, cerebral |
| Balanceret | **185–195 °C** | ~175–185 °C | THC + CBD + limonen — klassisk "all-round" |
| Tung & afslappende | **200–210 °C** | ~190–200 °C | Øget CBN & tungere terpener — kropslig afslapning |
| Ekstraktion / sedativ | **215–230 °C** | ~205–220 °C | CBN/caryophyllen dominerer; terpener nedbrydes |

---

## 5) Temperaturkort — tekst-visualisering (bogstavelig blok i Markdown)
> Nedenstående er et tekstbaseret "bar chart" design, beregnet til visning som kodeblok i Jupyter Book (så den vises ufortolket).

```text
135°C 140°C 145°C 150°C 155°C 160°C 165°C 170°C 175°C 180°C 185°C 190°C 195°C 200°C 205°C 210°C 215°C 220°C 225°C 230°C 235°C 240°C
CBG   🟩🟩🟩
THC                       🟧🟧🟧🟧🟧
CBD                              🟦🟦🟦🟦🟦🟦
CBN                                                  🟪🟪🟪🟪🟪
THCV                                                                                   🔴🔴🔴

Farvekoder:
🟩 = CBG   🟧 = THC   🟦 = CBD   🟪 = CBN   🔴 = THCV
```

---

## 6) Terpener — tekst-visualisering (bogstavelig blok)

```text
165°C 170°C 175°C 180°C 185°C 190°C 195°C 200°C 205°C 210°C 215°C 220°C
Pinene      🌲🌲
Myrcen           🌿🌿
Limonen               🍋🍋
Linalool                           💜💜💜
Caryophyllen                              🌶️🌶️🌶️

Symbolforklaring:
🌲 = Pinene   🌿 = Myrcen   🍋 = Limonen   💜 = Linalool   🌶️ = Caryophyllen
```

---

## 7) Effektmatrix — kombinationer og stemninger (forsknings-venlig tabel)
> Tabel til observation og tolkning af hvilke kombinationer af cannabinoider og terpener der typisk assosieres med bestemte oplevelsestyper.

| Temperatur (°C) | Aktive stoffer (est.) | Terpener (est.) | Stemning / Effekt | Typisk brug / observation |
|-----------------|------------------------|------------------|-------------------|---------------------------|
| 170–180 | THC + CBG | Pinene + Myrcen | Klar, energisk, kreativ | Dagtid, socialt, kreativt arbejde |
| 185–195 | THC + CBD | Limonen + Myrcen | Balanceret, glad, social | Hverdag, afslapning uden træthed |
| 200–210 | THC + CBD + CBN | Linalool + Caryophyllen | Rolig, kropslig, sedativ | Aften, film, restitution |
| 215–230 | CBN + Caryophyllen | (terpener falder) | Søvndyssende, meget kropslig | Inden sengetid, smertereduktion |

---

## 8) Metode & noter
- Temperaturintervaller er estimeret ud fra offentligt tilgængelig litteratur over kogepunkter/fordampningspunkter for rene forbindelser samt praktiske justeringer for metal-kapsler i konduktions-/konvektions-enheder.
- Variabler der påvirker resultater: fugtindhold i materiale, partikelstørrelse, homogenitet, mængde i kapsel, enhedsfejlmargin, batteristatus, omgivelser (vind, ventilation).
- For videnskabelig dokumentation: mål altid *den faktiske* urenhed/compound-udledning under kontrollerede forhold (fx ved hjælp af termokamera eller inline termistorer), og rapporter usikkerheder.

---

## 9) Referencer & videre læsning (eksempler — find og indsæt relevante kilder i din endelige version)
- Generelle reviews om cannabis-kemi, cannabinoid-fysik og terpener.
- Publikationer om fordamplingsfysik og apparatvariationer.
- Laboratorie-COA-metoder og standarder for cannabis-analyse.
(Erstat med konkrete kilder fra PubMed, ACS, eller akkrediterede laboratorier i din endelige rapport.)

---

## 10) MyST / Jupyter Book visningsnoter
- For at sikre at tekst-visualiseringerne ikke bliver `renderet` som almindelig Markdown i Jupyter Book, indpak dem i `{code-block}` eller triple-backtick med `text`:

````md
```{code-block} text
:caption: Temperaturkort (tekst-visualisering)
:class: copybutton
...indsæt blok...
```
````

- Overvej at bruge `admonition`-bokse til juridiske og etiske forbehold:

```md
```{admonition} Juridisk og etisk forbehold
:class: admonition-warning

Dette materiale er udelukkende til forskning/undervisning i jurisdiktioner, hvor det er lovligt.
```
```

---

### Appendiks: Eksempel på "Session-profil" (bare som illustration — dokumentér eksperimentelt)
> Hvis du vil indsamle observationsdata på sessioner i et kontrolleret, lovligt studie, så log parametre som: indstillet enhedstemp, tid i hver fase, mængde/masse i kapsel, subjektive effektskalaer, og eventuelle biomålinger. Sørg for etisk godkendelse (IRB/Etik) ved involvering af mennesker.

---

**Udgave:** 1.0 — samlet fra tidligere udveksling; verificér alle tal før publicering.
