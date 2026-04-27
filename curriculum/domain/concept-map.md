---
type: note
title: "Konceptuální mapa: Meta-dovednosti pro děti 11-13 let"
project: life-skills-education
created: 2026-01-19
---
# Konceptuální mapa: Meta-dovednosti pro děti 11-13 let

**Verze:** 1.0.0
**Datum:** 2026-01-08

---

## Hlavní konceptuální mapa

```mermaid
graph TB
    subgraph Users["👤 AKTÉŘI"]
        CHILD["🧒 Dítě<br/>(11-13 let)"]
        PARENT["👨‍👩‍👧 Rodič"]
        TEACHER["👩‍🏫 Učitel"]
    end

    subgraph Core["🎯 META-DOVEDNOSTI (Core)"]
        MS["Meta-dovednosti"]
        META["Metakognice"]
        EF["Exekutivní funkce"]
        CT["Kritické myšlení"]
        L2L["Učení se učit"]
        EI["Emocionální inteligence"]
        SR["Seberegulace"]
        CC["Komunikace & spolupráce"]
        DL["Digitální gramotnost"]
    end

    subgraph Frameworks["📋 FRAMEWORKY"]
        CASEL["CASEL<br/>(5 SEL kompetencí)"]
        P21["P21 / 4Cs"]
        FIN["Finské T1-T7"]
        OECD["OECD Learning Compass"]
    end

    subgraph Methods["🔧 METODY"]
        PHBL["Phenomenon-based<br/>Learning"]
        SOCR["Sokratovská metoda"]
        PBL["Problem-based<br/>Learning"]
        SCAFF["Metakognitivní<br/>scaffolding"]
    end

    subgraph AI["🤖 AI STRATEGIE"]
        CM["Cognitive Mirror<br/>Framework"]
        TQI["Teaching Quality<br/>Index (M0-M3)"]
        PROT["Protégé efekt"]
        ARP["AI Reflection<br/>Partner"]
    end

    subgraph Risks["⚠️ RIZIKA"]
        OFFL["Cognitive<br/>Offloading"]
    end

    %% User relationships
    CHILD --> MS
    PARENT -->|facilituje| CHILD
    TEACHER -->|facilituje| CHILD
    CHILD -->|používá| ARP

    %% Meta-skills hierarchy
    MS --> META
    MS --> EF
    MS --> CT
    MS --> L2L
    MS --> EI
    MS --> SR
    MS --> CC
    MS --> DL

    %% Inter-skill relationships
    META -.->|prerekvizita| L2L
    EF -.->|podporuje| SR
    EI -.->|podporuje| SR
    CT -.->|podporuje| DL

    %% Framework mappings
    CASEL -->|definuje| EI
    P21 -->|obsahuje| CT
    P21 -->|obsahuje| CC
    FIN -->|T1| L2L
    FIN -->|T5| DL
    OECD -->|podporuje| MS

    %% Methods develop skills
    PHBL -->|rozvíjí| MS
    SOCR -->|rozvíjí| CT
    SOCR -->|rozvíjí| META
    PBL -->|rozvíjí| CT
    SCAFF -->|rozvíjí| META

    %% AI relationships
    CM -->|implementuje| PROT
    CM -->|obsahuje| TQI
    CM -->|rozvíjí| META
    CM -->|mitiguje| OFFL
    ARP -->|implementuje| CM
    ARP -->|cílí na| CHILD

    %% Styling
    classDef core fill:#e1f5fe,stroke:#01579b
    classDef framework fill:#f3e5f5,stroke:#4a148c
    classDef method fill:#e8f5e9,stroke:#1b5e20
    classDef ai fill:#fff3e0,stroke:#e65100
    classDef risk fill:#ffebee,stroke:#b71c1c
    classDef user fill:#fce4ec,stroke:#880e4f

    class MS,META,EF,CT,L2L,EI,SR,CC,DL core
    class CASEL,P21,FIN,OECD framework
    class PHBL,SOCR,PBL,SCAFF method
    class CM,TQI,PROT,ARP ai
    class OFFL risk
    class CHILD,PARENT,TEACHER user
```

---

## Cognitive Mirror Framework Detail

```mermaid
flowchart LR
    subgraph Cycle["COGNITIVE MIRROR CYKLUS"]
        direction TB
        P["1. PRESENT<br/>Student vysvětluje"]
        Q["2. QUERY<br/>AI pokládá otázky"]
        R["3. REFLECT<br/>Kvalita = zrcadlo"]
        F["4. REFINE<br/>Student opravuje"]

        P --> Q --> R --> F --> P
    end

    subgraph Modes["TQI MÓDY"]
        M0["M0: Zmatené<br/>přeformulování"]
        M1["M1: Objasňující<br/>sonda"]
        M2["M2: Sokratovská<br/>mezera"]
        M3["M3: Přesná<br/>reformulace"]
    end

    subgraph Design["DESIGN PRINCIPY"]
        D1["❌ Answer Machine"]
        D2["✅ Cognitive Mirror"]
        D3["❌ Cognitive Offloading"]
        D4["✅ Active Engagement"]
    end

    R -->|nízká kvalita| M0
    R -->|částečná| M1
    R -->|dobrá| M2
    R -->|výborná| M3

    D2 -.-> Cycle
    D4 -.-> Cycle

    style M0 fill:#ffcdd2
    style M1 fill:#ffe0b2
    style M2 fill:#fff9c4
    style M3 fill:#c8e6c9
    style D1 fill:#ffcdd2
    style D3 fill:#ffcdd2
    style D2 fill:#c8e6c9
    style D4 fill:#c8e6c9
```

