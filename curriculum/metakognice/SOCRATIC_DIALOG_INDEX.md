---
title: "Sokratovský Dialog - Index Dokumentů"
module: metakognice
type: index
version: "1.0.0"
created: "2026-01-09"
language: cs
---

# 🧠 Sokratovský Dialog - Kompletní Balíček

> **Verze:** 1.0.0 | **Datum:** 2026-01-09 | **Modul:** Metakognice

Kompletní systém pro vedení Sokratovských dialogů s AI, určený pro děti 11-13 let.

---

## Soubory v Tomto Balíčku

### 📋 Primární Script

**`ai-scripts/script-03-socratic-gap.md`** (18 KB, 512 řádků)

Kompletní AI interaction script s:
- System Prompt pro chatbot AI
- Pracovní postup AI (POSLECH → IDENTIFIKACE → OTÁZKA)
- 4 vzorové dialogy s reálnými rozhovory
- Tabulka logických mezer
- Safeguards a časové limity
- Mapování na Activity 4 kurikula

**Kdo by to měl číst:**
- Vývojáři AI/Prompt Engineers (System Prompt)
- Facilitátoři (Vzorové dialogy, Safeguards)
- Kurikulární designéři (Mapování na aktivity)

---

### 📖 Průvodce pro Facilitátory

**`resources/socratic-facilitator-quick-guide.md`** (8,5 KB, 302 řádků)

Praktický průvodce pro rodiče a učitele s:
- Kontrolní seznam přípravy
- Pozorovací list během aktivit
- Pokyny pro různé situace
- Reflexní otázky
- Nejčastější chyby a jejich řešení
- Časový plán

**Kdo by to měl číst:**
- Rodiče a učitelé (MUSÍ)
- Lektoři a facilitátoři
- Všichni, kdo vedou aktivitu

**Kdy si to přečíst:**
- Minimálně 1 den před aktivitou
- Ideálně si vytisknout a mít u sebe během aktivity

---

### 📝 Pracovní List pro Dítě

**`resources/socratic-student-worksheet.md`** (11 KB, 272 řádků)

Interaktivní pracovní list pro tisk s:
- Fází PŘED, BĚHEM, PO
- Prostorem pro zápis otázek od AI
- Reflexí změny myšlení
- Sbírkou typů sokratovských otázek
- Zpracováním pro facilitátora

**Kdo by to měl Using:**
- Děti (MUSÍ - během aktivity)
- Facilitátoři (pro sledování reflexe)

**Kdy si to vytisknout:**
- Před aktivitou (1 list na dítě)
- Volitelně: Připravit 1-2 extra kopie

---

## Rychlý Start (5 minut)

### 1. Facilitátor
1. Přečtete si **`socratic-facilitator-quick-guide.md`** (15 minut)
2. Vytisknete si **pozorovací list** (příloha v průvodci)

### 2. Dítě
1. Dostane vytištěný **`socratic-student-worksheet.md`**
2. Facilitátor vysvětlí: "Budeme si hrát Sokratova hra - já se ptám, ty si myslíš"

### 3. AI Chatbot
1. Kopiř system prompt z **`script-03-socratic-gap.md`**
2. Vlož do AI chatbotu
3. Začni dialog podle návodu v průvodci

### 4. Po Aktivitě
1. Dítě vyplní pracovní list
2. Facilitátor položí reflexní otázky
3. Zaznamená poznámky do pozorovacího listu

---

## Mapování na Kurikulum

### Activity 4: Sokratovský Dialog

| Aspekt | Detail |
|--------|--------|
| **Bloom Level** | 4/6 - Evaluate |
| **Cíl** | Vyhodnotit vlastní strategie pomocí otázek |
| **Čas** | 30 minut (5 PŘED + 15 BĚHEM + 10 PO) |
| **AI Role** | Script-03-socratic-gap |
| **Dokumenty** | Všechny 3 soubory |

### Propojení s Ostatními Aktivitami

- **Activity 1-3**: Příprava na kritické myšlení
- **Activity 4**: 🎯 Sokratovský dialog (TOT BALÍČEK)
- **Activity 5**: Dítě si klád otázky samo (meta-aplikace)

---

## Klíčové Koncepty

### Co Je Sokratovský Dialog?

Metoda, kde facilitátor **pokládá otázky** místo toho, aby dával **odpovědi**. Cílem je, aby si osoba sama **uvědomila** své chyby v myšlení.

Principy:
1. **Posluchač (AI) pokládá otázku**
2. **Mluvčí (dítě) přemýšlí a odpovídá**
3. **Následující otázka vede hlubší**
4. **Nakonec si osoba sama poví: "Aha!"**

### Logické Mezery, Které AI Hledá

```
Skrytý předpoklad → "Platí to VŽDY?"
Bez důkazu       → "Jak víš, že je to pravda?"
Zaměšené pojmy   → "Je to totéž?"
Rozpor           → "To spolu nejde, ne?"
Generalizace     → "Existuje výjimka?"
```

### Typy Otázek AI

1. **Klarifikační** - Ujasní pojmy ("Co myslíš tím...?")
2. **Předpoklady** - Odhalí skryté ("Na čem to stojí?")
3. **Evidence** - Požádá důkaz ("Jak víš?")
4. **Perspektiva** - Změní úhel ("Jak by to viděl...?")
5. **Důsledky** - Prozkoumá "co kdyby" ("Jaký by to mělo dopad?")
6. **Meta-otázky** - Reflexe ("Proč se tě ptám?")

---

## Safeguards (Bezpečnost)

### Časový Limit
- **Maximum 15 minut** sokratovského dialogu
- Po 15 minutách: Povinná přestávka
- Pokud chce dítě pokračovat: "Příště!"

