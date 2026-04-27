---
type: "research"
subtype: "standard"
title: "Výzkumná zpráva: Cognitive Mirror Framework"
date: "2026-01-08"
project: "life-skills-education"
status: "completed"
confidence: "0.XX"
sources_count: "0"
tags: []
related: []
created_by: "/research"
---
# Výzkumná zpráva: Cognitive Mirror Framework

**Datum:** 2026-01-08
**Projekt:** life-skills-education
**Téma:** AI-powered metakognice a samoregulované učení

---

## Executive Summary

Framework "Cognitive Mirror" (Kognitivní zrcadlo) představuje paradigmatický posun v návrhu vzdělávacího AI. Místo tradičního přístupu, kde AI vystupuje jako vševědoucí tutor předávající znalosti, Cognitive Mirror invertuje vztah - AI se stává "učitelným nováčkem", který zrcadlí kvalitu studentova vysvětlování. Tento přístup využívá protégé efekt a podporuje metakognici tím, že studenti musí aktivně konstruovat a vysvětlovat své znalosti, místo pasivního přijímání odpovědí.

Pro projekt vzdělávání meta-dovedností dětí 11-13 let představuje tento framework klíčovou příležitost: navrhnout AI nástroje, které posílí metakognitivní schopnosti namísto jejich oslabení.

---

## 1. Co je Cognitive Mirror Framework?

### 1.1 Definice

Cognitive Mirror je koncepční rámec pro návrh vzdělávacího AI, který rekonceptualizuje umělou inteligenci jako **"učitelného nováčka navrženého tak, aby zrcadlil kvalitu studentova vysvětlování"** (Tomisu, Ueda & Yamanaka, 2025).

### 1.2 Klíčová inovace

Framework "přeprogramovává bezpečnostní omezení AI jako didaktické mechanismy k záměrnému vytváření 'pedagogicky užitečného deficitu' AI". Jinými slovy - záměrně omezuje znalosti AI tak, aby student musel aktivně vysvětlovat a učit, namísto pasivního přijímání hotových odpovědí.

### 1.3 Teoretické základy

Framework stojí na třech pilířích vzdělávací teorie:

| Teorie | Klíčový princip | Aplikace v CM |
|--------|----------------|---------------|
| **Protégé efekt** | Studenti se učí lépe, když musí učit druhé | AI vystupuje jako učený žák, kterého student vyučuje |
| **Reflektivní praxe** (Schön) | Reflection-in-action a reflection-on-action | Čtyřkrokový cyklus vyvolává kontinuální reflexi |
| **Metakognice** | Sebemonitorování a sebekorekce | AI zrcadlí kvalitu myšlení studenta zpět k němu |

---

## 2. Klíčové principy a komponenty

### 2.1 Čtyřkrokový interakční cyklus

```
┌─────────────────────────────────────────────────────────────┐
│                    COGNITIVE MIRROR LOOP                     │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│   1. PRESENT ─────► 2. QUERY ─────► 3. REFLECT ─────► 4. REFINE
│       │                │                │                │  │
│       │                │                │                │  │
│   Student          AI pokládá       AI odpověď       Student│
│   vysvětluje       otázky pouze     indikuje         opravuje
│   koncept          na základě       kvalitu          mezery │
│   AI               session info     vysvětlení              │
│                                                             │
│                         ◄───────────────────────────────────┘
│                              (Opakuje se)                   │
└─────────────────────────────────────────────────────────────┘
```

**Detailní popis kroků:**

1. **Present (Prezentovat)**: Student vysvětluje koncept AI systému
2. **Query (Dotazovat)**: Systém pokládá otázky pouze na základě informací z aktuální session
3. **Reflect (Reflektovat)**: Kvalita AI odpovědi indikuje kvalitu studentova vysvětlení
4. **Refine (Zdokonalovat)**: Student identifikuje mezery a reviduje své vysvětlení

### 2.2 Čtyři režimy odpovědí (M0-M3)

| Režim | Název | Popis | Kdy se použije |
|-------|-------|-------|----------------|
| **M0** | Zmatené přeformulování | Záměrně nízkokompetenční zrcadlení | Nejasné/neúplné vysvětlení |
| **M1** | Objasňující sonda | Cílené otázky pro přesnější definice | Částečné porozumění |
| **M2** | Sokratovská mezera | Poukazuje na chybějící logické spojení | Dobré, ale neúplné vysvětlení |
| **M3** | Přesná reformulace | Korektní parafráze při kvalitním vysvětlení | Výborné vysvětlení |

