# Schweigepflicht-Gateway: Arbeitsschema / working scheme

**Stand: 10.10.2026 · Fassung 0.2 – nicht endgültig.** Dieses Dokument beschreibt das Schema, nach dem ich vertrauliche Unterlagen mit großen Sprachmodellen bearbeite, ohne die Unterlagen selbst herauszugeben. Der Programmcode folgt in eigenen Veröffentlichungen.

*Status: 10 Oct 2026 · version 0.2 – not final. This document describes the scheme by which I process confidential documents with large language models without handing over the documents themselves. The code will follow in separate publications. English and Russian versions below. / Русская версия — в конце.*

Autor: Sergei Sevriukov, LeckerMath, Dortmund · https://leckermath.de · Text: CC BY 4.0

Zum Hintergrund: 25 Jahre Bank, interne Kontrolle und Prüfung; Schulungen und Zertifizierung im Qualitätsmanagement (ISO 9001, internes Audit). Der Beitrag dieses Schemas liegt in der Organisation des Ablaufs, nicht in besonderem Programmcode.

---

## 1. Ausgangspunkt

Große Sprachmodelle werden von großen Teams gebaut; mit ihnen in Konkurrenz zu treten, ist für eine kleine Kanzlei oder eine einzelne Buchhalterin sinnlos – und unnötig. Große Prüfungs- und Beratungsgesellschaften haben eigene Lösungen. Die Frage ist eine andere: Was tun die gewöhnlichen Fachleute, die auf diese Modelle angewiesen sind, obwohl die Modelle häufig Falsches behaupten und vertrauliche Unterlagen nicht sehen dürfen?

Die Antwort dieses Schemas: **Man vertraut dem eigenen Textbestand und prüft daran alles, was die großen Modelle sagen** – durch das Prisma der eigenen Ausbildung, des eigenen Wissens und der eigenen Praxis. Dazu werden drei Dinge, die jedes für sich bekannt sind, zu einem Ablauf verbunden:

1. eine **lokale Schicht**, die Unterlagen liest, die Beteiligten erkennt und vor der Weitergabe durch Rollenmarken ersetzt;
2. **große externe Sprachmodelle**, die nur dieses Blatt sehen und die fachliche Arbeit leisten – austauschbar, sobald ein besseres erscheint;
3. einen **eigenen, geprüften Bestand amtlicher Texte**, an dem jede Antwort per Programm kontrolliert wird – mit anschließender Rückführung der Namen, wieder lokal.

Die Bausteine sind austauschbar: Erscheint ein besseres Modell, wird es angeschlossen; Schicht und Textbestand bleiben.

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

## 3a. Das Verzeichnis der Beteiligten

Wer je ein Theaterstück gelesen hat, kennt die Lösung: Vor dem Text stehen die handelnden Personen – wer wer ist und in welchem Verhältnis zu den anderen. Dieses Verzeichnis gibt beim Lesen die Ordnung vor. Die Idee ist so alt wie das Drama und stammt nicht von mir.

Übertragen auf Unterlagen: Die prüfende Person benennt die wesentlichen Beteiligten und ihre Rollen; jede erhält eine Marke, die in allen Unterlagen gleich bleibt. Dem Modell ist gleichgültig, ob dort ein Name oder »Beteiligter 1, Berater der Gesellschaft« steht – der Sachverhalt bleibt lesbar, die Person bleibt verborgen. Ohne ein solches Verzeichnis zerfällt ein anonymisierter Schriftwechsel in Sätze ohne Zusammenhang.

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
- Offengelegt werden hier die Ergebnisse **eines** echten Falls. Mehr lässt die Vertraulichkeit nicht zu: Echte Fälle können nur mit Einwilligung der Betroffenen ausgewertet und nie im Wortlaut gezeigt werden. Jeder neue Fall schärft die Regeln; eine belastbare Statistik über viele Fälle und eine Prüfung durch Dritte sind genau das, wofür eine Förderung gebraucht wird.
- Rechtlich ist das Ersetzen durch Rollenmarken eine **Pseudonymisierung**: Der Schlüssel bleibt lokal, die Zuordnung ist für die Kanzlei wiederherstellbar. Ob und unter welchen Bedingungen das berufsrechtlich genügt, ist nicht Gegenstand dieses Dokuments.
- Keine Rechts- oder Steuerauskunft. Keine externe Bewertung.