### Facilitátor Přítomen
- Sedí vedle nebo v dohledu
- Sleduje pocity dítěte
- Intervencuje, pokud se dítě frustráciuje >2 min

### AI Guardrails
- ✗ Nikdy neříká "To je špatně"
- ✗ Nikdy nepředjímá ani nevysvětluje
- ✓ Zůstává v tématu metakognice
- ✓ Respektuje hranice dítěte

---

## Vzorové Dialogy (4 Příklady)

V **`script-03-socratic-gap.md`** najdeš 4 kompletní vzorové dialogy:

1. **Dialog 1: Předpoklad** - "Učení se večer"
2. **Dialog 2: Nejasná definice** - "Jsem chytrý/á"
3. **Dialog 3: Evidence** - "Více práce je lepší"
4. **Dialog 4: Perspektiva** - "Introverts nejsou vůdci"

Každý dialog ukazuje:
- Tvrzení dítěte
- Jak AI identifikuje mezeru
- Řadu otázek
- Jak dítě dospěje k poznání

---

## Nejčastější Otázky

### Q: Co když dítě neví odpověď?
**A:** To je OK! AI položí jednodušší otázku nebo změnit typ. Pokud po 2-3 pokusech neví, řekl: "Je to těžké, není nic špatného."

### Q: Co když se dítě frustráciuje?
**A:** Pauzovat. Přejít na méně Sokratovský přístup (Script 1 nebo bez AI). Wellbeing > Metodologie.

### Q: Jak dlouho to trvá, než dítě pochopí?
**A:** 2-3 seance. Nejdřív bude zvědavé "Proč mi AI neodpovídá?", pak pochopí. Po 4. seanci si bude klád otázky samo.

### Q: Mohu používat s mladšími/staršími dětmi?
**A:** 10-12 let: Jednodušší otázky a kratší seance (10 minut)
13-14 let: Identické
15+ let: Složitější témata, déle (20 minut)

### Q: Mohu tuto metodou bez AI?
**A:** Ano! Facilitátor pokládá otázky sám. Ale AI má výhodu: Dítě si neuvědomuje, že je to připraveno (levnější se čítí automaticky).

---

## Jak Měřit Úspěch

### Měřítka Úspěchu

✓ **Skvělé (5/5):** Dítě samo si klád otázky, změnilo názor, vidí důvod
✓ **Velmi dobré (4/5):** Dítě pochopilo meshu, ale nezmění názor
✓ **Dobré (3/5):** Dítě odpovídalo, ale ne do hloubky
✓ **Částečné (2/5):** Dítě pochopilo, ale frustrované
✓ **Počátek (1/5):** Dítě si všimlo, že AI se ptá na otázky

### Sledovací List Pokroku

Zaznamenávej v **pozorovacím listu** z průvodce:
- Které otázky AI byly nejúčinnější?
- Kde se dítě frustráciilo?
- Vidíš změnu myšlení?
- Jak se dítě cítilo?

---

## Přílohy a Další Materiály

### V Tomto Balíčku
- ✓ System Prompt (pro AI)
- ✓ Vzorové dialogy (4 příklady)
- ✓ Pracovní postupy (AI, facilitátor)
- ✓ Pracovní list pro dítě
- ✓ Pozorovací list
- ✓ Reflexní otázky

### V Ostatních Modulech
- `resources/karticky-reflexnich-otazek.md` - Tisknutelné kartičky
- `resources/poster-meta-cyklus.md` - Vizuální pomůcka

---

## Příští Kroki

Po úspěšném Sokratovském dialogu:

1. **Activity 5: Můj Učební Projekt**
   - Dítě pracuje na vlastním projektu
   - Samo si klád sokratovské otázky
   - Metakognice se stává praktickou

2. **Deník Reflexe (Ongoing)**
   - Dítě si zapisuje své "aha!" momenty
   - Facilitátor vidí dlouhodobý pokrok

3. **Přenos do Jiných Oblasti**
   - Dítě používá Sokratovské otázky v matematice
   - Dítě si klád otázky o přátelstvích
   - Metakognice je generalizovaná

---

## Kontakt a Verze

**Verze:** 1.0.0
**Vytvořeno:** 2026-01-09
**Framework:** Cognitive Mirror First Approach
**Licence:** CC-BY-SA

**Projekt:** Life Skills Education - Metakognice Modul
**Autoři:** Curriculum Team

---

## Rychlý Ref Card

```
┌──────────────────────────────────────────────────┐
│ SOKRATOVSKÝ DIALOG - RYCHLÝ PŘEHLED             │
├──────────────────────────────────────────────────┤
│ ČAS: 30 min (5 PŘED + 15 BĚHEM + 10 PO)        │
│ VĚKOVÁ SKUPINA: 11-13 let                       │
│ CÍЛЬ: Evaluace vlastní myšlení (Bloom L4)      │
│ AI ROLE: Pokládá otázky, nikdy neodpovídá     │
│ FACILITÁTOR: Vždy přítomen, jen pozoruje      │
│                                                  │
│ KLÍČ: Otázka → Reflexe → Poznání               │
├──────────────────────────────────────────────────┤
│ 📄 Script:    script-03-socratic-gap.md        │
│ 📖 Průvodce:  socratic-facilitator-quick-guide │
│ 📝 Worksheet: socratic-student-worksheet.md    │
└──────────────────────────────────────────────────┘
```

---

**Připraveno pro tisk a okamžité použití. Veškeré soubory jsou v češtině.**

*Cognitive Mirror First - Zdravá integrace AI do vzdělávání dětí*
