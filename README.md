# Life Skills Education — kurikulum a QuestForge

> **Vzdělávací materiály a herní systém pro rozvoj metadovedností u dětí 11–13 let.**
> Quest-based learning s AI průvodcem (Claude Code), Cognitive Mirror princip, kurikulum 8 modulů.

---

## Co tady najdete

Tento repozitář obsahuje **dva spolu související projekty**:

### 1. Kurikulum metadovedností (`curriculum/`)
Komplexní vzdělávací materiály pro 8 oblastí, které dnešní děti potřebují připravit na budoucnost:

| Modul | Co rozvíjí |
|-------|-----------|
| **Metakognice** | Přemýšlení o vlastním myšlení, učební strategie |
| **Kritické myšlení** | Analýza argumentů, logické klamy, ověřování |
| **Emoční inteligence** | Rozpoznání emocí, empatie, regulace |
| **Finanční gramotnost** | Rozpočty, rozhodování, spoření |
| **Informační gramotnost** | SIFT metoda, dezinformace, hodnocení zdrojů |
| **Digitální gramotnost** | Kybernetická bezpečnost, AI literacy |
| **Komunikace a spolupráce** | Naslouchání, asertivita, týmová práce |
| **Adaptabilita a rezilience** | Růstové myšlení, zvládání změn |

Každý modul má: facilitátorský průvodce, 5 aktivit, student workbook, AI scripty, hodnocení a tištěné materiály (`printables/`).

