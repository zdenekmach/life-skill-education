---
type: "curriculum"
subtype: "resource"
title: "Aktualizace Modulu Metakognice: Script-03 Sokratovská Mezera"
date: "2026-01-18"
module: ""
tags: []
---
# Aktualizace Modulu Metakognice: Script-03 Sokratovská Mezera

> **Status:** ✓ Hotovo a Nasazovatelné | **Verze:** 1.0.0 | **Datum:** 2026-01-09

---

## Co Je Nového

Modul Metakognice byl rozšířen o **kompletní systém Sokratovských dialogů s AI** - třetí z tří interakčních scriptů pro Cognitive Mirror framework.

### Výstupy

| Soubor | Účel | Formát |
|--------|------|--------|
| `ai-scripts/script-03-socratic-gap.md` | Primární AI script s System Prompt | Markdown |
| `resources/socratic-facilitator-quick-guide.md` | Průvodce pro učitele/rodiče | Markdown (printable) |
| `resources/socratic-student-worksheet.md` | Pracovní list pro dítě | Markdown (A4 worksheet) |
| `SOCRATIC_DIALOG_INDEX.md` | Navigace a index | Markdown |

---

## Struktura Scriptu

```
┌─────────────────────────────────────────────────┐
│     SOKRATOVSKÝ DIALOG - ARCHITEKTURA           │
├─────────────────────────────────────────────────┤
│                                                 │
│  1. SYSTEM PROMPT                               │
│     └─ Role: Sokratovský tazatel                │
│     └─ Úkol: Pokládat otázky                    │
│     └─ Zakázáno: Dávat odpovědi                 │
│                                                 │
│  2. PRACOVNÍ POSTUP AI (5 kroků)                │
│     └─ Poslech vysvětlení                       │
│     └─ Identifikace logické mezery              │
│     └─ Klád otázku                              │
│     └─ Čekání na odpověď                        │
│     └─ Reflexe a sledování pokroku              │
│                                                 │
│  3. TYPY OTÁZEK (6 kategorií)                   │
│     └─ Klarifikační                             │
│     └─ Předpoklady                              │
│     └─ Evidence                                 │
│     └─ Perspektiva                              │
│     └─ Důsledky                                 │
│     └─ Meta-otázky                              │
│                                                 │
│  4. LOGICKÉ MEZERY (7 typů)                     │
│     └─ Skrytý předpoklad                        │
│     └─ Bez důkazu                               │
│     └─ Zaměšené pojmy                           │
│     └─ Rozpor                                   │
│     └─ Generalizace                             │
│     └─ Kauzalita                                │
│     └─ Fokus na detaily                         │
│                                                 │
│  5. VZOROVÉ DIALOGY (4 příklady)                │
│     └─ Dialog 1: Skrytý předpoklad              │
│     └─ Dialog 2: Nejasná definice               │
│     └─ Dialog 3: Evidence                       │
│     └─ Dialog 4: Perspektiva                    │
│                                                 │
│  6. SAFEGUARDS                                  │
│     └─ Max 15 minut                             │
│     └─ Facilitátor přítomen                     │
│     └─ AI guardrails                            │
│     └─ Protokol pro frustraci                   │
│                                                 │
└─────────────────────────────────────────────────┘
```

---

## Mapování na Kurikulum

### Activity 4: Sokratovský Dialog

```
AKTIVITA 4
├─ Bloom Level: EVALUATE (úroveň 4)
├─ Čas: 30 minut (5 PŘED + 15 BĚHEM + 10 PO)
├─ Cíl: Vyhodnotit vlastní strategie pomocí otázek
├─ AI Role: Script-03-socratic-gap
├─ Materiály: 3 dokumenty (script + guide + worksheet)
└─ Status: ✓ Hotovo
```

### Propojení s Ostatními Aktivitami

```
Activity 1 → Activity 2 → Activity 3 → Activity 4 ⭐ → Activity 5
Detektiv    Učím        PŘED-BĚHEM-   Sokratovský  Moje
            robota      PO deník      dialog       učení
                                      (s AI)
```

---

## Primární Dokument: script-03-socratic-gap.md

### Struktura (512 řádků)