### 2.3 Teaching Quality Index (TQI)

TQI je metrika hodnotící kvalitu vysvětlování, která dynamicky přepíná mezi režimy odpovědí. Systém se pohybuje od "zmateného zrcadlení" (M0) k "přesné reformulaci" (M3) v závislosti na kvalitě studentova vysvětlení.

### 2.4 Klíčové komponenty systému

1. **Educator-defined curriculum scope** - Učitelé definují rozsah kurikula
2. **Persona-driven RAG** - Vynucuje omezení "studentské persony" AI
3. **Knowledge-integrity checks** - Skenuje odpovědi na koncepty mimo rozsah

---

## 3. Rozdíl od tradičního AI tutoringu

### 3.1 Srovnání přístupů

| Aspekt | Tradiční AI Tutor | Cognitive Mirror |
|--------|-------------------|------------------|
| **Role AI** | Vševědoucí expert | Učitelný nováček |
| **Tok znalostí** | AI → Student | Student → AI |
| **Aktivita studenta** | Pasivní příjemce | Aktivní konstruktor |
| **Cíl interakce** | Správná odpověď | Kvalitní vysvětlení |
| **Metakognice** | Často potlačena | Aktivně podporována |
| **Kognitivní zátěž** | Offloading (odlehčení) | Engagement (zapojení) |

### 3.2 Problém kognitivního offloadingu

Výzkum ukazuje na **"kognitivní paradox AI ve vzdělávání"** (PMC, 2025):

> "Zatímco AI jistě usnadňuje učení, také snižuje příležitosti pro aktivní vybavování a řešení problémů, které jsou esenciální pro kognitivní vývoj."

**Klíčová zjištění z výzkumu:**

- Časté používání AI **negativně koreluje** s kritickým myšlením
- Studenti spoléhající na AI vykazují **snížené rozhodovací a analytické schopnosti**
- Prolongovaná expozice AI vede k **poklesu paměti a retence**
- Studenti přijímají informace od AI **pasivně bez kritického zkoumání**

### 3.3 Jak Cognitive Mirror řeší tyto problémy

```
Tradiční AI:    Student → Otázka → AI odpověď → Student přijme
                        (Cognitive OFFLOADING)

Cognitive Mirror: Student → Vysvětlení → AI zrcadlí → Student reflektuje → Zlepšení
                        (Cognitive ENGAGEMENT)
```

---

## 4. Design patterny pro AI posilující metakognici

### 4.1 Základní design principy

#### Princip 1: Nepřímé scaffolding

Místo přímých odpovědí používat:
- Nápovědy a vodítka
- Krok za krokem plány
- Sokratovské otázky
- Zpětné zrcadlení

#### Princip 2: Kompletní metakognitivní cykly

AI by mělo provádět studenty **celými cykly plánování-monitorování-evaluace**, nikoliv jen jednotlivými kroky.

```
┌────────────────────────────────────────────────────────────┐
│              KOMPLETNÍ METAKOGNITIVNÍ CYKLUS               │
├────────────────────────────────────────────────────────────┤
│                                                            │
│    PLÁNOVÁNÍ          MONITOROVÁNÍ          EVALUACE       │
│    ─────────          ───────────           ────────       │
│    • Co chci           • Jak mi to          • Dosáhl jsem  │
│      dosáhnout?          jde?                 cíle?        │
│    • Jaká strategie?   • Rozumím tomu?      • Co bych      │
│    • Co potřebuji      • Kde mám            udělal jinak?  │
│      vědět?              problém?           • Co jsem se   │
│                                               naučil?      │
│                                                            │
└────────────────────────────────────────────────────────────┘
```

#### Princip 3: Strukturované promptování

Namísto free-form vstupů používat:
- Dekompozici úkolů
- Řetězení promptů
- Výběr fází učení před dotazem

#### Princip 4: Adaptivní kontrola

"Sdílená a adaptivní kontrola" - instruktoři definují povolené rozsahy podpory, studenti vykonávají autonomii v rámci hranic.

### 4.2 Praktické design patterny

#### Pattern A: "Explain to Learn"

