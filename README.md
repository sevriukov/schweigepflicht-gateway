# Schweigepflicht-Gateway: Arbeitsschema / working scheme

**Stand: 10.10.2026 · Fassung 0.1 – nicht endgültig.** Dieses Dokument beschreibt das Schema, nach dem ich vertrauliche Unterlagen mit großen Sprachmodellen bearbeite, ohne die Unterlagen selbst herauszugeben. Der Programmcode folgt in eigenen Veröffentlichungen.

*Status: 10 Oct 2026 · version 0.1 – not final. This document describes the scheme by which I process confidential documents with large language models without handing over the documents themselves. The code will follow in separate publications. English version below.*

Autor: Sergei Sevriukov, LeckerMath, Dortmund · https://leckermath.de · Text: CC BY 4.0

---

## 1. Ausgangspunkt

Wer vertrauliche Zahlen und Schreiben prüft, steht vor einer schlechten Wahl: auf leistungsfähige Sprachmodelle verzichten oder Unterlagen an einen zentralen Anbieter geben. Modelle, die auf eigener Hardware laufen, antworten bei schwierigen fachlichen Fragen deutlich schwächer als die großen; dieser Abstand lässt sich von einem Einzelnen nicht aufholen. Große Modelle wiederum nennen Fundstellen und Regelungen, die es nicht gibt.

Das Schema verbindet deshalb drei Dinge, die jedes für sich bekannt sind, zu einem Ablauf:

1. eine **lokale Schicht**, die Unterlagen liest, die Beteiligten erkennt und vor der Weitergabe durch Rollenmarken ersetzt;
2. **große externe Sprachmodelle**, die nur dieses Blatt sehen und die fachliche Arbeit leisten;
3. einen **eigenen, geprüften Bestand amtlicher Texte**, an dem jede Antwort per Programm kontrolliert wird – mit anschließender Rückführung der Namen, wieder lokal.

## 2. Drei Stellen, eine Richtung

```
prüfende Person  ⇄  lokaler Sekretär  →  externes Modell (eines oder mehrere)
freier Text,          sieht die Originale;       sieht nur das Austauschblatt;
wenige Minuten        liest, ordnet, ersetzt     gliedert, prüft, stellt Rückfragen
                      Namen durch Rollenmarken,  in Rollenmarken, nennt Varianten
                      führt Namen zurück
                              │
                              ▼
                 geprüfter Textbestand (lokal)
                 Kontrolle der Antwort per Programm
```

- Die **prüfende Person** gibt in freien Worten vor, worum es geht, und entscheidet am Ende. Sie füllt keine Formulare aus.
- Der **lokale Sekretär** ist die einzige Stelle, die Originale sieht. Er arbeitet vollständig auf dem eigenen Rechner.
- Das **externe Modell** erhält Tatsachen – Beträge, Fristen, Normen, Abläufe –, aber keine Personen.

## 3. Ablauf

**A. Sachverhalt sammeln**

1. Einleitung der prüfenden Person: Lage, Problem, Ziel, Aufgabe – getippt oder gesprochen.
2. Der Ordner wird unverändert übergeben: Scans, Fotos, PDF, Chat-Auszüge, Sprachnachrichten, Notizen. Alles wird lokal gelesen.
3. Annahme: Was lesbar war, was nicht, und warum – als Protokoll. Unlesbares geht nicht ins Blatt.
4. Der Sekretär schlägt die gefundenen Personen und Organisationen vor; die prüfende Person bestimmt die wesentlichen und ihre Rollen. Eine Gegenprobe des Programms zeigt, wer im Schriftverkehr handelt, aber nicht benannt wurde.
5. Austauschblatt: Einleitung, Verzeichnis der Beteiligten (Marke, Art, Rolle, Zugehörigkeit), Tabelle »wer schreibt wem«, die Unterlagen mit Rollenmarken.
6. Kontrolle vor der Weitergabe in mehreren Stufen; Freigabe nur durch einen Code der prüfenden Person.
7. Das externe Modell gliedert den Fall und stellt Rückfragen in Rollenmarken; die prüfende Person sieht sie mit Klarnamen und antwortet frei. Das wiederholt sich, bis sie »genug« sagt.

**B. Arbeit am Vorschlag**

Das Modell legt Varianten vor – jede mit Norm, Voraussetzungen, Rechenweg, Fristen und nötigen Unterlagen. Die prüfende Person kommentiert; der Sekretär gibt die Kommentare in Rollenmarken zurück.

**C. Ergebnis**

Der Sekretär setzt die Namen wieder ein und stellt das Ergebnis und die offenen Fragen getrennt dar.

**Regel für den Inhalt:** Es werden alle Varianten dargestellt; keine wird ausgewählt, und Personen werden nicht bewertet. Die Auswahl trifft ein Mensch.

## 4. Kontrolle der Antwort

Was das externe Modell liefert, wird nicht geglaubt, sondern geprüft – per Programm, am eigenen Textbestand:
- Gibt es die genannte Norm, den Absatz, die Nummer?
- Stammt die Fundstelle aus der Fassung, die im fraglichen Jahr galt?
- Beträge, Zinsen, Zuschläge und Fristen werden neu berechnet, nicht übernommen.
- Bei mehreren Modellen werden die Antworten nebeneinandergelegt: Übereinstimmung, Mehrheit, Abweichung.

Der offene Teil dieses Textbestands ist veröffentlicht: https://huggingface.co/datasets/sevriukov/german-tax-law-corpus

## 5. Was gemessen ist – und was nicht

