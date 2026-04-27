---
type: "curriculum"
subtype: "activity"
title: "Aktivita 1: Strážce hesla"
date: "2026-01-18"
module: ""
tags: []
---
# Aktivita 1: Strážce hesla

## Přehled

### Cíl
Naučit děti vytvářet a spravovat silná hesla a pochopit důležitost dvoufázového ověření (2FA).

### Výstupy
Po aktivitě žáci:
- Vědí, co dělá heslo silným
- Umí vytvořit zapamatovatelné, ale bezpečné heslo
- Rozumí, proč existuje 2FA a jak funguje
- Znají základy správce hesel

### Časový plán
| Fáze | Čas | Aktivita |
|------|-----|----------|
| Úvod | 5 min | "Jaké je tvoje heslo?" soutěž |
| Teorie | 10 min | Anatomie silného hesla |
| Praxe | 20 min | Tvorba hesel + 2FA |
| Reflexe | 10 min | Akční plán |

---

## Průběh aktivity

### 1. Úvod: Hra "Uhádni heslo" (5 min)

**Setup:**
Ukaž statistiku nejčastějších hesel (bez skutečného lámání):

```
TOP 10 NEJHORŠÍCH HESEL 2025:

1. 123456
2. password
3. 12345678
4. qwerty
5. abc123
6. heslo
7. 111111
8. password123
9. admin
10. iloveyou
```

**Diskuse:**
- Proč lidé volí tato hesla?
- Co mají společného?
- Jak dlouho by trvalo je prolomit? (sekundy!)

---

### 2. Teorie: Anatomie silného hesla (10 min)

#### Co dělá heslo silným?

```
╔══════════════════════════════════════════════════════════╗
║                  SILNÉ HESLO                             ║
╠══════════════════════════════════════════════════════════╣
║                                                          ║
║   DÉLKA         → Minimálně 12 znaků (čím víc, tím líp) ║
║   SLOŽITOST     → Mix písmen, číslic, symbolů            ║
║   UNIKÁTNOST    → Jiné pro každý účet!                  ║
║   NEPŘEDVÍDATELNOST → Žádná slova ze slovníku           ║
║                                                          ║
╠══════════════════════════════════════════════════════════╣
║                                                          ║
║   ❌ ŠPATNĚ:  heslo123, MojeJmeno2010, qwerty            ║
║   ✅ DOBŘE:   K0l@č-Str0m-7-M0drý!                       ║
║                                                          ║
╚══════════════════════════════════════════════════════════╝
```

#### Metoda "Passphrase" (heslo-věta)

```
KROK 1: Vymysli větu, kterou si zapamatuješ
        "Můj pes Rek má 4 nohy a miluje piškoty"

KROK 2: Vezmi první písmena + čísla
        MpRm4namP

KROK 3: Přidej symboly
        MpRm4namP!@

KROK 4: Nahraď některá písmena
        MpRm4n@mP!@

VÝSLEDEK: 12 znaků, mix všeho, zapamatovatelné!
```

#### Alternativa: 4 náhodná slova

```
Koláč-Strom-Modrý-7

= 18 znaků
= Snadno zapamatovatelné
= Těžké prolomit (kombinace jsou astronomické)
```

---

### 3. Praxe: Tvorba hesel (20 min)

#### Cvičení 1: Hodnocení hesel (5 min)

**Rozdej karty s hesly. Děti hodnotí 1-5:**

| Heslo | Délka | Složitost | Hodnocení |
|-------|-------|-----------|-----------|
| martin2010 | 10 | nízká | ⭐ |
| P@ssw0rd! | 9 | střední | ⭐⭐ |
| K0l@č-Str0m-7! | 14 | vysoká | ⭐⭐⭐⭐ |
| správně-kůň-baterie-sponka | 27 | vysoká | ⭐⭐⭐⭐⭐ |

#### Cvičení 2: Vytvoř vlastní heslo (10 min)

**Pracovní list:**

```
MOJE BEZPEČNÉ HESLO

Metoda 1: Věta
1. Moje věta: ___________________________________________
2. První písmena: ______________________________________
3. S čísly a symboly: __________________________________

Metoda 2: Náhodná slova
4. Čtyři slova: ________________________________________
5. S číslem a symbolem: ________________________________

POZNÁMKA: Toto heslo NEPOUŽÍVEJ - je to jen cvičení!
Skutečné heslo si vytvoř doma soukromě.
```

**AI asistence (volitelně):**
Použij skript `script-01-password-coach.md` pro zpětnou vazbu na strukturu hesla (ne na skutečné heslo!).

#### Cvičení 3: Co je 2FA? (5 min)