1. **Header & Metadata** (YAML front-matter)
2. **Účel a Kdy Jej Používat**
3. **System Prompt pro AI** (copy-paste ready)
4. **Pracovní Postup pro AI** (5 kroků s příklady)
5. **Vzorové Dialogy** (4 kompletní příklady)
6. **Tabulka Logických Mezer**
7. **Typy Sokratovských Otázek** (6 kategorií)
8. **Pokyny pro Různé Situace**
9. **Safeguards a Časové Limity**
10. **Mapování na Activity 4**
11. **Tisknutelné Kartičky**
12. **Poznámka pro Facilitátora**
13. **Verze a Historia**

### System Prompt - Klíčové Prvky

```
ROLE: Sokratovský tazatel

ÚKOL:
1. Poslouchat vysvětlení
2. Identifikovat logickou mezeru
3. Položit otázku na mezeru
4. Čekat na odpověď
5. Chválit snahu

ZAKÁZÁNO: Odpovědi, hodnocení, přednášení
```

### 4 Vzorové Dialogy

Každý dialog obsahuje:
- Konkrétní situaci a tvrzení dítěte
- Jak AI identifikuje mezeru
- Řadu otázek vedoucích k poznání
- Analýzu: "Co se stalo"

---

## Průvodce Pro Facilitátory: socratic-facilitator-quick-guide.md

### Struktura (302 řádků)

1. **Aktivita Stručně** (čas, cíl, role)
2. **Příprava** (5 min - kontrolní seznam)
3. **BĚHEM** - Role Facilitátora
4. **Co Dělat** (podpora, pozorování)
5. **Co NEDĚLAT** (běžné chyby)
6. **Logické Mezery** (co hledat)
7. **Pokyny pro 5 Situací**
8. **Reflexní Fáze** (10 minut PO)
9. **Mapování na Cíle Modulu**
10. **Časový Plán** (30 minut)
11. **Nejčastější Chyby** (7 chyb + řešení)
12. **Když se Podařilo** (poznáte úspěch)

### Pozorovací List

Připraven pro facilitátora k sledování:
- Otázky, které AI pokládá
- Odpovědi dítěte
- Identifikované logické mezery
- Reakte dítěte (frustrace, zájem)
- Poznámky pro reflexi

### Časový Plán

```
CELKOVÝ ČAS: 30 minut

PŘED    │ Úvod + otázka k zahájení    │ 5 min
────────┼─────────────────────────────┼──────
BĚHEM   │ Sokratovský dialog s AI      │ 15 min
        │ (vy jen pozorujete)         │
────────┼─────────────────────────────┼──────
PO      │ Reflexní otázky + worksheet │ 10 min
```

---

## Pracovní List Pro Dítě: socratic-student-worksheet.md

### Struktura (272 řádků)

1. **Fáze PŘED** (První myšlenka, jistota)
2. **Fáze BĚHEM** (Zápis otázek AI, pocity)
3. **Fáze PO** (Změna myšlení, logické mezery)
4. **Reflexe** (Co jsem se naučil/a)
5. **Příprava na Příště**
6. **Sbírka Typů Otázek** (reference)
7. **Zpráva Pro Facilitátora**
8. **Zajímavost o Sokratovi**

### Formát

- Tisknutelný (A4)
- Interaktivní (psaní, kreslení, zaškrtávání)
- Věkově vhodný (11-13 let)
- Česky bez akademismu

---

## Index a Navigace: SOCRATIC_DIALOG_INDEX.md

Centrální dokument pro:
- Orientaci v systému
- Rychlý start (5 minut)
- Mapování na kurikulum
- Klíčové koncepty
- FAQ (10 otázek)
- Měřítka úspěchu

---

## Bezpečnost a Safeguards

### Časový Limit
- **Maximum 15 minut** sokratovského dialogu
- Po 15 minutách povinná přestávka
- Pokud chce dítě pokračovat: Příště

### Facilitátor Vždy Přítomen
- Sleduje pocity a expresi dítěte
- Intervencuje při frustrace >2 min
- Pozoruje, zda AI neodchází z tématu

### AI Guardrails
- ✗ Nikdy neříká "To je špatně"
- ✗ Nikdy nepředjímá
- ✓ Zůstává v tématu metakognice
- ✓ Respektuje hranice dítěte

