---
name: questforge
description: "Triggers: /prep, /quest, /progress, 'questforge', 'quest', 'vzdělávání', 'mise pro děti'. When user needs quest-based learning session orchestration."
---
# QuestForge — Quest-Based Learning System

**Verze:** 1.0.0 | **Účel:** Orchestrace quest-based learningu pro domácí vzdělávání

---

## Kontext

Vzdělávací systém pro děti (11–13 let) postavený na Quest-Based Learning s narativním rámcem. Kurikulum existuje (8 modulů, 150+ souborů) v `curriculum/`, QuestForge je delivery infrastruktura.

### Klíčové principy
- **Kurikulum na pozadí** — děti nevidí "teď děláme finanční gramotnost"
- **Planety míchají témata** — každá mise kombinuje 2–4 kurikulární moduly
- **Cognitive Mirror** — nikdy přímé odpovědi, vždy sokratovské otázky
- **Mix digitálních a fyzických aktivit** — micro:bit, mikroskop, dalekohled, telefony
- **Kooperativní questy** — spolupráce = vyšší XP
- **Jazyk variabilní** — česky default, anglicky podle kontextu planety

### Architektura
- **State = markdown** — žádná DB, žádný frontend
- **3 commands:** `/prep` (rodič), `/quest` (děti + agent), `/progress` (přehled)
- **1 agent:** Quest Master (NPC průvodce, Orákulum)
- **Campaign dir:** `campaign/` (relativní k repu)

---

## Workflow

### /prep flow (rodič připravuje)
1. Načti campaign state (quest-log, characters, world)
2. Vyber kurikulární aktivity (2–4 z různých modulů)
3. Zabal do narativu planety
4. Generuj active-quest.md + session plan + hádanky
5. Generuj **session flow** (`session-NNN-flow.md`) — facilitátorský tahák:
   - Časová osa s konkrétními akcemi
   - Odemykací sekvence (mapa, databáze, logy) pro Field Computer
   - Správné řešení puzzlů (pořadí fragmentů, šifry)
   - Vodítka pro zaseknuté děti
6. Checklist co připravit fyzicky

### /quest flow (session s dětmi)
1. Ověř active-quest existuje
2. Spusť Quest Master agenta
3. Agent vede session (NPC role, hádanky, hodnocení)
4. Po session: aktualizace quest-log + character sheets

### /progress flow
1. Načti characters + quest-log
2. Zobraz přehled (XP, level, planety, doporučení)

---

## Soubory kampaně

```
campaign/
├── world.md              # Lore, planety, pravidla
├── characters/           # Character sheets operátorů
├── quest-log.md          # Historie misí
├── active-quest.md       # Aktuální quest
├── apps/                 # Volitelné: interaktivní web nástroje
├── puzzles/session-NNN/  # Hádanky per session
└── sessions/
    ├── session-NNN-plan.md  # Facilitátorský plán (detailní)
    └── session-NNN-flow.md  # Flow tahák (časová osa + odemykání)
```

---

## Kurikulum mapping

| Modul kurikula | Typické aktivity ve questu |
|----------------|---------------------------|
| Kritické myšlení | Analýza důkazů, rozlišování pravdivých/falešných informací |
| Informační gramotnost | Vyhodnocení zdrojů, SIFT metoda, fact-checking |
| Finanční gramotnost | Rozpočty, resource management, ekonomické rozhodování |
| Digitální gramotnost | Šifry, kódování, kybernetická bezpečnost |
| Emoční inteligence | Komunikace s NPC, empatie, vyjednávání |
| Adaptabilita | Neznámé prostředí, improvizace, řešení problémů |
| Komunikace | Prezentace zjištění, argumentace, naslouchání |
| Metakognice | Reflexe vlastního učení, strategie řešení |

---

## Quality gates

- Každá session pokrývá min. 2 kurikulární moduly
- Min. 1 fyzická aktivita
- Min. 1 hádanka/šifra
- Session plan má jasné časování (~90 min)
- Quest Master nikdy nedává přímé odpovědi

---

## Templates

V `skills/questforge/templates/` najdete:
- `quest-template.md` — šablona pro nový quest
- `character-template.md` — šablona postavy
- `session-plan.md` — šablona facilitátorského plánu