- An erfundenen, unabhängig erstellten Schreiben sank der Anteil durchgelassener Angaben von 28,7 % über 6,0 % auf 2,1 %.
- An echten Unterlagen überträgt sich das nicht ohne Weiteres: Nach menschlicher Freigabe fanden sich wiederholt noch Reste. Daraus entstanden eine zweite, listenunabhängige Kontrolle und eine dritte Stufe vor der Weitergabe.
- Mit einem von der prüfenden Person vorgegebenen Verzeichnis der Beteiligten ließen sich an einem echten Fall 12 von 15 Tatsachen der richtigen Organisation zuordnen; ohne Verzeichnis keine.
- Erprobt an **einem** echten Fall. Eine Wiederholung an weiteren Fällen und eine Prüfung durch Dritte stehen aus.
- Rechtlich ist das Ersetzen durch Rollenmarken eine **Pseudonymisierung**: Der Schlüssel bleibt lokal, die Zuordnung ist für die Kanzlei wiederherstellbar. Ob und unter welchen Bedingungen das berufsrechtlich genügt, ist nicht Gegenstand dieses Dokuments.
- Keine Rechts- oder Steuerauskunft. Keine externe Bewertung.

## 6. Wie es dazu kam (mit Datum belegbar)

| Zeit | Schritt | Beleg |
|---|---|---|
| 2024 | Beginn der Arbeit an KI für vertrauliche Finanz- und Steuerdaten; Hardware für eigene Rechnungen | Mitteilung an das Finanzamt vom 24.09.2024; öffentlicher Beitrag vom 17.05.2024 |
| 02.2025 | Trennermethode nach Zhuravlev auf Grafikkarten | öffentlicher Beitrag vom 24.02.2025 |
| 03–09.2025 | Arbeit mit großen Modellen; unzuverlässige Fundstellen; erste Prototypen einer geprüften Textdatenbank | öffentlicher Beitrag vom 02.09.2025 |
| 08–10.2026 | heutige Programmbasis; Forschungsprotokoll mit Versuchen, auch misslungenen | veröffentlichter Korpus, 09.10.2026 |
| 10.10.2026 | dieses Schema, Fassung 0.1 | dieses Dokument |

## 7. Offen

Anonymisierung ohne Reste an fremden Fällen; Zeitmessung mit unabhängigen Prüfpersonen; Zusammenführen der Antworten mehrerer Modelle; Regelwerke für weitere Berufe mit Schweigepflicht.

---

# English

## 1. Starting point

Anyone who examines confidential figures and letters faces a poor choice: do without capable language models, or hand documents to a central provider. Models that run on one's own hardware answer hard professional questions markedly worse than the large ones, and a single person cannot close that gap. Large models, in turn, cite provisions that do not exist.

The scheme therefore combines three things, each known on its own, into one workflow:

1. a **local layer** that reads the documents, recognises the parties and replaces them with role markers before anything leaves the machine;
2. **large external language models** that see only this sheet and do the professional work;
3. an **own, verified body of official texts** against which every answer is checked by code — followed by restoring the names, again locally.

## 2. Three positions, one direction

The **examiner** states in free words what the matter is about and decides at the end. The **local secretary** is the only position that sees originals and runs entirely on the examiner's own machine. The **external model** receives facts — amounts, deadlines, provisions, sequences — but no persons.

## 3. Workflow

**A. Collecting the facts.** Free-form introduction by the examiner (typed or spoken) → the case folder is handed over as it is and read locally → acceptance protocol: what could be read, what could not, and why; unreadable material does not enter the sheet → the secretary proposes the persons and organisations found, the examiner names the essential ones and their roles, and a counter-check shows who acts in the correspondence without having been named → exchange sheet: introduction, list of parties (marker, kind, role, affiliation), a table of who writes to whom, the documents with role markers → multi-stage check before release; release only by the examiner's code → the external model structures the case and asks questions in role markers; the examiner sees them with real names and answers freely, until the examiner says "enough".

**B. Working on the proposal.** The model presents variants — each with provision, conditions, calculation, deadlines and required documents. The examiner comments; the secretary passes the comments on in role markers.

**C. Result.** The secretary restores the names and presents the result and the open questions separately.

**Rule for content:** all variants are presented; none is chosen, and persons are not judged. A human makes the choice.

## 4. Checking the answer

What the external model delivers is not believed but checked — by code, against the own body of texts: does the cited provision, paragraph and number exist; does the citation come from the version in force in the year in question; amounts, interest, surcharges and deadlines are recalculated, not copied; with several models, the answers are laid side by side: agreement, majority, deviation.

The open part of this body of texts is published: https://huggingface.co/datasets/sevriukov/german-tax-law-corpus

## 5. What has been measured — and what has not

On invented, independently written letters the share of details let through fell from 28.7 % to 6.0 % to 2.1 %. This does not carry over to real documents without more: after human release, remnants were repeatedly found, which led to a second, list-independent check and a third stage before release. With a list of parties given by the examiner, 12 of 15 facts in one real case could be attributed to the right organisation; without the list, none. Tested on **one** real case; repetition on further cases and review by third parties are outstanding. Legally, replacing names with role markers is **pseudonymisation**: the key stays local and the mapping can be restored by the firm; whether and under which conditions this satisfies professional secrecy rules is outside the scope of this document. Not legal or tax advice. No external evaluation.

## 6. How it came about

Work on AI for confidential financial and tax data since 2024 (message to the tax office of 24 Sep 2024; public post of 17 May 2024); Zhuravlev's separator method on GPUs in February 2025 (public post of 24 Feb 2025); work with large models, unreliable citations and first prototypes of a verified text database between March and September 2025 (public post of 2 Sep 2025); today's code base since August 2026; the open corpus published on 9 Oct 2026; this scheme, version 0.1, on 10 Oct 2026.