## 6. Wie es dazu kam (mit Datum belegbar)

| Zeit | Schritt | Beleg |
|---|---|---|
| 2024 | Beginn der Arbeit an KI für vertrauliche Finanz- und Steuerdaten; Hardware für eigene Rechnungen | Mitteilung an das Finanzamt vom 24.09.2024; öffentlicher Beitrag vom 17.05.2024 |
| 02.2025 | Trennermethode nach Zhuravlev auf Grafikkarten | öffentlicher Beitrag vom 24.02.2025 |
| 03–09.2025 | Arbeit mit großen Modellen; unzuverlässige Fundstellen; erste Prototypen einer geprüften Textdatenbank | öffentlicher Beitrag vom 02.09.2025 |
| 08–10.2026 | heutige Programmbasis; Forschungsprotokoll mit Versuchen, auch misslungenen | veröffentlichter Korpus, 09.10.2026 |
| 10.10.2026 | dieses Schema, Fassung 0.1 und 0.2 | dieses Dokument |

## 7. Stand und Ausblick

Als Prototyp ist das Vorhaben abgeschlossen: Der Ablauf ist von Anfang bis Ende durchlaufen. Offen sind die Anonymisierung ohne Reste an fremden Fällen, die Zeitmessung mit unabhängigen Prüfpersonen, das Zusammenführen der Antworten mehrerer Modelle, ein Austauschformat für Rückmeldungen aus der Praxis und Regelwerke für weitere Berufe mit Schweigepflicht.

Für die Fortführung gibt es zwei Wege, die sich nicht ausschließen: ein offenes Werkzeug, das Kanzleien selbst betreiben, oder ein fertiges Produkt eines Softwarehauses auf dieser Grundlage. Das Schema ist dafür ausgelegt, dass ein Softwarehaus mittlerer Größe es umsetzen kann.

---

# English

## 1. Starting point

Large language models are built by large teams; for a small firm or a single accountant, competing with them is pointless — and unnecessary. Large audit and advisory companies have their own solutions. The question is a different one: what are ordinary professionals to do who depend on these models although the models often state things that are false and must not see confidential documents?

The answer of this scheme: **trust your own body of texts and check everything the large models say against it** — through the lens of your own training, knowledge and practice. To that end, three things, each known on its own, are combined into one workflow:

1. a **local layer** that reads the documents, recognises the parties and replaces them with role markers before anything leaves the machine;
2. **large external language models** that see only this sheet and do the professional work — interchangeable as soon as a better one appears;
3. an **own, verified body of official texts** against which every answer is checked by code — followed by restoring the names, again locally.

## 2. Three positions, one direction

The **examiner** states in free words what the matter is about and decides at the end. The **local secretary** is the only position that sees originals and runs entirely on the examiner's own machine. The **external model** receives facts — amounts, deadlines, provisions, sequences — but no persons.

## 3. Workflow

**A. Collecting the facts.** Free-form introduction by the examiner (typed or spoken) → the case folder is handed over as it is and read locally → acceptance protocol: what could be read, what could not, and why; unreadable material does not enter the sheet → the secretary proposes the persons and organisations found, the examiner names the essential ones and their roles, and a counter-check shows who acts in the correspondence without having been named → exchange sheet: introduction, list of parties (marker, kind, role, affiliation), a table of who writes to whom, the documents with role markers → multi-stage check before release; release only by the examiner's code → the external model structures the case and asks questions in role markers; the examiner sees them with real names and answers freely, until the examiner says "enough".

**B. Working on the proposal.** The model presents variants — each with provision, conditions, calculation, deadlines and required documents. The examiner comments; the secretary passes the comments on in role markers.

**C. Result.** The secretary restores the names and presents the result and the open questions separately.

**Rule for content:** all variants are presented; none is chosen, and persons are not judged. A human makes the choice.

## 3a. The cast of characters

Anyone who has read a play knows the solution: before the text comes the list of characters — who is who, and how they relate to one another. That list sets the order for reading. The idea is as old as drama and is not mine.

Applied to documents: the examiner names the essential parties and their roles; each gets a marker that stays the same across all documents. To the model it makes no difference whether a name stands there or "party 1, adviser to the company" — the facts remain readable, the person remains hidden. Without such a list, anonymised correspondence falls apart into sentences without connection.

## 4. Checking the answer

