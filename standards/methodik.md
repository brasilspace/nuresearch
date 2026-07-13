# nuresearch — Rechercherahmen & Dokumentstandard für Dossiers

**Dokument-Key:** `methodik`
**Status:** v1.0 — freigegeben durch CEO/Chief of Staff am 2026-07-13
**Owner:** Marlene (Founding Research Analyst)
**Zweck:** Verbindliches Fundament-Dokument. Jedes künftige nuresearch-Dossier baut auf dieser Gliederung, Quellen- und Zitationskonvention auf. Dieses Dokument ist selbst ein Deliverable-Muster: Es trennt Fakten und Annahmen und weist seine Quellen aus.

---

## 1. Executive Summary (dieses Standards)

- Ein **Dossier** ist ein strukturiertes Markdown-Dokument mit fester Gliederung (Abschnitt 2), das eine Rechercheeinheit (z. B. ein Wirkstoff, eine Kombination oder eine Fragestellung) belegbasiert abbildet.
- Jede zentrale Aussage ist **entweder belegt (mit Quelle) oder als Annahme/Schätzung gekennzeichnet** — beides wird niemals vermischt (Abschnitt 5). Das ist das Kernprinzip von nuresearch.
- Quellen werden nach einer **Evidenzhierarchie** (Abschnitt 3) und nach **Aktualität + Interessenkonflikten** bewertet und im **einheitlichen Zitationsformat** (Abschnitt 4) angegeben.
- Gesundheitsbezogene Aussagen durchlaufen vor Abgabe eine **Health-Claims-/HWG-Checkliste** (Abschnitt 6).
- **Definition of Done** und ein **Abnahme-Checkliste** stehen in Abschnitt 7.
- nuresearch liefert **ausschließlich Text/Markdown** — keine Software, keine individuelle medizinische oder rechtliche Beratung.

---

## 2. Standard-Gliederung eines Dossiers

Jedes Dossier verwendet die folgenden Abschnitte in dieser Reihenfolge. Nicht zutreffende Abschnitte werden **nicht gelöscht**, sondern mit „Nicht anwendbar" oder „Keine belastbare Quellenlage" gekennzeichnet, damit Lücken sichtbar bleiben.

| # | Abschnitt | Inhalt / Zweck | Pflicht |
|---|-----------|----------------|---------|
| 0 | **Kopf / Metadaten** | Titel, Dokument-Key, Version, Datum, Autor:in, Status, Stichjahr der Marktdaten | Ja |
| 1 | **Executive Summary / Kernaussagen** | 3–7 Bullets mit den wichtigsten belegten Erkenntnissen + höchster Evidenzgrad; zuerst lesbar | Ja |
| 2 | **Wirkstoff / Mechanismus** | Substanzdefinition, chemische Form(en), Bioverfügbarkeit/Matrix, postulierter Wirkmechanismus | Ja |
| 3 | **Studienlage** | Evidenztabelle: Studientyp, n, Population, Dosis, Dauer, Endpunkte, Effektgröße, Evidenzgrad, Quelle | Ja |
| 4 | **Sicherheit** | Nebenwirkungen, Tolerable Upper Intake Level (UL), Wechselwirkungen, Kontraindikationen, Risikogruppen | Ja |
| 5 | **Markt** | Marktdaten, Wettbewerb, Segmente — je mit Quelle **und Stichjahr** | Nach Auftrag |
| 6 | **Zielgruppen** | Für wen gilt die Evidenz (Alter, Geschlecht, Vorerkrankung); Übertragbarkeit der Studienpopulation | Ja |
| 7 | **Regulatorik** | Health-Claims-Status (zugelassen/pending/unzulässig), HWG-/LFGB-/Novel-Food-Einordnung | Ja |
| 8 | **Offene Punkte / unklare Quellenlage** | Explizit benannte Lücken, Widersprüche, veraltete Evidenz, ungeklärte Fragen | Ja |
| 9 | **Quellen** | Vollständige Referenzliste im Zitationsformat (Abschnitt 4) | Ja |
| 10 | **Glossar** | Fachbegriffe, Abkürzungen | Bei Bedarf |

**Konventionen für die Studienlage-Tabelle (Abschnitt 3 eines Dossiers):**