```
IMPLEMENTACE:
1. Student má za úkol vysvětlit koncept AI
2. AI simuluje "zmateného studenta" s cílenými mezerami
3. Kvalita AI porozumění = kvalita studentova vysvětlení
4. AI pokládá upřesňující otázky
5. Student iterativně zlepšuje své vysvětlení

PŘÍKLAD PROMPTU:
"Jsem tvůj student, který se teprve učí. Vysvětli mi [koncept].
Budu ti klást otázky, pokud něčemu nerozumím."
```

#### Pattern B: "Reflective Checkpoint"

```
IMPLEMENTACE:
1. Před každou AI odpovědí: "Co si myslíš, že by mohla být odpověď?"
2. Po AI interakci: "Co jsi se právě naučil?"
3. Periodicky: "Jak bys vysvětlil tento koncept vlastními slovy?"

PŘÍKLAD:
Student: "Jak funguje fotosyntéza?"
AI: "Než ti odpovím - co už o fotosyntéze víš? Zkus mi to shrnout."
```

#### Pattern C: "Metacognitive Scaffolding"

```
FÁZE PŘED UČENÍM:
- "Co je tvým cílem?"
- "Co už víš o tomto tématu?"
- "Jakou strategii použiješ?"

FÁZE BĚHEM UČENÍ:
- "Jak ti to jde?"
- "Rozumíš tomuto kroku?"
- "Co tě překvapilo?"

FÁZE PO UČENÍ:
- "Co jsi se naučil?"
- "Co bys udělal jinak?"
- "Kde můžeš toto použít?"
```

#### Pattern D: "Socratic Gap"

```
IMPLEMENTACE:
1. AI identifikuje logickou mezeru ve vysvětlení
2. Místo korekce pokládá otázku: "A co když...?"
3. Student musí sám doplnit chybějící logiku

PŘÍKLAD:
Student: "Rostliny potřebují vodu k růstu."
AI: "Ano, ale proč myslíš, že voda nestačí sama o sobě?
     Co ještě rostliny potřebují a proč?"
```

### 4.3 Anti-patterny (čemu se vyhnout)

| Anti-pattern | Proč je škodlivý | Alternativa |
|--------------|------------------|-------------|
| Přímé odpovědi | Podporuje pasivitu | Sokratovské otázky |
| Neomezený přístup k AI | Vede k závislosti | Strukturované sessions |
| AI jako zdroj pravdy | Potlačuje kritické myšlení | AI jako "učící se partner" |
| Chybí reflexe | Žádná metakognice | Povinné shrnutí "co jsem se naučil" |

---

## 5. Evidence efektivity

### 5.1 Primární studie - Cognitive Mirror

**Studie:** Ritsumeikan Moriyama Junior and Senior High School, červenec 2025
- **Vzorek:** 36 studentů 3. ročníku
- **Obsah:** Anglické relativní adverbia
- **Pozorování:** Studenti se přesunuli "od hledání odpovědí k budování vysvětlení" a stali se vědomými nejednoznačností ve svém porozumění

**Limitace:** Autoři explicitně uvádějí, že studie "postrádá randomizaci, kontrolní skupiny a systematické měření; proto nepodporuje kauzální tvrzení."

### 5.2 Podpůrné studie

#### Metakognitivní scaffolding s Teachable Agents (APLUS)

- **Vzorek:** 444 studentů 6.-8. ročníku (208 dokončilo studii)
- **Zjištění:** Přidání metakognitivního scaffoldingu **zesílilo efekt learning-by-teaching** více než baseline prostředí

#### Adaptivní vs. plánovaný scaffolding

- **Metodika:** Generativní AI agenti poskytující real-time, adaptivní a personalizovanou odpověď
- **Výsledky:** Adaptivní metakognitivní scaffolding (AMS) **významně zlepšil** výkon v computational thinking a podporoval komplexnější využití dovedností
- **Další efekty:** Podpořil rekurzivní metakognitivní chování a **snížil mentální námahu**

#### Strukturované promptování vs. cognitive offloading

- **Zjištění:** Strukturované strategie zapojení mohou **zmírnit negativní efekty** cognitive offloadingu
- **Klíč:** Trénovat účastníky používat AI jako "informační nástroj" spíše než "agent řešící úkoly"

#### ChatGPT vs. lidští tutoři (kritické myšlení)