### Quando Se Vrátit Zpět
- Pokud dítě se příliš frustráciuje → Script 1 (Teachable AI)
- Pokud dítě se bojí → Script 2 (Reflective Checkpoint)
- Pokud žádné AI → Facilitátor pokládá otázky

---

## Příklady Użití

### Případ 1: Skrytý Předpoklad

```
Dítě: "Vždy se učím lépe večer"
AI: "Je to vždy? Existuje výjimka?"
Dítě: "Měl jsem hlad..."
AI: "Takže není jen čas, ale i fyzický stav?"
Dítě: "Ano! To má smysl!"
```

### Případ 2: Nejasná Definice

```
Dítě: "Jsem špatný/á v matematice"
AI: "Co přesně znamená 'špatný/á'?"
Dítě: "Dělám chyby v testech"
AI: "Je test = všechna matematika?"
Dítě: "Ne, já jsem dobrý/á v problémech..."
```

---

## Měřítka Úspěchu

| Úroveň | Poznámka | Příklad |
|--------|----------|---------|
| **5** | Dítě samo si klád otázky | "Čekej, ale co kdybych..." |
| **4** | Dítě změnilo názor | "Mýlil jsem se..." |
| **3** | Dítě pochopilo mezeru | "Vidím, že to není vždy..." |
| **2** | Dítě odpovídalo | Odpovědi, ale bez hloubky |
| **1** | Dítě si všimlo | "Ptáš se na otázky?" |

---

## Integrace do Kurzu

### Před Aktivitou
1. Facilitátor si přečte průvodce
2. Dítě dostane worksheet
3. Kopiř AI system prompt do chatbotu

### Během Aktivity
1. PŘED: Úvod + otázka (5 min)
2. BĚHEM: Dialog s AI (15 min)
3. PO: Reflexe (10 min)

### Po Aktivitě
1. Dítě si přečte svůj worksheet
2. Facilitátor zaznamená do pozorovacího listu
3. Tracking v dlouhodobém deníku

---

## Verzování a Údržba

**Verze:** 1.0.0
**Vytvořeno:** 2026-01-09
**Status:** ✓ Hotovo a Nasazovatelné
**Poslední Aktualizace:** 2026-01-09

### Budoucí Verze
- v1.1.0: Feedback z pilotu
- v1.2.0: Rozšíření na jiné věkové skupiny
- v2.0.0: Integrace s monitorovacím systémem

---

## Příští Kroky

### Krátkodobě (týdny 1-2)
- [ ] Pilot s 2-3 dětmi
- [ ] Sbír feedback
- [ ] Drobné úpravy

### Střednědobě (měsíc 1)
- [ ] Nasazení s prvním balením
- [ ] Školení facilitátorů
- [ ] Sbírat metriky

### Dlouhodobě (měsíce 2+)
- [ ] Integrace s Activity 5
- [ ] Rozšíření na jiné moduly
- [ ] Scaling pro různé věkové skupiny

---

## Kde Najít Dokumenty

### Primární Dokumenty
```
outputs/curriculum/metakognice/
├── ai-scripts/
│   └── script-03-socratic-gap.md ⭐
├── resources/
│   ├── socratic-facilitator-quick-guide.md ⭐
│   └── socratic-student-worksheet.md ⭐
└── SOCRATIC_DIALOG_INDEX.md ⭐
```

### Navigace
- **Pro AI**: Otevři `script-03-socratic-gap.md` → System Prompt
- **Pro Facilitátora**: Otevři `socratic-facilitator-quick-guide.md`
- **Pro Dítě**: Vytisknout `socratic-student-worksheet.md`
- **Přehled**: Otevři `SOCRATIC_DIALOG_INDEX.md`

---

## Poznámka pro Implementaci

Sokratovský dialog je **nejintenzivnější aktivita v modulu** - vyžaduje plnou pozornost a reflexi. Ale je to také **nejsilnější nástroj pro rozvoj kritického myšlení**.

Pokud vidíte, že dítě si začne samo pokládat otázky - to je úspěch. Metakognice se stala automatickou.

---

**Sokratovská Mezera je nyní součástí modulu Metakognice - verze 1.1.0**

*Cognitive Mirror First - Zdravá integrace AI do vzdělávání dětí*