| Studie (Quelle) | Typ | n | Population | Dosis / Form | Dauer | Endpunkt(e) | Ergebnis / Effektgröße | Evidenzgrad |
|---|---|---|---|---|---|---|---|---|
| _z. B. [Autor Jahr]_ | RCT / Meta-Analyse / Kohorte … | | | | | | inkl. p-Wert **und** Effektmaß (RR, OR, MD, SMD, CI) | A–D (s. 3.1) |

Regel: **Statistische Signifikanz ≠ klinische Relevanz.** Immer Effektgröße + Konfidenzintervall angeben, nicht nur „signifikant". Dosis/Form/Population müssen zur Fragestellung passen (Bioverfügbarkeits- und Zielgruppen-Lens).

---

## 3. Quellenqualitäts-Rubrik

### 3.1 Evidenzhierarchie

Absteigende Aussagekraft für Wirksamkeitsfragen (angelehnt an OCEBM Levels of Evidence und den GRADE-Ansatz — siehe Quellen):

| Grad | Studientyp | Aussagekraft |
|---|---|---|
| **A** | Systematische Review / Meta-Analyse von RCTs | höchste |
| **A/B** | Einzelnes, gut designtes RCT (randomisiert, kontrolliert, verblindet) | hoch |
| **B** | Kohortenstudie (prospektiv) | mittel-hoch |
| **C** | Fall-Kontroll-Studie, Querschnittsstudie | mittel |
| **C/D** | Fallserie, unkontrollierte Studie | niedrig |
| **D** | In-vitro / Tierstudie, Mechanismus-Plausibilität | niedrig (nicht auf Menschen übertragbar ohne Humanevidenz) |
| **D** | Expertenmeinung, Erfahrungsbericht, Herstellerangabe | niedrigste |

Regel: **Der genannte Evidenzgrad gehört zu jeder zentralen Wirkaussage.** Mechanistische Plausibilität (in-vitro/Tier) allein rechtfertigt **keine** Wirkaussage für den Menschen.

### 3.2 Quellenklassen: Primär / Sekundär / Tertiär

- **Primärquelle** — Originalstudie / Originaldaten (z. B. RCT-Publikation in einem peer-reviewten Journal, EFSA-Gutachten, amtlicher Verordnungstext). **Bevorzugt.**
- **Sekundärquelle** — Aggregation/Bewertung von Primärquellen (systematische Review, Meta-Analyse, Cochrane-Review, Leitlinie).
- **Tertiärquelle** — Lehrbuch, Enzyklopädie, Fachportal-Zusammenfassung, Behörden-Merkblatt. Nur zur Einordnung/Definition, **nicht** als alleiniger Beleg für eine Wirkaussage.

Rangfolge bei der Belegwahl: **Primär > Sekundär > Tertiär.** Für aggregierte Wirksamkeitsaussagen sind Sekundärquellen (Meta-Analysen/Cochrane) oft die beste verfügbare Ebene — Primär- und Sekundärquelle können sich ergänzen.

**Blogs, Hersteller-Marketing und KI-Zusammenfassungen sind keine zitierfähigen Belege** für Wirk-, Markt- oder Sicherheitsaussagen. Sie dürfen höchstens als Kontext/Signal genannt und dann als solche gekennzeichnet werden.

### 3.3 Aktualität

- Publikationsjahr **immer** angeben.
- Faustregel: Für schnelllebige Felder (Markt, Regulatorik, laufende Studienlage) Quellen **≤ 5 Jahre** bevorzugen; ältere Quellen nur, wenn sie weiterhin Referenz sind (z. B. Grundlagenverordnung, etablierter Mechanismus).
- Regulatorik **stets gegen die konsolidierte/aktuell gültige Fassung** prüfen (Verordnungen werden geändert).
- Bei Marktdaten das **Stichjahr** der Daten nennen, nicht nur das Publikationsjahr.

### 3.4 Interessenkonflikte & Verzerrung

Bei jeder wichtigen Quelle prüfen und bei Relevanz ausweisen:
- **Finanzierung / Sponsoring** (Herstellerfinanzierte Studien → Verzerrungsrisiko kennzeichnen).
- **Publikationsbias** (Nur positive Ergebnisse publiziert? Studienregister-Abgleich möglich?).
- **Interessenkonflikt-Erklärung** der Autor:innen.
- **Methodische Qualität** (Randomisierung, Verblindung, Drop-out, Präregistrierung).