What the external model delivers is not believed but checked — by code, against the own body of texts: does the cited provision, paragraph and number exist; does the citation come from the version in force in the year in question; amounts, interest, surcharges and deadlines are recalculated, not copied; with several models, the answers are laid side by side: agreement, majority, deviation.

The open part of this body of texts is published: https://huggingface.co/datasets/sevriukov/german-tax-law-corpus

## 5. What has been measured — and what has not

On invented, independently written letters the share of details let through fell from 28.7 % to 6.0 % to 2.1 %. This does not carry over to real documents without more: after human release, remnants were repeatedly found, which led to a second, list-independent check and a third stage before release. With a list of parties given by the examiner, 12 of 15 facts in one real case could be attributed to the right organisation; without the list, none. Disclosed here are the results of **one** real case. Confidentiality allows no more: real cases can be evaluated only with the consent of those concerned and can never be shown verbatim. Every new case sharpens the rules; sound statistics over many cases and review by third parties are exactly what funding is needed for. Legally, replacing names with role markers is **pseudonymisation**: the key stays local and the mapping can be restored by the firm; whether and under which conditions this satisfies professional secrecy rules is outside the scope of this document. Not legal or tax advice. No external evaluation.

## 6. How it came about

Work on AI for confidential financial and tax data since 2024 (message to the tax office of 24 Sep 2024; public post of 17 May 2024); Zhuravlev's separator method on GPUs in February 2025 (public post of 24 Feb 2025); work with large models, unreliable citations and first prototypes of a verified text database between March and September 2025 (public post of 2 Sep 2025); today's code base since August 2026; the open corpus published on 9 Oct 2026; this scheme, version 0.1 and 0.2, on 10 Oct 2026.

## 7. Status and outlook

As a prototype the project is complete: the workflow has been run from beginning to end. For continuation there are two routes that do not exclude each other: an open tool that firms run themselves, or a finished product by a software house on this basis. The scheme is laid out so that a software house of medium size can implement it.

---

# По-русски

## 1. С чего всё началось

Большие языковые модели делают большие команды; состязаться с ними маленькой канцелярии или отдельному бухгалтеру бессмысленно — и не нужно. У крупных аудиторских и консультационных компаний есть свои решения. Вопрос в другом: что делать обычным специалистам, которые от этих моделей зависят, хотя модели часто утверждают неверное, а конфиденциальные бумаги им показывать нельзя?

Ответ этой схемы: **верить собственной базе текстов и проверять по ней всё, что говорят большие модели** — через призму своего образования, знаний и практики. Для этого три вещи, каждая из которых известна сама по себе, соединены в один ход работы:

1. **локальный слой**, который читает бумаги, находит участников и перед передачей заменяет их ролевыми метками;
2. **большие внешние модели**, которые видят только этот лист и делают профессиональную работу — их можно менять, как только появится лучшая;
3. **собственная выверенная база официальных текстов**, по которой каждый ответ проверяется программой, — после чего имена возвращаются, снова локально.

Части заменяемы: вышла модель лучше — подключили её; слой и база остаются.

## 2. Три звена, одно направление

```
проверяющий  ⇄  локальный секретарь  →  внешняя модель (одна или несколько)
свободный текст,   видит подлинники;         видит только обменный лист;
несколько минут    читает, упорядочивает,    раскладывает дело, проверяет,
                   заменяет имена метками,   задаёт вопросы метками,
                   возвращает имена          называет варианты
                          │
                          ▼
             выверенная база текстов (локально)
             проверка ответа программой
```

- **Проверяющий** своими словами говорит, о чём дело, и в конце решает сам. Форм он не заполняет.
- **Локальный секретарь** — единственное звено, которое видит подлинники. Он работает целиком на своём компьютере.
- **Внешняя модель** получает факты — суммы, сроки, нормы, ход событий, — но не людей.

## 3. Ход работы

**А. Сбор фактуры**

1. Вводная проверяющего: ситуация, проблема, цель, задача — текстом или голосом.
2. Папка дела отдаётся как есть: сканы, фотографии, PDF, выгрузки переписки, голосовые, заметки. Всё читается локально.
3. Приёмка: что прочитано, что нет и почему — протоколом. Нечитаемое в лист не идёт.
4. Секретарь предлагает найденных людей и организации; проверяющий называет главных и их роли. Встречная проверка программы показывает, кто действует в переписке, но назван не был.
5. Обменный лист: вводная, перечень действующих лиц (метка, вид, роль, к кому относится), таблица «кто кому пишет», бумаги с ролевыми метками.
6. Контроль перед передачей в несколько ступеней; выпуск — только по коду проверяющего.
7. Внешняя модель раскладывает дело и задаёт вопросы метками; проверяющий видит их с настоящими именами и отвечает свободно. Так по кругу, пока он не скажет «достаточно».

