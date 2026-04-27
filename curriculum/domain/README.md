---
type: note
title: "Domain Knowledge Model: Meta-dovednosti pro děti 11-13 let"
project: life-skills-education
created: 2026-01-19
---
# Domain Knowledge Model: Meta-dovednosti pro děti 11-13 let

**Verze:** 1.0.0
**Datum vytvoření:** 2026-01-08
**Projekt:** life-skills-education

---

## O tomto modelu

Tento domain knowledge model zachycuje klíčové koncepty, vztahy a entity v oblasti vzdělávání meta-dovedností pro děti 11-13 let s využitím AI jako "cognitive mirror".

Model slouží jako:
- **Reference** pro konzistentní používání terminologie
- **Mapa** vztahů mezi koncepty
- **Základ** pro další research a vývoj

---

## Struktura modelu

```
knowledge/domain/
├── README.md              # Tento soubor
├── model.yaml            # Hlavní model (actors, concepts, artifacts)
├── relations.yaml        # Vztahy mezi entitami
├── concept-map.md        # Mermaid vizualizace
├── glossary.md           # Slovník pojmů (CZ/EN)
└── sources.md            # Reference a zdroje (61 zdrojů)
```

---

## Statistiky modelu

| Metrika | Hodnota |
|---------|---------|
| **Verze** | 1.0.0 |
| **Aktéři** | 4 |
| **Koncepty** | 26 |
| **Artefakty** | 6 |
| **Vztahy** | 52 |
| **Zdroje** | 61 |
| **Pojmy v glossary** | 35+ |

---

## Klíčové entity

### Aktéři

| ID | Název | Role |
|----|-------|------|
| `child` | Dítě (11-13 let) | Primární uživatel |
| `parent` | Rodič/Vychovatel | Facilitátor |
| `teacher` | Učitel | Facilitátor (B2B) |
| `ai_assistant` | AI Asistent | Cognitive Mirror nástroj |

### Core koncepty (Meta-dovednosti)

| ID | Název | Kritické období |
|----|-------|-----------------|
| `metacognition` | Metakognice | 11-17 let |
| `executive_functions` | Exekutivní funkce | 10-15 let |
| `critical_thinking` | Kritické myšlení | - |
| `learning_to_learn` | Učení se učit | - |
| `emotional_intelligence` | Emocionální inteligence | - |
| `self_regulation` | Seberegulace | - |
| `communication_collaboration` | Komunikace a spolupráce | - |
| `digital_literacy` | Digitální gramotnost | - |

### Klíčové frameworky

| ID | Název | Zdroj |
|----|-------|-------|
| `cognitive_mirror` | Cognitive Mirror Framework | Frontiers 2025 |
| `casel_framework` | CASEL (5 SEL kompetencí) | casel.org |
| `p21_framework` | P21 / 4Cs | Battelle for Kids |
| `finnish_t1_t7` | Finské T1-T7 | Finnish NAE |
| `oecd_learning_compass` | OECD Learning Compass 2030 | OECD |

### Plánované artefakty

| ID | Název | Status | Timeline |
|----|-------|--------|----------|
| `ai_reflection_partner` | AI Reflection Partner | Planned | Q2 2026 |
| `socratic_ai_dialog` | Socratic AI Dialog | Planned | Q2 2026 |
| `metacognition_tracker` | Meta-cognition Tracker | Planned | Q3 2026 |

---

## Jak používat model

### 1. Rychlé vyhledání pojmu

Otevřete `glossary.md` a vyhledejte český nebo anglický termín.

### 2. Pochopení vztahů

Otevřete `concept-map.md` pro vizuální Mermaid diagramy nebo `relations.yaml` pro strojově čitelné vztahy.

### 3. Hledání zdrojů

Použijte `sources.md` pro kompletní seznam akademických zdrojů s URL.

### 4. Strojové zpracování

Parsujte `model.yaml` a `relations.yaml` pro automatizované dotazy.

---

## Klíčové insights z modelu

### 1. Kritické vývojové okno

Věk 11-13 let je kritickým obdobím pro:
- **Metakognici** (rozvoj 11-17 let)
- **Exekutivní funkce** (rapidní vývoj 10-15 let)
- **Abstraktní myšlení** (Piagetova formálně-operační fáze)

### 2. Cognitive Mirror jako diferenciátor

AI designovaná jako "teachable agent" (učitelný nováček) namísto "answer machine":
- Využívá **protégé efekt**
- Mitiguje **cognitive offloading**
- Aktivně rozvíjí **metakognici**

### 3. Framework konsenzus

Všechny hlavní frameworky (OECD, P21, CASEL, Finnish T1-T7, WEF) se shodují na:
- Kritickém myšlení
- Kreativitě
- Spolupráci
- Komunikaci
- Učení se učit
- Digitální gramotnosti

### 4. Strategická příležitost

- **Timing:** AI tutoring mainstream 2025-2026
- **Gap:** Žádné AI nástroje v CZ pro meta-dovednosti
- **Window:** Reforma RVP 2027 = vstup do škol

---

## Verzování

| Verze | Datum | Změny |
|-------|-------|-------|
| 1.0.0 | 2026-01-08 | Iniciální verze modelu |

---

## Příbuzné dokumenty

- [Výzkumná zpráva: Meta-dovednosti](../outputs/research/2026-01-08-meta-skills-education.md)
- [Výzkumná zpráva: Cognitive Mirror](../outputs/research/2026-01-08-cognitive-mirror-framework.md)
- [Výzkumná zpráva: Finský systém](../outputs/research/2026-01-08-finnish-education.md)
- [Výzkumná zpráva: 21st century skills](../outputs/research/2026-01-08-21st-century-skills.md)
- [Strategický plán](../strategic-plan-ai-first-mover-2026-01-08.md)
- [Wardley Map](../context/strategic-thinking/wardley-maps/meta-skills-education-map.md)

---

*Domain model vytvořen jako součást projektu life-skills-education*