---

## 4. Zitationsformat

Einheitliches Format für den Abschnitt „Quellen" jedes Dossiers:

> **[Kürzel]** Autor(en) oder Institution. *Titel.* Publikationsorgan/Herausgeber, Jahr. DOI oder stabiler Link. [Zugriffsdatum bei Webquellen]

**Beispiele (Formatmuster):**

- **[EU 2006]** Europäisches Parlament und Rat. *Verordnung (EG) Nr. 1924/2006 über nährwert- und gesundheitsbezogene Angaben über Lebensmittel.* Amtsblatt der EU, 2006. CELEX 32006R1924. https://eur-lex.europa.eu/legal-content/DE/ALL/?uri=celex%3A32006R1924
- **[Autor Jahr]** Nachname AB, Nachname CD. *Titel der Studie.* Journal. Jahr;Band(Heft):Seiten. doi:10.xxxx/xxxxx
- **[Institution Jahr]** EFSA Panel on … *Titel des Gutachtens.* EFSA Journal, Jahr. doi:… [zugegriffen JJJJ-MM-TT]

Regeln:
- Im Fließtext auf Quellen mit **[Kürzel]** verweisen; jede zentrale Zahl/Wirkaussage trägt einen Verweis.
- **DOI bevorzugt** vor URL (persistenter). Bei Webquellen ohne DOI: stabiler Link **+ Zugriffsdatum**.
- **Keine toten oder erfundenen Links.** Vor Abgabe jeden Link auf Erreichbarkeit prüfen.
- Primärquelle direkt zitieren, nicht „zitiert nach". Wenn nur Sekundärzitat verfügbar: als solches kennzeichnen.

---

## 5. Trennung von Fakten und Annahmen + Umgang mit fehlender Quellenlage

**Kernprinzip:** Jede Aussage ist genau eine von zwei Kategorien — belegter Fakt oder Annahme/Schätzung. Vermischung ist ein Abgabe-Blocker.

### 5.1 Kennzeichnungskonvention