```
╔═══════════════════════════════════════════════════════════╗
║                DVOUFÁZOVÉ OVĚŘENÍ (2FA)                   ║
╠═══════════════════════════════════════════════════════════╣
║                                                           ║
║   1. NĚCO, CO ZNÁŠ         = Heslo                       ║
║              +                                            ║
║   2. NĚCO, CO MÁŠ          = Telefon (SMS, aplikace)     ║
║              =                                            ║
║   DVOJNÁSOBNÁ OCHRANA!                                    ║
║                                                           ║
╠═══════════════════════════════════════════════════════════╣
║                                                           ║
║   I když někdo zjistí heslo, bez tvého telefonu          ║
║   se nepřihlásí!                                          ║
║                                                           ║
║   TYPY 2FA:                                               ║
║   • SMS kód (méně bezpečné)                              ║
║   • Autentikační aplikace (Google/Microsoft Authenticator)║
║   • Bezpečnostní klíč (hardware)                         ║
║                                                           ║
╚═══════════════════════════════════════════════════════════╝
```

**Demonstrace:**
Ukaž, jak vypadá přihlášení s 2FA (screenshot nebo demo účet).

---

### 4. Reflexe: Můj bezpečnostní plán (10 min)

#### Osobní audit

```
MŮJ BEZPEČNOSTNÍ AUDIT

□ Mám různá hesla pro různé účty?
  Pokud ne, které účty jsou nejdůležitější k změně?
  ___________________________________________________

□ Mám zapnuté 2FA na důležitých účtech?
  • Email: □ Ano □ Ne □ Nevím
  • Sociální sítě: □ Ano □ Ne □ Nevím
  • Hry: □ Ano □ Ne □ Nevím

□ Znám někoho, kdo používá "heslo123"?
  Jak bych mu/jí pomohl/a?
  ___________________________________________________
```

#### Akční plán

```
DO PŘÍŠTÍHO TÝDNE:

1. Změním heslo na: _________________________________
2. Zapnu 2FA na: ___________________________________
3. Promluvím o bezpečnosti s: ______________________
```

---

## Správce hesel - Bonus

### Proč správce hesel?

```
PROBLÉM:
• 50+ účtů = 50+ různých hesel?
• Nikdo si tolik nezapamatuje

ŘEŠENÍ: SPRÁVCE HESEL
• Jeden "master" password
• Generuje silná hesla
• Pamatuje je za tebe
• Synchronizuje mezi zařízeními

PŘÍKLADY:
• Bitwarden (zdarma, open-source)
• 1Password
• LastPass
• Správce v prohlížeči (Chrome, Firefox)
```

---

## Materiály k tisku

### Karty s hesly k hodnocení
```
┌─────────────────────┐  ┌─────────────────────┐
│                     │  │                     │
│    martin2010       │  │    P@ssw0rd!        │
│                     │  │                     │
│  Hodnocení: ___/5   │  │  Hodnocení: ___/5   │
└─────────────────────┘  └─────────────────────┘

┌─────────────────────┐  ┌─────────────────────┐
│                     │  │                     │
│   K0l@č-Str0m-7!    │  │  heslo              │
│                     │  │                     │
│  Hodnocení: ___/5   │  │  Hodnocení: ___/5   │
└─────────────────────┘  └─────────────────────┘

┌─────────────────────┐  ┌─────────────────────┐
│                     │  │                     │
│    qwertyuiop       │  │ správně-kůň-baterie │
│                     │  │                     │
│  Hodnocení: ___/5   │  │  Hodnocení: ___/5   │
└─────────────────────┘  └─────────────────────┘
```

---

## Poznámky pro facilitátora

### Bezpečnostní upozornění
- **NIKDY** nežádej skutečná hesla dětí
- Cvičení jsou na strukturu, ne na reálné použití
- Zdůrazni, že si nová hesla tvoří doma soukromě

### Diferenciace
- **Začátečníci:** Fokus na délku a základní pravidla
- **Pokročilí:** Správce hesel, různé typy 2FA

### Propojení s domovem
- Navrhni rodinný "security audit"
- Sdílej zdroje pro rodiče

### Možné otázky
- "Co když zapomenu heslo?" → Reset, bezpečnostní otázky
- "Je SMS 2FA bezpečné?" → Lepší než nic, aplikace je lepší
- "Můžu mít jedno heslo pro všechno?" → Ne, ukradne jedno = ukradne vše

---

## Hodnocení

### Pozorování
- [ ] Rozumí konceptu silného hesla
- [ ] Umí použít metodu passphrase
- [ ] Chápe účel 2FA

### Výstup
- Pracovní list s cvičným heslem (ne skutečným!)
- Akční plán pro zlepšení bezpečnosti

---

**Verze:** 1.0.0
**Datum vytvoření:** 2026-01-11