- **ChatGPT výhody:** 24/7 dostupnost, neodsuzující interakce, snížení psychologických bariér
- **Lidští tutoři výhody:** Emocionální spojení, přizpůsobená zpětná vazba, hluboké dotazování
- **Závěr:** Optimální je **hybridní model** kombinující oba přístupy

### 5.3 Ochranné faktory proti cognitive offloadingu

Výzkum identifikoval faktory, které chrání před negativními efekty AI:

1. **Vyšší vzdělání** - funguje jako "ochranný buffer"
2. **Formální trénink kritického myšlení**
3. **Strukturované používání AI** s reflexivními praktikami
4. **Metakognitivní podpora** během používání AI

---

## 6. Aplikace pro děti 11-13 let

### 6.1 Vývojový kontext

Věk 11-13 let představuje **kritické období**:
- Významný osobní a sociální vývoj
- Zvýšená sebeuvědomělost (může bránit participaci)
- Kritická fáze pro vývoj metakognitivních dovedností
- Potřeba více strukturovaného vedení než u starších studentů

### 6.2 Specifické požadavky pro tuto věkovou skupinu

| Aspekt | Požadavek | Implementace |
|--------|-----------|--------------|
| **Struktura** | Více vedení než u starších | Jasné kroky, checkpointy |
| **Motivace** | Engagement bez kritiky | Gamifikace, pozitivní zpětná vazba |
| **Abstrakce** | Konkrétní příklady | Reálné situace ze života |
| **Sociální** | Peer learning | Skupinové aktivity |
| **Autonomie** | Postupné budování | Volby v rámci hranic |

### 6.3 Adaptované design principy pro 11-13 let

#### Princip 1: Strukturovaná autonomie

```
SPRÁVNĚ:
"Vyber si, jak chceš tento problém vyřešit:
 A) Nakreslit diagram
 B) Napsat seznam kroků
 C) Vysvětlit spolužákovi"

ŠPATNĚ:
"Co chceš dělat?" (příliš otevřené)
```

#### Princip 2: Viditelný pokrok

```
IMPLEMENTACE:
- Progress bar pro metakognitivní dovednosti
- Odznaky za "dobré otázky"
- Deník "co jsem se dnes naučil"
```

#### Princip 3: Peer teaching s AI podporou

```
FLOW:
1. Student A vysvětluje koncept AI (AI = "zmatený spolužák")
2. AI identifikuje mezery formou otázek
3. Student A vylepšuje vysvětlení
4. Student A poté vysvětluje reálnému spolužákovi
5. Spolužák poskytuje feedback
```

#### Princip 4: Scaffolded reflection

```
ŠABLONA PRO 11-13 LET:

PŘED AKTIVITOU:
"Co už vím o tomto tématu? _______________"
"Co chci zjistit? _______________"
"Jak to zkusím zjistit? _______________"

PO AKTIVITĚ:
"Co jsem se naučil: _______________"
"Co mě překvapilo: _______________"
"Co mi ještě není jasné: _______________"
"Kde to mohu použít: _______________"
```

### 6.4 Příklady aktivit

#### Aktivita 1: "Nauč AI robota"

**Cíl:** Rozvoj vysvětlovacích dovedností a metakognice

```
PRŮBĚH:
1. Student dostane úkol naučit AI robota [koncept]
2. Robot reaguje podle TQI (M0-M3)
3. Student musí vylepšovat své vysvětlení
4. Na konci: "Co jsi musel změnit, aby robot rozuměl?"
```

#### Aktivita 2: "Detektiv vlastního myšlení"

**Cíl:** Rozvoj sebemonitorování

```
PRŮBĚH:
1. Student řeší problém
2. AI periodicky ptá: "Jak ti to jde? Co děláš právě teď?"
3. Student vede "deník myšlení" v reálném čase
4. Na konci analýza: "Kdy ti to šlo nejlépe? Proč?"
```

#### Aktivita 3: "Před a po"

**Cíl:** Rozvoj self-assessment

```
PRŮBĚH:
1. PŘED: "Jak dobře rozumím tomuto tématu? (1-10)"
2. Učební aktivita s AI
3. PO: "Jak dobře rozumím nyní? (1-10)"
4. Diskuze: "Co se změnilo? Proč?"
```

---

## 7. Implementační úvahy a výzvy

### 7.1 Technické výzvy

