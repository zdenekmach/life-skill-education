# Kampaň — co sem patří a jak ji vytvořit

Tento adresář je **prázdný úmyslně**. Každá rodina si tvoří vlastní kampaň: vlastní svět, vlastní postavy, vlastní příběh. Ukázkovou kampaň autora jsme do repa nezahrnuli — byla by lokální (vázaná na konkrétní děti) a brala by vám prostor k vlastní kreativitě.

---

## Co je kampaň

Kampaň = dlouhodobý herní svět, ve kterém se odehrávají jednotlivé questy (mise). Drží pohromadě:

- **Příběhový rámec** (`world.md`) — kde se to odehrává, kdo je Orákulum (NPC průvodce), jaká jsou pravidla, jaké lokace existují.
- **Postavy operátorů** (`characters/<jmeno>.md`) — jména, role, schopnosti, XP, deník.
- **Aktivní quest** (`active-quest.md`) — to, co se právě hraje.
- **Historie** (`quest-log.md`) — co už bylo dokončeno.
- **Sessions** (`sessions/`) — facilitátorské plány a flow taháky pro rodiče.
- **Hádanky** (`puzzles/session-NNN/`) — šifry, otázky, materiály per session.

---

## Jak by mohla kampaň vypadat (inspirace)

### Příklad 1 — Vesmírná stanice

> Stanice **Nexus** je pradávná meziplanetární základna s vlastní inteligencí (**Orákulum**). Děti jsou operátoři, kteří létají na mise do vzdálených planetárních systémů (Kepler-7, Verdantis...). Každá planeta má vlastní výzvy — záhadné signály, krizi zásob, kontakt s neznámými životními formami.
>
> **Kurikulum schované jako:** dešifrování staničních logů (informační gramotnost), správa rozpočtu expedice (finanční gramotnost), katalogizace nálezů (vědecká metoda), komunikace s NPC (emoční inteligence).

### Příklad 2 — Magická knihovna

> **Knihovna Aletheia** je živé místo, kde se setkávají všechny příběhy a poznání světa. **Knihovník** (Orákulum) hledá pomoc — knihy se ztrácejí, příběhy se mění. Děti jsou mladí badatelé, kteří se musí vydat do jednotlivých příběhových světů a obnovit pořádek.
>
> **Kurikulum schované jako:** rozluštění starých textů (kritické myšlení), vyjednávání s postavami z příběhů (komunikace), volba mezi více verzemi pravdy (informační gramotnost).

### Příklad 3 — Detektivní agentura

> **Agentura Sentinel** přijímá nové vyšetřovatele. Klienti přicházejí s případy — od podvodu na bazaru přes záhadné zmizení až po dezinformační kampaň ve školních novinách. Každý případ vyžaduje sběr důkazů, analýzu a obhajobu řešení.
>
> **Kurikulum schované jako:** ověřování zdrojů (informační gramotnost), interview svědků (emoční inteligence), rekonstrukce financí (finanční gramotnost), prezentace závěrů (komunikace).

---

## Jak si svou kampaň vytvořit (krok za krokem)

### Krok 1 — Příběhový svět (`world.md`)

Vytvořte soubor `campaign/world.md`. Měl by obsahovat:

- **Setting** — kde se to odehrává? (vesmír / fantasy / současnost / historický)
- **Hub lokace** — odkud se vyráží na mise? (stanice, knihovna, agentura)
- **Orákulum** — kdo je průvodce? Jak mluví? Jaký má charakter?
- **Lokace/planety/světy** — seznam míst, kam mohou děti cestovat. Pro každé krátký popis a typické výzvy.
- **Pravidla XP** — kolik XP za quest, level thresholdy (např. L1: 0–100, L2: 100–250, L3: 250–500...).

**Tip:** Nemusíte mít všechno hotové na začátku. Stačí 2–3 lokace a první mise. Svět se přirozeně rozšíří během hraní.

### Krok 2 — Postavy operátorů

Spusťte první session pomocí `/quest`. Quest Master vás provede tvorbou postav (zeptá se na jméno, roli, 3 schopnosti, vybavení). Character sheety se uloží do `campaign/characters/<jmeno>.md` podle šablony v `skills/questforge/templates/character-template.md`.

**Pravidlo:** Děti si volí **fiktivní jména** (ne svá vlastní). To chrání jejich soukromí a podporuje vžití do role.

### Krok 3 — První quest

Spusťte `/prep` — Claude Code načte stav kampaně a vygeneruje první quest z kurikula. Výstup:

- `campaign/active-quest.md` — briefing pro děti
- `campaign/sessions/session-001-plan.md` — facilitátorský plán pro vás
- `campaign/puzzles/session-001/` — případné hádanky

Projděte si plán, případně upravte podle naladění dětí.

### Krok 4 — Hraní

Spusťte `/quest`. Quest Master přebírá konverzaci, hraje Orákulum a NPC, vede děti misí. Vy jako rodič facilitujete fyzicky (tisk, props, čas).

### Krok 5 — Po session

Quest Master automaticky aktualizuje `quest-log.md`, character sheets a status questu. Pomocí `/progress` zobrazíte přehled.

---

## Co je v `.gitignore`

Tento template repo má v `.gitignore` všechny soubory s aktivním obsahem kampaně:

- `campaign/active-quest.md`
- `campaign/quest-log.md`
- `campaign/sessions/*-plan.md`, `*-flow.md`
- `campaign/puzzles/session-*/`
- `campaign/SESSION-LEARNINGS.md`

Důvod: pokud byste repo někdy chtěli sdílet/forknout, vaše konkrétní kampaň (s jmény dětí, jejich silnými stránkami, deníky) by zůstala lokální. Pokud chcete commitovat svou kampaň do svého private forku, smažte odpovídající řádky v `.gitignore`.

---

## Šablony

V `skills/questforge/templates/` najdete:

- `character-template.md` — šablona postavy
- `quest-template.md` — šablona questu
- `session-plan.md` — šablona facilitátorského plánu

Quest Master a `/prep` z nich automaticky čerpají.