### 2. QuestForge plugin (`commands/`, `skills/`, `agents/`)
Plugin pro [Claude Code](https://github.com/zdenekmach/cli_starter_pack), který orchestruje **quest-based learning**: děti se učí tím, že plní mise v příběhovém světě, ne tím, že sedí nad učebnicí.

**Tři příkazy:**
- `/prep` — rodič připraví session (Claude vygeneruje quest z kurikula)
- `/quest` — spustí Quest Master agenta, který vede session s dětmi
- `/progress` — přehled stavu postav a misí

**Jeden agent:**
- **Quest Master** — NPC průvodce, drží Cognitive Mirror princip (nikdy nedává přímé odpovědi, vždy klade otázky)

---

## Pro koho je to určeno

- **Rodiče**, kteří chtějí doma s dětmi pracovat na metadovednostech a hledají strukturu, ne improvizaci.
- **Učitelé** v alternativních školách, doma vzdělávajících rodičů, kroužcích.
- **Facilitátory** vzdělávacích aktivit pro děti 11–13 let.

**Předpoklady:**
- Základní orientace v terminálu (instalace Claude Code — viz [návod](https://github.com/zdenekmach/cli_starter_pack))
- Účet u Anthropic / API klíč pro Claude
- Ochota investovat čas do přípravy první kampaně (cca 2–4 hodiny pro vlastní svět)

---

## Jak začít

1. **Naklonujte tento repozitář:**
   ```bash
   git clone https://github.com/zdenekmach/Life-skills-education.git
   cd Life-skills-education
   ```

2. **Nainstalujte Claude Code** (pokud ještě nemáte):
   - Návod: [zdenekmach/cli_starter_pack](https://github.com/zdenekmach/cli_starter_pack)
   - Plus API klíč od [Anthropic](https://console.anthropic.com/)

3. **Spusťte Claude Code v adresáři projektu:**
   ```bash
   claude
   ```
   Plugin QuestForge se automaticky načte (rozpozná `.claude-plugin/`).

4. **Vytvořte si první kampaň** — viz [`campaign/README.md`](campaign/README.md) pro inspiraci a krok-za-krokem návod.

5. **Spusťte první session:**
   ```
   /prep
   ```
   pak
   ```
   /quest
   ```

Detailní pokyny viz [`INSTALL.md`](INSTALL.md).

---

## Struktura repozitáře

```
Life-skills-education/
├── README.md                  ← jste tady
├── INSTALL.md                 ← detailní instalace + první kroky
├── LICENSE                    ← MIT
│
├── .claude-plugin/            ← QuestForge plugin manifest
├── commands/                  ← /prep, /quest, /progress
├── skills/questforge/         ← QuestForge SKILL + templates
├── agents/                    ← Quest Master NPC agent
│
├── campaign/                  ← VAŠE kampaň (template, žádný předgenerovaný obsah)
│   ├── README.md              ← jak si vytvořit svět + 3 inspirační příklady
│   ├── world-template.md      ← šablona příběhového světa
│   ├── characters/            ← character sheets operátorů
│   ├── puzzles/               ← hádanky per session
│   └── sessions/              ← facilitátorské plány
│
├── curriculum/                ← 8 modulů + domain model
│   ├── README.md              ← přehled kurikula
│   ├── ATTRIBUTION.md         ← zdroje a inspirace
│   ├── domain/                ← model.yaml, glossary, concept-map
│   └── <modul>/               ← facilitator-guide, activities, workbook, ai-scripts, assessment, resources
│
├── research/                  ← vědecké podklady (21st century skills, finská škola, cognitive mirror, gamifikace)
├── printables/                ← DOCX pracovní listy, kartičky, postery
├── training/                  ← workshop pro rodiče/učitele (1 den)
├── guides/                    ← parent study guide
└── docs/                      ← přehledy: meta-skills overview, QuestForge for parents
```

---

## Filozofie a principy

### Cognitive Mirror

> **AI nikdy nedává přímé odpovědi.** Místo "správná odpověď je X" klade otázky: "Co myslíš ty? Proč si to myslíš? Z čeho to vyvozuješ?"

Tento princip se táhne celým systémem — kurikulárními aktivitami, AI scripty pro modulové činnosti i Quest Master agentem. Důvod: výzkumy ukazují, že odpovědi, ke kterým dítě dojde samo, si pamatuje výrazně lépe, než ty, které mu někdo řekne.

### Kurikulum na pozadí

Děti nevidí strukturu kurikula. Nevidí "Modul 3: Informační gramotnost, Aktivita 2". Vidí příběh, postavu, výzvu. Za ní stojí explicitně mapované cíle — pro rodiče v `campaign/sessions/session-NNN-plan.md`, pro děti neviditelné.

### Kombinace fyzického a digitálního

Quest Master vede dialog v Claude Code, ale úkoly děti řeší fyzicky: papírové šifry, mikroskop, micro:bit, dalekohled, hra v terénu. Jen čistě digitální učení by bylo proti smyslu projektu.

### Bezpečnost dětí

- Operátoři vystupují **pod fiktivními jmény** (chrání soukromí, posiluje vžití do role).
- Žádné osobní informace o dětech v záznamech / character sheetech.
- Hrozby v příběhu = intelektuální výzvy, ne fyzické nebezpečí.

---

## Status projektu

> **EXPERIMENT & WORK IN PROGRESS** — tento systém je osobní projekt ve fázi vývoje a pilotního testování. Není to certifikovaný vzdělávací materiál ani hotový produkt. Používejte na vlastní uvážení a přizpůsobte svým dětem.

Zpětná vazba je vítaná — pokud něco nefunguje, něco vás napadne, narazíte na chybu nebo máte otázky, **napište mi**.

---

## Licence a autorství

- **Licence:** [MIT](LICENSE)
- **Autor:** Zdeněk Macháček, 2026
- **Inspirace a zdroje:** viz [`curriculum/ATTRIBUTION.md`](curriculum/ATTRIBUTION.md)

---

## Další čtení

- [`docs/meta-skills-education-overview.md`](docs/meta-skills-education-overview.md) — kompletní přehled vzdělávacího přístupu
- [`docs/questforge-overview-for-parents.md`](docs/questforge-overview-for-parents.md) — QuestForge pro rodiče (čte se nejdřív)
- [`research/2026-01-08-cognitive-mirror-framework.md`](research/2026-01-08-cognitive-mirror-framework.md) — teoretický základ Cognitive Mirror
- [`research/2026-03-04-quest-narrative-gamification-education.md`](research/2026-03-04-quest-narrative-gamification-education.md) — proč quest-based learning funguje