| Výzva | Popis | Možné řešení |
|-------|-------|--------------|
| **Kalibrace "nevědění"** | Nastavit správnou úroveň AI "neznalosti" bez úniku skutečných znalostí | Striktní persona prompting, RAG s omezeným kontextem |
| **TQI validace** | Spolehlivě měřit kvalitu vysvětlení | Multi-dimenzionální hodnocení (struktura, přesnost, hloubka) |
| **Konzistence persony** | Udržet AI v roli "nováčka" | Systémové prompty, guardrails |
| **Škálovatelnost** | Personalizace pro každého studenta | Adaptivní algoritmy |

### 7.2 Pedagogické výzvy

| Výzva | Popis | Možné řešení |
|-------|-------|--------------|
| **Gaming TQI** | Studenti mohou "hackovat" systém místo skutečného učení | Variabilní hodnocení, lidský oversight |
| **Frustrace** | "Zmatená" AI může frustrovat | Postupná kalibrace obtížnosti |
| **Motivace** | Proč učit AI místo být učen? | Gamifikace, odznaky, peer recognition |
| **Transfer** | Přenesení metakognice do reálného života | Explicitní bridging aktivity |

### 7.3 Etické výzvy

| Výzva | Popis | Možné řešení |
|-------|-------|--------------|
| **Algoritmická férovost** | Riziko penalizace nestandardních stylů vysvětlování | Diverzifikované datasety, kulturní citlivost |
| **Privacy** | Data o metakognici studentů | Transparentní nakládání, minimální sběr |
| **Digitální propast** | Nerovný přístup k technologii | Offline verze, školní zařízení |
| **Závislost** | I na "dobrém" AI | Pravidelné AI-free sessions |

### 7.4 Implementační doporučení

#### Fáze 1: Pilotní testování (3 měsíce)

```
AKTIVITY:
1. Výběr 10-15 studentů pro pilotní skupinu
2. Testování 2-3 aktivit s Cognitive Mirror principy
3. Sběr kvalitativní zpětné vazby
4. Iterace designu

METRIKY:
- Engagement (čas strávený, dokončení)
- Kvalita reflexí (hloubka, specifičnost)
- Studentská spokojenost
```

#### Fáze 2: Rozšířené testování (6 měsíců)

```
AKTIVITY:
1. Rozšíření na 30-50 studentů
2. Implementace plného Cognitive Mirror cyklu
3. Pre/post hodnocení metakognitivních dovedností
4. Srovnání s kontrolní skupinou

METRIKY:
- MSLQ (Motivated Strategies for Learning Questionnaire)
- Transfer úkoly (metakognice v jiných kontextech)
- Akademický výkon
```

#### Fáze 3: Full implementace

```
AKTIVITY:
1. Integrace do celého kurikula
2. Trénink facilitátorů
3. Continuous improvement loop
```

### 7.5 Role dospělého facilitátora

Cognitive Mirror **nenahrazuje** lidského pedagoga, ale mění jeho roli:

| Tradiční role | Nová role |
|---------------|-----------|
| Přenos znalostí | Facilitace objevování |
| Hodnocení správnosti | Podpora reflexe |
| Kontrola | Mentoring |
| Odpovídání na otázky | Pokládání lepších otázek |

---

## 8. Shrnutí a doporučení pro projekt

### 8.1 Klíčová zjištění

1. **Cognitive Mirror** invertuje tradiční AI tutoring - student učí AI místo opačně
2. **Protégé efekt** s AI podporuje hlubší učení a metakognici
3. **Kognitivní offloading** je reálné riziko tradičního AI - CM ho adresuje
4. **Strukturované používání** AI s metakognitivní podporou je klíčové
5. **Věk 11-13** vyžaduje více struktury, ale je ideální pro budování metakognitivních návyků

### 8.2 Konkrétní doporučení pro projekt

#### DOPORUČENÍ 1: Adoptovat Cognitive Mirror principy

Implementovat základní design pattern "AI jako učitelný nováček" do vzdělávacích aktivit.

#### DOPORUČENÍ 2: Vytvořit strukturované metakognitivní šablony

Před/během/po šablony pro všechny aktivity s AI.

#### DOPORUČENÍ 3: Kombinovat AI s peer learning

AI jako příprava na peer teaching - student nejprve "vyzkouší" vysvětlení na AI, pak na spolužákovi.

