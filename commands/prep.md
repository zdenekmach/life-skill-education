---
description: "Připrav quest session — generuj quest a session plán z kurikula"
---

# Prep — Připrav quest session

**Verze:** 1.0.0 | **Účel:** Generování questu a session plánu z kurikula

Připrav quest session: $ARGUMENTS

---

## Kdy aktivovat

- Rodič chce připravit další session pro děti
- Potřeba nového questu z kurikula
- Plánování víkendové/večerní session

---

## Workflow

1. **Načti stav kampaně**
   - Přečti `campaign/quest-log.md` — co už bylo dokončeno
   - Přečti character sheets v `campaign/characters/` — level, schopnosti, XP
   - Přečti `campaign/world.md` — dostupné planety, narativní arcy

2. **Vyber kurikulární obsah**
   - Projdi `curriculum/domain/model.yaml` — dostupné moduly a aktivity
   - Projdi `curriculum/<modul>/activities/` — konkrétní aktivity
   - Vyber 2–4 aktivity z RŮZNÝCH modulů (planety míchají témata)
   - Preferuj aktivity navazující na předchozí session
   - Pokud je to první session — začni úvodními aktivitami z více modulů

3. **Zabal do narativu**
   - Vyber planetu (novou nebo pokračování) z `world.md`
   - Vytvoř quest příběh propojující vybrané aktivity
   - Přidej hádanku/šifru jako engagement mechaniku
   - Navrhni fyzické aktivity (micro:bit, mikroskop, dalekohled, telefony)

4. **Generuj výstupy**
   - Aktualizuj `campaign/active-quest.md` — briefing, cíle, XP, materiály
   - Vytvoř `campaign/sessions/session-NNN-plan.md` — facilitátorský plán s časováním
   - Vytvoř hádanky v `campaign/puzzles/session-NNN/`
   - Pokud quest potřebuje tištěné materiály — vygeneruj a upozorni

5. **Checklist pro rodiče**
   - [ ] Co vytisknout
   - [ ] Co připravit fyzicky (props)
   - [ ] Co nahrát na micro:bit
   - [ ] Odhadovaný čas session

---

## Pravidla

| Situace | Akce |
|---------|------|
| První session | Začni úvodním questem na startovní planetě, character creation |
| Málo XP pro novou planetu | Pokračuj na aktuální planetě, přidej vedlejší quest |
| Kurikulum vyčerpáno pro aktuální planetu | Navrhni přesun na novou |
| Mezera >2 týdny od poslední session | Přidej "recap" fázi na začátek |
| Jeden z operátorů výrazně napřed v XP | Navrhni quest kde zaostávající vynikne |

---

## Gates

- [ ] Quest pokrývá min. 2 různé kurikulární moduly
- [ ] Session plan má jasné časování (celkem ~90 min)
- [ ] Minimálně 1 fyzická aktivita v session
- [ ] Minimálně 1 hádanka/šifra
- [ ] active-quest.md aktualizován
- [ ] Facilitátorský plán obsahuje sokratovské otázky

---

## Output

**Formát:** markdown
**Soubory:**
- `campaign/active-quest.md` (aktualizace)
- `campaign/sessions/session-NNN-plan.md` (nový)
- `campaign/puzzles/session-NNN/` (nové hádanky)

---

*Tip: Po vygenerování projdi session plan a uprav podle aktuálního naladění dětí.*
