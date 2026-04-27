---
description: "Spusť Quest Master agenta pro interaktivní session s dětmi"
---

# Quest — Spusť quest session

**Verze:** 1.0.0 | **Účel:** Spuštění Quest Master agenta pro interaktivní session s dětmi

Spusť quest: $ARGUMENTS

---

## Kdy aktivovat

- Děti jsou připraveny na session
- `/prep` už vygeneroval active-quest.md a session plan
- Rodič chce spustit interaktivní quest s AI průvodcem

---

## Workflow

1. **Ověř připravenost**
   - Zkontroluj že `campaign/active-quest.md` existuje a má status "Čeká na operátory"
   - Zkontroluj že character sheets existují (pokud ne — session začne tvorbou postav)

2. **Spusť Quest Master agenta**
   - Deleguj na agenta `quest-master` s kontextem:
     - `campaign/world.md` — lore a pravidla
     - `campaign/active-quest.md` — aktuální quest
     - `campaign/characters/*.md` — character sheets
     - `campaign/puzzles/session-NNN/` — hádanky pro tuto session
   - Agent přebírá dialog s dětmi

3. **Po skončení session**
   - Quest Master zapíše výsledky do `campaign/quest-log.md`
   - Aktualizuje character sheets (XP, poznámky)
   - Aktualizuje status v `active-quest.md`

---

## Pravidla

| Situace | Akce |
|---------|------|
| Chybí active-quest.md | Upozorni — nejdřív spustit `/prep` |
| Chybí character sheets | Quest Master začne tvorbou postav |
| Děti chtějí odbočit od questu | Nechej je — flexibilita je důležitější než plán |
| Děti jsou frustrované | Quest Master nabídne hint (nikdy přímou odpověď) |
| Čas vypršel ale quest nedokončen | Uložit stav, pokračovat příště |

---

## Output

Quest Master agent přebírá konverzaci. Po skončení aktualizuje:
- `campaign/quest-log.md`
- `campaign/characters/*.md`
- `campaign/active-quest.md` (status → dokončen)

---

*Poznámka: Quest Master = interaktivní NPC, ne tutor. Hraje role, pokládá otázky, nikdy nevysvětluje "teď se učíte X".*