- **Fakt (belegt):** Aussage + Quellenverweis **[Kürzel]**. Ohne Verweis gilt nichts als Fakt.
- **Annahme / Schätzung:** Präfix **„Annahme:"** bzw. **„Schätzung:"**, plus Begründung und Unsicherheitsgrad. Beispiel: _„Annahme: Der Markt wächst weiter im hohen einstelligen Prozentbereich (Extrapolation aus [X 2023], nicht separat belegt)."_
- **Interpretation/Einordnung** der Analystin: als solche kennzeichnen („Einordnung:"), von der zitierten Aussage getrennt halten.

### 5.2 Umgang mit fehlender / schwacher Quellenlage

- **Nicht raten, nicht erfinden.** Keine erfundenen Studien, Zahlen, Zitate oder Quellen — unter keinen Umständen.
- Lücke **offen benennen** im Abschnitt „Offene Punkte": Was fehlt, warum, welche Quelle wäre nötig.
- Wo möglich, mit dem weiterarbeiten, was belegbar ist; die Lücke isolieren statt sie zu überbrücken.
- Widersprüchliche Evidenz **beide Seiten** darstellen, nicht die bequemere wählen.
- Formulierung bei schwacher Evidenz vorsichtig halten („erste Hinweise aus einer kleinen Studie", nicht „belegt wirksam").

### 5.3 Verwendete Lenses (in Kommentaren/Begründungen benennen)

Fakt-vs-Annahme · Evidenzhierarchie · Quellenqualität & Aktualität · Health-Claims-Zulässigkeit · Effektgröße vs. Signifikanz · Bioverfügbarkeit & Form · Zielgruppen-Fit · Sicherheit & Obergrenzen.

---

## 6. Health-Claims- / HWG-Checkliste (Prüfschritt vor Abgabe)

Anzuwenden auf **jede gesundheitsbezogene Aussage** in einem Dossier. Ziel: klar kennzeichnen, was rechtlich zulässig **kommuniziert** werden dürfte — nicht individuelle Rechtsberatung.

1. **Ist es eine gesundheitsbezogene Angabe** im Sinne der VO (EG) Nr. 1924/2006? (Behauptung eines Zusammenhangs zwischen Lebensmittel/Inhaltsstoff und Gesundheit.)
2. **Status im EU-Register prüfen:** zugelassen / abgelehnt / pending (Art. 13/14-Claims). Im Zweifel als „ungeklärt" markieren und im EU-Register verifizieren.
3. **Zugelassenen Wortlaut / Bedingungen einhalten:** Nur mit belegtem Nährstoffgehalt und zulässiger Formulierung. Abweichende/übertreibende Formulierungen kennzeichnen.
4. **Krankheitsbezug (HWG):** Aussagen, die Krankheiten vorbeugen/behandeln/heilen, sind für Lebensmittel/NEM grundsätzlich **unzulässig** (Verbot krankheitsbezogener Angaben; HWG-Grenzen). → als unzulässig markieren.
5. **Novel-Food-Status** des Inhaltsstoffs prüfen (VO (EU) 2015/2283): zugelassen als Lebensmittel/-zutat? → sonst Vermarktungsschranke benennen.
6. **LFGB / Irreführungsverbot:** Keine irreführenden oder nicht belegten Wirkaussagen.
7. **Einordnung ins Dossier:** Jede gesundheitsbezogene Aussage bekommt ein Label — **[zulässig]**, **[pending]**, **[unzulässig]** oder **[ungeklärt — zu prüfen]** — mit Quellenverweis.

> Hinweis: Diese Checkliste ist ein Recherche-Prüfschritt, **keine Rechtsberatung im Einzelfall**. Verbindliche Prüfung bleibt bei Rechts-/Regulatory-Funktion bzw. externer Beratung.

---

## 7. Definition of Done & Abnahme-Checkliste

Ein Dossier ist abgabefertig, wenn **alle** Punkte erfüllt sind:

- [ ] Standard-Gliederung (Abschnitt 2) vollständig; nicht anwendbare Abschnitte gekennzeichnet.
- [ ] Executive Summary steht zuerst und ist ohne Volltext verständlich.
- [ ] Jede zentrale Aussage ist **belegt** oder **als Annahme/Schätzung markiert** — keine Vermischung.
- [ ] Alle Quellen sind **real, auffindbar, korrekt zitiert** (Format Abschnitt 4); kein toter/erfundener Link.
- [ ] Evidenzgrad je zentraler Wirkaussage angegeben; Effektgröße + CI statt nur „signifikant".
- [ ] Markt-/Zahlenangaben mit **Stichjahr**.
- [ ] Gesundheitsbezogene Aussagen mit Health-Claims-/HWG-Label (Abschnitt 6).
- [ ] Abschnitt „Offene Punkte" benennt Lücken und Widersprüche offen.
- [ ] Deliverable ist **Markdown, keine Software**, keine individuelle Beratung.

Abschlusskommentar am Issue enthält: Status, Link zum Dokument, Kurz-Zusammenfassung der Kernergebnisse, benannte offene Punkte, nächster Schritt / Empfänger der Übergabe.

---

## 8. Offene Punkte / unklare Quellenlage (dieses Standards)

- **Annahme:** Die Evidenzgrad-Skala (A–D, Abschnitt 3.1) ist eine pragmatische Synthese gängiger Frameworks (OCEBM, GRADE) für den nuresearch-Gebrauch, kein wörtliches Zitat einer einzelnen Norm. Bei Bedarf auf GRADE-Terminologie (hoch/moderat/niedrig/sehr niedrig) umstellbar. **Entscheidung CEO (2026-07-13): A–D beibehalten.**
- **Offen:** Ob ein separates, feiner granuliertes Zitations-Styleguide (z. B. Vancouver vs. APA) verbindlich vorgegeben werden soll. Aktueller Standard ist das pragmatische Format in Abschnitt 4. **Entscheidung CEO (2026-07-13): pragmatisches Format beibehalten, kein verbindlicher Vancouver/APA-Styleguide.**
- **Offen:** Der EU-Health-Claims-Register-Status einzelner Substanzen ist **dossierspezifisch zum Erstellungszeitpunkt** zu verifizieren — dieser Standard legt nur den Prüfschritt fest, nicht die konkreten Ergebnisse.
- **Zu ergänzen bei Bedarf:** Vorlage/Template als eigenes Dokument (`dossier-template`), sobald das erste Wirkstoff-Dossier beauftragt wird. **Entscheidung CEO (2026-07-13): auf diesen Zeitpunkt vertagt.**

---

## 9. Quellen

- **[EU 2006]** Europäisches Parlament und Rat. *Verordnung (EG) Nr. 1924/2006 über nährwert- und gesundheitsbezogene Angaben über Lebensmittel.* Amtsblatt der EU L 404, 2006; konsolidierte Fassung 02006R1924. CELEX 32006R1924. https://eur-lex.europa.eu/legal-content/DE/ALL/?uri=celex%3A32006R1924
- **[EU-Register]** Europäische Kommission. *EU Register of nutrition and health claims made on foods.* Laufend aktualisiert. https://food.ec.europa.eu/food-safety/labelling-and-nutrition/nutrition-and-health-claims/eu-register-health-claims_en (Datenbank: https://ec.europa.eu/food/food-feed-portal/screen/health-claims/eu-register )
- **[EU 2015]** Europäisches Parlament und Rat. *Verordnung (EU) 2015/2283 über neuartige Lebensmittel (Novel Food).* Amtsblatt der EU, 2015. CELEX 32015R2283. https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:32015R2283
- **[HWG]** *Gesetz über die Werbung auf dem Gebiete des Heilwesens (Heilmittelwerbegesetz — HWG).* Bundesrepublik Deutschland, in der jeweils geltenden Fassung. https://www.gesetze-im-internet.de/hwg/
- **[LFGB]** *Lebensmittel-, Bedarfsgegenstände- und Futtermittelgesetzbuch (LFGB).* Bundesrepublik Deutschland, in der jeweils geltenden Fassung. https://www.gesetze-im-internet.de/lfgb/
- **[EFSA]** European Food Safety Authority. *Health claims / Dietary Reference Values / Tolerable Upper Intake Levels.* https://www.efsa.europa.eu/en/topics/topic/health-claims
- **[BfR]** Bundesinstitut für Risikobewertung. *Nahrungsergänzungsmittel / Höchstmengen.* https://www.bfr.bund.de/
- **[Cochrane]** Cochrane Library. *Systematic reviews.* https://www.cochranelibrary.com/
- **[PubMed]** U.S. National Library of Medicine. *PubMed / MEDLINE.* https://pubmed.ncbi.nlm.nih.gov/
- **[OCEBM 2011]** OCEBM Levels of Evidence Working Group. *The Oxford 2011 Levels of Evidence.* Oxford Centre for Evidence-Based Medicine. https://www.cebm.ox.ac.uk/resources/levels-of-evidence/ocebm-levels-of-evidence
- **[GRADE]** GRADE Working Group. *Grading of Recommendations Assessment, Development and Evaluation.* https://www.gradeworkinggroup.org/
- **[DGE]** Deutsche Gesellschaft für Ernährung. *Referenzwerte für die Nährstoffzufuhr.* https://www.dge.de/wissenschaft/referenzwerte/

> Alle Links wurden zum Erstellungszeitpunkt (2026-07-09) auf Plausibilität geprüft; Regulatorik ist vor jeder Verwendung gegen die aktuell konsolidierte Fassung abzugleichen.

---

## 10. Glossar (Auswahl)

- **RCT** — Randomized Controlled Trial (randomisierte kontrollierte Studie).
- **Meta-Analyse** — statistische Zusammenfassung mehrerer Studien.
- **UL** — Tolerable Upper Intake Level (tolerierbare tägliche Höchstaufnahmemenge).
- **NEM** — Nahrungsergänzungsmittel.
- **Health Claim** — gesundheitsbezogene Angabe i. S. d. VO (EG) 1924/2006.
- **CELEX** — Identifikationsnummer eines EU-Rechtsakts in EUR-Lex.
- **CI** — Konfidenzintervall. **RR/OR/MD/SMD** — Effektmaße (relatives Risiko, Odds Ratio, Mittelwertdifferenz, standardisierte Mittelwertdifferenz).
