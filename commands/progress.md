---
description: "Zobraz stav postav a questů v kampani"
---

# Progress — Stav postav a questů

**Verze:** 1.0.0 | **Účel:** Přehled postupu operátorů v kampani

Zobraz progress: $ARGUMENTS

---

## Kdy aktivovat

- Kontrola stavu obou postav
- Plánování další session
- Přehled co bylo dokončeno
- Motivace — ukázat dětem jejich pokrok

---

## Workflow

1. **Načti data**
   - Přečti character sheets v `campaign/characters/`
   - Přečti `campaign/quest-log.md`
   - Přečti `campaign/world.md` (planety, level thresholds)

2. **Generuj přehled**
   - Stav obou operátorů: level, XP, progress bar k dalšímu levelu
   - Schopnosti a inventář
   - Seznam dokončených questů s XP
   - Navštívené planety
   - Co odemyká další level

3. **Doporučení**
   - Která planeta/quest dál
   - Oblasti kurikula, které ještě nebyly pokryté
   - Streak / frekvence sessions

---

## Pravidla

| Situace | Akce |
|---------|------|
| Žádné dokončené questy | Zobraz "Kampaň čeká na první misi" + doporuč /prep |
| Chybí character sheets | "Operátoři se ještě nepřihlásili" |
| Velký gap mezi sessions | Navrhni kratší "warm-up" quest |
| Oba operátoři na max levelu | Navrhni nový narativní arc |

---

## Output formát

```
══════════════════════════════════════
  KAMPAŇ — STATUS REPORT
══════════════════════════════════════

  [Jméno 1] — Level X [████████░░] XXX/YYY XP
  Role: ...
  Schopnosti: ...

  [Jméno 2] — Level X [██████░░░░] XXX/YYY XP
  Role: ...
  Schopnosti: ...

──────────────────────────────────────
  MISE: X dokončeno | Planety: Y navštíveno
──────────────────────────────────────

  Poslední mise: [název] ([datum])
  Další level odemyká: [co]

  Doporučení: ...
══════════════════════════════════════
```

---

*Tip: Použij při začátku session pro rychlý recap.*