---

## Hierarchie meta-dovedností

```mermaid
graph TD
    MS["META-DOVEDNOSTI"]

    subgraph Cognitive["🧠 Kognitivní"]
        META["Metakognice"]
        EF["Exekutivní funkce"]
        CT["Kritické myšlení"]
        L2L["Učení se učit"]
    end

    subgraph SocioEmotional["❤️ Sociálně-emocionální"]
        EI["Emocionální inteligence"]
        SR["Seberegulace"]
        CC["Komunikace & spolupráce"]
    end

    subgraph Digital["💻 Digitální"]
        DL["Digitální gramotnost"]
        AIL["AI gramotnost"]
    end

    MS --> Cognitive
    MS --> SocioEmotional
    MS --> Digital

    META --> L2L
    EF --> SR
    EI --> SR
    CT --> DL
    DL --> AIL

    classDef cognitive fill:#e3f2fd,stroke:#1565c0
    classDef socio fill:#fce4ec,stroke:#c2185b
    classDef digital fill:#f3e5f5,stroke:#7b1fa2

    class META,EF,CT,L2L cognitive
    class EI,SR,CC socio
    class DL,AIL digital
```

---

## Mapování frameworků

```mermaid
graph LR
    subgraph Dovednost["META-DOVEDNOST"]
        CT["Kritické<br/>myšlení"]
        CR["Kreativita"]
        CO["Spolupráce"]
        CM["Komunikace"]
        L2L["Učení se<br/>učit"]
        DL["Digitální<br/>gramotnost"]
        EI["Emocionální<br/>inteligence"]
        AD["Adaptabilita"]
    end

    subgraph Framework["FRAMEWORK"]
        P21["P21<br/>4Cs"]
        CASEL["CASEL<br/>SEL"]
        FIN["Finské<br/>T1-T7"]
        OECD["OECD<br/>2030"]
        WEF["WEF<br/>2025"]
    end

    %% P21 mappings
    P21 -->|✓| CT
    P21 -->|✓| CR
    P21 -->|✓| CO
    P21 -->|✓| CM

    %% CASEL mappings
    CASEL -->|✓| EI
    CASEL -->|✓| CO

    %% Finnish mappings
    FIN -->|T1| L2L
    FIN -->|T5| DL
    FIN -->|T2| CM

    %% OECD mappings
    OECD -->|✓| CT
    OECD -->|✓| AD
    OECD -->|✓| L2L

    %% WEF mappings
    WEF -->|✓| CT
    WEF -->|✓| AD
    WEF -->|✓| DL

    classDef tier1 fill:#c8e6c9,stroke:#2e7d32
    class CT,CR,CO,CM,L2L,DL tier1
```

---

## Produkt Roadmap

```mermaid
gantt
    title AI Meta-Skills Product Roadmap
    dateFormat  YYYY-MM

    section Phase 1 - Research
    Studium CM Framework       :2026-01, 1M
    Design principles          :2026-02, 1M
    Tech spike Claude API      :2026-03, 1M

    section Phase 2 - Prototype
    AI Reflection Partner v1   :2026-04, 2M
    Workshop integrace         :2026-05, 1M

    section Phase 3 - Pilot
    Rekrutace 20 rodin         :2026-07, 1M
    Pilot test                 :2026-08, 2M

    section Phase 4 - Refine
    Iterace designu            :2026-10, 2M
    B2B verze                  :2026-11, 1M

    section Phase 5 - Launch
    B2C Launch                 :2027-01, 1M
    B2B Launch                 :2027-02, 1M
```

---

## Aktéři a jejich interakce

```mermaid
sequenceDiagram
    participant C as 🧒 Dítě
    participant AI as 🤖 AI Reflection Partner
    participant P as 👨‍👩‍👧 Rodič

    Note over C,P: Cognitive Mirror cyklus

    C->>AI: Vysvětluje koncept
    AI->>C: Pokládá upřesňující otázky (M1-M2)
    C->>AI: Zlepšuje vysvětlení
    AI->>C: Zrcadlí kvalitu (TQI)

    AI-->>P: Dashboard: přehled interakcí
    P->>C: Facilituje reflexi

    Note over C: Metakognice se rozvíjí
```

---

## Legenda

| Symbol | Význam |
|--------|--------|
| 🧒 | Dítě (primární uživatel) |
| 👨‍👩‍👧 | Rodič/Vychovatel |
| 👩‍🏫 | Učitel |
| 🤖 | AI asistent |
| 🎯 | Core dovednosti |
| 📋 | Framework |
| 🔧 | Metoda |
| ⚠️ | Riziko |
| ✅ | Doporučený přístup |
| ❌ | Anti-pattern |

---

*Konceptuální mapa vytvořena jako součást domain modelu projektu life-skills-education*
