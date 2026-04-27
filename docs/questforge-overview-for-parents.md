---
title: "QuestForge — Vzdělávací hra pro děti"
author: "Zdeněk Macháček"
date: "2026-03-25"
---

# QuestForge — Vzdělávací hra pro děti

> Quest-Based Learning systém pro domácí vzdělávání dětí 11–13 let

---

## Co je QuestForge

QuestForge je vzdělávací systém postavený na principu **quest-based learningu** — děti se učí tím, že plní mise v příběhovém světě, ne tím, že sedí nad učebnicí.

**Příběhový rámec:** Kdesi v prostoru mezi světy existuje stanice **Nexus** — pradávná meziplanetární základna s vlastní inteligencí zvanou **Orákulum**. Orákulum hledá schopné operátory a vysílá je na mise do vzdálených světů, které potřebují pomoc.

Děti jsou ti operátoři. Každá mise je ve skutečnosti vzdělávací aktivita — ale děti to tak nevnímají. Vidí příběh, hádanky, výzvy.

**Klíčový princip:** Každá mise skrytě kombinuje 2–4 vzdělávací moduly. Dítě neví, že „teď dělá finanční gramotnost" — ví, že musí spočítat zásoby pro expedici na planetu Kepler-7.

---

## Pedagogické principy

### Cognitive Mirror

AI (v roli Orákula) **nikdy nedává přímé odpovědi**. Místo toho klade sokratovské otázky, které vedou dítě k vlastnímu objevu. Když se dítě zeptá „Jaká je správná odpověď?", Orákulum odpoví: „Co myslíš ty? A proč?"

Toto je záměrná volba — výzkumy ukazují, že odpovědi, ke kterým dítě dojde samo, si pamatuje výrazně lépe než ty, které mu někdo řekne.

### Kurikulum na pozadí

Děti nevidí strukturu kurikula. Nevidí „Modul 3: Informační gramotnost, Aktivita 2". Vidí: „Na planetě Kepler-7 jsme našli protichůdné záznamy v databázi stanice — musíme zjistit, které informace jsou spolehlivé."

Za tímto příběhem stojí propracované kurikulum s 8 metadovednostmi.

### 8 metadovedností

| Modul | Co se děti učí | Příklad ve hře |
|-------|---------------|----------------|
| **Metakognice** | Přemýšlet o vlastním myšlení | „Jak jsi přišel/a na toto řešení?" |
| **Kritické myšlení** | Analyzovat argumenty, rozlišovat fakt od názoru | Vyhodnocení protichůdných záznamů |
| **Informační gramotnost** | Ověřování zdrojů, SIFT metoda | Fact-checking staničních logů |
| **Finanční gramotnost** | Rozpočty, rozhodování o zdrojích | Správa zásob pro expedici |
| **Digitální gramotnost** | Kybernetická bezpečnost, šifry | Dešifrování zpráv, hesla |
| **Emoční inteligence** | Empatie, seberegulace | Komunikace s NPC na planetách |
| **Komunikace a spolupráce** | Naslouchání, argumentace, týmová práce | Společné řešení, prezentace zjištění |
| **Adaptabilita a rezilience** | Zvládání neznámého, improvizace | Nečekané komplikace během misí |

### Další principy

- **Mix digitálních a fyzických aktivit** — šifry na papíře, fotografování přírody, experimenty s mikroskopem, programování micro:bit, práce s dalekohledem.
- **Kooperativní questy** — dva operátoři spolupracují. Spolupráce = vyšší XP.
- **Bloom's Taxonomy** — aktivity pokrývají všechny úrovně od porozumění (Understand) po tvorbu (Create).

---

## Jak session vypadá

### Příprava (rodič, ~15 min)

Rodič použije příkaz `/prep`, který:

1. Vybere vhodné aktivity z kurikula (na základě aktuálního levelu dětí)
2. Zabalí je do narativu aktuální planety
3. Vygeneruje hádanky, šifry, tiskové materiály
4. Vytvoří facilitátorský plán s časovým harmonogramem
5. Vypíše checklist co připravit fyzicky (tisk, pomůcky)

### Session (~90 min)