**Б. Работа над предложенным**

Модель предлагает варианты — каждый с нормой, условиями, расчётом, сроками и нужными документами. Проверяющий комментирует; секретарь передаёт комментарии метками.

**В. Итог**

Секретарь возвращает имена и отдельно показывает результат и открытые вопросы.

**Правило содержания:** показываются все варианты; ни один не выбирается, и людей не оценивают. Выбор делает человек.

## 3а. Перечень действующих лиц

Кто читал хоть одну пьесу, знает решение: перед текстом стоят действующие лица — кто есть кто и кем приходится остальным. Этот список задаёт порядок чтения. Идея стара как драма и придумана не мной.

В применении к бумагам: проверяющий называет главных участников и их роли; каждый получает метку, одну и ту же во всех документах. Модели всё равно, стоит там фамилия или «участник 1, консультант общества», — фактура читается, человек остаётся скрытым. Без такого перечня обезличенная переписка рассыпается на фразы без связи.

## 4. Проверка ответа

Тому, что отдаёт внешняя модель, не верят, а проверяют — программой, по своей базе:
- есть ли названная норма, абзац, номер;
- из той ли редакции взята ссылка, которая действовала в нужном году;
- суммы, проценты, надбавки и сроки пересчитываются, а не переписываются;
- если моделей несколько, ответы кладутся рядом: согласие, большинство, расхождение.

Открытая часть этой базы опубликована: https://huggingface.co/datasets/sevriukov/german-tax-law-corpus

## 5. Что измерено — и что нет

- На придуманных письмах, написанных независимо, доля пропущенных сведений снизилась с 28,7 % до 6,0 % и до 2,1 %.
- На настоящих бумагах это само собой не повторяется: после одобрения человеком остатки находились снова. Отсюда второй, не зависящий от списков контроль и третья ступень перед передачей.
- С перечнем действующих лиц, заданным проверяющим, на одном настоящем деле 12 фактов из 15 удалось отнести к нужной организации; без перечня — ни одного.
- Здесь раскрыты результаты **одного** настоящего дела. Большего не позволяет конфиденциальность: настоящие дела можно разбирать только с согласия тех, кого они касаются, и нельзя показывать дословно. Каждое новое дело шлифует правила; надёжная статистика по многим делам и проверка со стороны — именно то, на что нужно финансирование.
- С точки зрения права замена имён метками — это **псевдонимизация**: ключ остаётся у себя, соответствие восстановимо. Достаточно ли этого по правилам профессиональной тайны и при каких условиях — не предмет этого документа.
- Не правовая и не налоговая консультация. Внешней оценки не было.

## 6. Как к этому пришли (подтверждается датами)

| Когда | Шаг | Чем подтверждено |
|---|---|---|
| 2024 | начало работы над ИИ для конфиденциальных финансовых и налоговых данных; оборудование для собственных расчётов | сообщение в налоговую от 24.09.2024; публикация от 17.05.2024 |
| 02.2025 | метод Журавлёва на видеокартах | публикация от 24.02.2025 |
| 03–09.2025 | работа с большими моделями; ненадёжные ссылки; первые прототипы выверенной базы | публикация от 02.09.2025 |
| 08–10.2026 | нынешние программы; журнал опытов, включая неудачные | опубликованный корпус, 09.10.2026 |
| 10.10.2026 | эта схема, версии 0.1 и 0.2 | этот документ |

## 7. Состояние и что дальше

Как прототип проект завершён: ход работы пройден от начала до конца. Открыто: обезличивание без остатков на чужих делах; замеры времени с независимыми проверяющими; сведение ответов нескольких моделей; формат обмена для обратной связи из практики; наборы правил для других профессий с обязанностью хранить тайну.

Продолжать можно двумя путями, они не исключают друг друга: открытое средство, которое канцелярии ставят у себя сами, или готовый продукт софтверной компании на этой основе. Схема задумана так, чтобы её могла воплотить софтверная компания средней величины.