#### DOPORUČENÍ 4: Implementovat reflektivní checkpointy

Povinné reflexe před a po každé AI interakci.

#### DOPORUČENÍ 5: Trénovat facilitátory

Připravit rodiče/učitele na novou roli "reflection moderators".

#### DOPORUČENÍ 6: Měřit metakognitivní dovednosti

Implementovat měření pomocí standardizovaných nástrojů (adaptovaný MSLQ).

#### DOPORUČENÍ 7: Pravidelné AI-free sessions

Zajistit, že některé aktivity jsou bez AI - prevence závislosti.

### 8.3 Další výzkum

- Longitudinální studie efektivity CM u dětí 11-13 let
- Kulturní adaptace pro české prostředí
- Optimální "dávkování" AI vs. human interakce
- Transfer metakognitivních dovedností do běžného života

---

## Zdroje

### Primární zdroj

1. Tomisu, H., Ueda, J., & Yamanaka, T. (2025). [The cognitive mirror: a framework for AI-powered metacognition and self-regulated learning](https://www.frontiersin.org/journals/education/articles/10.3389/feduc.2025.1697554/full). *Frontiers in Education*, 10, 1697554.

### Sekundární zdroje

2. PMC (2025). [The cognitive paradox of AI in education: between enhancement and erosion](https://pmc.ncbi.nlm.nih.gov/articles/PMC12036037/). *Frontiers in Psychology*.

3. Li et al. (2025). [Scaffolding Metacognition in Programming Education: Understanding Student–AI Interactions and Design Implications](https://arxiv.org/html/2511.04144v1). *arXiv*.

4. MDPI (2025). [Mapping the Scaffolding of Metacognition and Learning by AI Tools in STEM Classrooms](https://www.mdpi.com/2079-3200/13/11/148). *Journal of Intelligence*, 13(11), 148.

5. Springer (2019). [The Effect of Metacognitive Scaffolding for Learning by Teaching a Teachable Agent](https://link.springer.com/article/10.1007/s40593-019-00190-2). *International Journal of Artificial Intelligence in Education*.

6. ScienceDirect (2025). [Adaptive metacognitive prompting in young learners and the role of prior performance](https://www.sciencedirect.com/science/article/pii/S2212868925000200). *Learning and Individual Differences*.

7. Nature (2025). [A qualitative systematic review on AI empowered self-regulated learning in higher education](https://www.nature.com/articles/s41539-025-00319-0). *npj Science of Learning*.

8. MDPI (2025). [From Offloading to Engagement: An Experimental Study on Structured Prompting and Critical Reasoning with Generative AI](https://www.mdpi.com/2306-5729/10/11/172). *Data*, 10(11), 172.

9. Frontiers in Education (2025). [Socratic wisdom in the age of AI: a comparative study of ChatGPT and human tutors](https://www.frontiersin.org/journals/education/articles/10.3389/feduc.2025.1528603/full). *Frontiers in Education*, 10.

10. arXiv (2025). [Chrysalis: A Unified System for Comparing Active Teaching and Passive Learning with AI Agents in Education](https://arxiv.org/html/2510.05271).

11. MDPI (2024). [Integrating Youth Perspectives into the Design of AI-Supported Collaborative Learning Environments](https://www.mdpi.com/2227-7102/14/11/1197). *Education Sciences*, 14(11), 1197.

12. ACM (2024). [Teach AI How to Code: Using Large Language Models as Teachable Agents for Programming Education](https://dl.acm.org/doi/10.1145/3613904.3642349). *CHI Conference*.

13. ScienceDirect (2025). [Adaptive vs. planned metacognitive scaffolding for computational thinking](https://www.sciencedirect.com/science/article/pii/S0360131525002416). *Computers & Education*.

14. BJET (2025). [Enhancing self-regulated learning and learning experience in generative AI environments: The critical role of metacognitive support](https://bera-journals.onlinelibrary.wiley.com/doi/10.1111/bjet.13599). *British Journal of Educational Technology*.

15. Nature Scientific Reports (2025). [Generative AI tool use enhances academic achievement through shared metacognition and cognitive offloading](https://www.nature.com/articles/s41598-025-01676-x).

---

*Výzkumná zpráva vytvořena pro projekt life-skills-education*
*Datum: 2026-01-08*
*Verze: 1.0*