| Fáze | Čas | Co se děje |
|------|-----|-----------|
| Probuzení Nexusu | 20 min | Quest Master (AI) představí misi, děti si tvoří/aktualizují postavu |
| Hlavní mise | 50 min | Průzkum planety, řešení problémů, hádanky, sokratovské dialogy |
| Fyzická aktivita | 10 min | Experiment, fotodokumentace, práce s pomůckami |
| Reflexe a uzavření | 10 min | Co jsme zjistili? XP, level-up |

**Role rodiče:** Facilitátor, ne přednášející. Pomáhá s technikou, pozoruje, ale odpovědi hledají děti samy (s pomocí Orákula).

### Po session

- Automatická aktualizace XP a levelů
- Reflexe v quest logu (co se povedlo, co bylo těžké)
- Podklady pro další session

---

## XP a progrese

### Jak se získává XP

| Akce | XP | Poznámka |
|------|----|----------|
| Dokončení questu | 30–80 | Podle délky a složitosti |
| Vyřešení hádanky/šifry | 10–20 | Bonus za elegantní řešení |
| Spolupráce | 15 | Prokazatelná týmová práce |
| Real-world aktivita | 20–40 | Fyzické aktivity (foto, experiment) |
| Kvalitní odůvodnění | 10–20 | Vysvětlení PROČ, ne jen CO |
| Reflexe / deník | 10 | Záznam co se naučili |

### Levely

| Level | XP | Odemyká |
|-------|----|---------|
| 1 — Nováček | 0 | Základní přístup k Nexusu |
| 2 — Průzkumník | 100 | Nová planeta, první speciální schopnost |
| 3 — Navigátor | 250 | Přístup k tajným zprávám |
| 4 — Specialista | 500 | Vlastní výzkumná laboratoř na Nexusu |
| 5 — Velitel mise | 800 | Možnost navrhovat vlastní questy |
| 6 — Strážce Nexusu | 1200 | Plný přístup k paměti Orákula |

---

## Technické řešení

QuestForge běží na **Claude Code** — CLI nástroji od Anthropic pro práci s AI.

| Komponenta | Řešení |
|-----------|--------|
| AI engine | Claude Code (Anthropic) |
| Plugin | QuestForge — 3 příkazy: `/prep`, `/quest`, `/progress` |
| Quest Master | Specializovaný AI agent v roli Orákula (NPC průvodce) |
| State management | Markdown soubory (žádná databáze, žádný frontend) |
| Kurikulum | 150+ markdown souborů (8 modulů × 5 aktivit + AI skripty + průvodci + pracovní listy) |

**Proč markdown?** Jednoduché na údržbu, čitelné bez speciálních nástrojů, verzovatelné přes Git, snadno rozšiřitelné.

---

## Co by potřeboval někdo, kdo chce začít sám

### Minimální varianta (1–2 hodiny setup)

Nepotřebujete celý systém. Stačí:

1. **Claude Code** nainstalovaný a funkční
2. **Jeden CLAUDE.md soubor** s instrukcemi: „Jsi Orákulum, vzdělávací AI pro děti. Nikdy nedávej přímé odpovědi, jen kladeš otázky..."
3. **Jeden příběhový rámec** — nemusí být vesmírná stanice, může být cokoliv (tajná laboratoř, záchranná expedice, detektivní agentura)
4. **Připravené aktivity** pro první session

Toto zvládne kdokoliv s Claude Code a základní představou, co chce děti naučit.

### Střední varianta (1 den setup)

Přidejte:

- **Kurikulární strukturu** — definujte 3–5 témat, která chcete pokrýt
- **XP systém** — motivace a progrese
- **Character sheets** — děti si vytvoří postavu
- **Quest log** — sledování postupu

### Plná varianta (QuestForge)

Kompletní systém s:

- 8 kurikulárními moduly (150+ souborů)
- Quest Master agentem
- Automatickou přípravou sessions
- Tisknutelnými materiály (šifry, hádanky, pracovní listy)
- Facilitátorskými průvodci

---

## Kontakt

Pokud vás QuestForge zaujal a chcete vědět víc:

**Zdeněk Macháček**
AI konzultant | Personal AI Systems

---

*QuestForge v1.0 | Cognitive Mirror Framework | 2026*
