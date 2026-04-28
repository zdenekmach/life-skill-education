# Instalace a první kroky

> Návod od nuly k první quest session — pro rodiče bez technické zkušenosti.

---

## Krok 1 — Předpoklady

Potřebujete:

1. **Počítač** (Mac, Linux, nebo Windows s WSL2)
2. **Claude Code** nainstalovaný a přihlášený
   - **Pokud Claude Code ještě nemáte**: následujte [návod v repu cli_starter_pack](https://github.com/zdenekmach/cli_starter_pack) — provede vás instalací a přihlášením.
3. **Git** (na Macu obvykle už je; jinak `xcode-select --install` nebo balík od [git-scm.com](https://git-scm.com/))

> **Kontrola:** v terminálu napište `claude --version`. Pokud uvidíte verzi (např. `claude 1.x.x`), máte hotovo. Pokud ne, vraťte se k instalaci.

---

## Krok 2 — Stažení projektu

Otevřete terminál a vyberte si adresář, kde chcete projekt mít. Doporučuji vyhradit si pro to vlastní složku, např. `~/Projects/`:

```bash
mkdir -p ~/Projects && cd ~/Projects
git clone https://github.com/zdenekmach/Life-skills-education.git
cd Life-skills-education
```

Po stažení by `ls` mělo zobrazit strukturu:

```
README.md  INSTALL.md  LICENSE
.claude-plugin/  commands/  skills/  agents/
campaign/  curriculum/  research/  printables/  training/  guides/  docs/
```

---

## Krok 3 — Spuštění Claude Code v projektu

V adresáři projektu spusťte:

```bash
claude
```

Při prvním spuštění Claude Code v tomto adresáři vám pravděpodobně **nabídne aktivaci pluginu QuestForge**. Potvrďte. Plugin se načte z `.claude-plugin/` a `commands/`, `skills/`, `agents/` budou dostupné.

> **Ověření:** napište do Claude Code `/help` a v seznamu by měly být `prep`, `quest`, `progress`. Pokud tam nejsou, restartujte Claude Code a zkontrolujte, že jste v adresáři `Life-skills-education`.

### Alternativa — instalace přes plugin marketplace

Pokud chcete plugin používat z **jiného** adresáře (např. máte vlastní projekt vedle), můžete ho nainstalovat jako plugin do Claude Code:

```bash
# z adresáře Life-skills-education
claude
> /plugin marketplace add .
> /plugin install questforge
```

Pak se `/prep`, `/quest`, `/progress` načtou globálně.

> Pro 99 % případů stačí varianta z Kroku 3 — pracujte přímo v adresáři projektu, vše se načte automaticky.

---

## Krok 4 — Vytvoření vlastní kampaně

QuestForge nemá předgenerovanou kampaň — každá rodina si tvoří vlastní svět. Otevřete [`campaign/README.md`](campaign/README.md) a projděte si:

- **3 inspirační příklady** (vesmírná stanice, magická knihovna, detektivní agentura)
- **Krok-za-krokem návod** jak si vytvořit vlastní `world.md`

**Minimum pro start:**
1. Vytvořte `campaign/world.md` (stačí 2–3 lokace a krátký popis Orákula — jméno NPC průvodce a jeho tón).
2. To je vše. Postavy se vytvoří během první session.

> **Tip:** Pokud nechcete strávit hodiny psaním světa, **požádejte Claude Code o pomoc**: "Pomoz mi vytvořit `campaign/world.md` pro [vesmír / fantasy / detektivku] — máme 2 děti ve věku 11 a 13. Použij šablonu z `campaign/world-template.md`." Claude vygeneruje návrh, který upravíte.

---

## Krok 5 — První session

V Claude Code v adresáři projektu spusťte:

```
/prep
```

Claude:
1. Načte `campaign/world.md` a kurikulum
2. Vybere 2–4 aktivity z různých modulů
3. Vygeneruje první quest — `campaign/active-quest.md`
4. Připraví facilitátorský plán — `campaign/sessions/session-001-plan.md`
5. Případně hádanky — `campaign/puzzles/session-001/`
6. Vám dá checklist (co vytisknout, co fyzicky připravit)

Projděte si plán, vytiskněte materiály, nachystejte props.

Až budou děti připravené, spusťte:

```
/quest
```

Claude Code přepne do role **Quest Master** — agenta, který drží roli Orákula, vede děti misí a po skončení automaticky aktualizuje záznamy.

---

## Krok 6 — Po session

Quest Master automaticky uloží:
- Dokončený quest do `campaign/quest-log.md`
- XP a poznámky do character sheetů v `campaign/characters/`
- Status aktivního questu

Pomocí `/progress` zobrazíte přehled:

```
/progress
```

---

## Časté otázky

### Kolik to stojí

Záleží na tom, jak je Claude Code přihlášený:
- **Claude Pro / Max předplatné** — fixní měsíční cena, žádné per-session náklady (pro běžné rodinné používání obvykle stačí Pro plán).
- **Anthropic API klíč (pay-as-you-go)** — jedna session (~90 min) typicky spotřebuje **0,50–2 USD** podle množství textu a délky dialogu. Příprava session přes `/prep` cca **0,20–0,80 USD**.

### Kolik to zabere času rodiči

- **Setup repa + prvního světa:** 1–3 hodiny (jednorázově)
- **Příprava session přes `/prep`:** 5–15 minut (Claude udělá většinu práce, rodič projde plán)
- **Fyzická příprava:** 15–30 minut (tisk, props)
- **Samotná session:** 60–120 minut (Quest Master vede, rodič facilituje)
- **Po session:** 0 minut (vše se aktualizuje automaticky)

### Pro jaký věk je to vhodné

Cílová skupina je **11–13 let**. Některé aktivity zvládnou i 9–10leté děti, některé budou vhodné i pro 14–15leté. Hodně záleží na konkrétním dítěti.

### Co když dítě "prokoukne" že se učí

To je v pořádku. Cognitive Mirror princip funguje, i když dítě ví, že je to vzdělávací aktivita — pokud Quest Master zachovává roli a otázky jsou autenticky zajímavé, dítě je vtažené do příběhu, ne do "učení".

### Můžu si projekt přizpůsobit

Ano. Vše je open-source pod MIT. Forknete repo, upravujete kurikulum, měníte princip Quest Mastera, přidáváte vlastní moduly. Pokud uděláte něco zajímavého a chcete sdílet — pull request je vítaný.

### Co dělat, když něco nefunguje

1. Zkontrolujte, že jste v adresáři `Life-skills-education` (`pwd`).
2. Zkontrolujte, že Claude Code vidí plugin (`/help` musí ukazovat `prep`, `quest`, `progress`).
3. Pokud `/prep` nezná stav kampaně: ověřte, že existuje `campaign/world.md`.
4. Pokud Quest Master neodpovídá v charakteru: zkontrolujte, že `agents/quest-master.md` existuje a `campaign/active-quest.md` je vytvořený.
5. Pokud nic z toho nepomohlo: napište mi.

---

## Co dál

- Přečtěte si [`docs/questforge-overview-for-parents.md`](docs/questforge-overview-for-parents.md) — širší kontext, jak to funguje a proč.
- Projděte si [`curriculum/README.md`](curriculum/README.md) — co všechno máte k dispozici v 8 modulech.
- Otevřete jeden modul (např. [`curriculum/kriticke-mysleni/`](curriculum/kriticke-mysleni/)) a podívejte se na facilitator-guide a aktivity — to vám dá pocit, jaké úkoly se objeví ve vašich questech.
