```mermaid
---
config:
  layout: elk
---

graph TD
    %% --- RAW MATERIALS ---
    Coal(Coal)
    Ore(Iron Ore)
    Flux(Limestone / Flux)
    Scraps(Scraps)

    %% --- INTERMEDIATES ---
    Coke(Coke)
    Separation((Separation <br/> Density Sorting))
    Pig(Pig Iron)
    Slag(Slag)
    
    %% --- FINAL PRODUCTS ---
    Cast(Cast Iron)
    Steel(Standard Steel)
    Alloy(Alloy / Special Steels)
    Cement(Cement & Road Materials)

    %% --- PROCESS FLOW ---

    %% 1. Fuel Preparation
    Coal -->|Coke Ovens| Coke

    %% 2. The Blast Furnace
    %% Inputs mixed into the "Charge"
    Ore --> CombineBF
    Coke --> CombineBF
    Flux --> CombineBF
    
    %% The Reaction happens on this line
    CombineBF -->|Blast Furnace Smelting| Separation

    %% 3. The Separation (The Node you requested)
    %% Physics does the work here
    Separation -->|Bottom Tap / Heavy| Pig
    Separation -->|Top Skim / Light| Slag

    %% 4. Waste Processing
    Slag -->|Crushing & Rapid Cooling| Cement

    %% 5. Iron Processing
    Pig -->|Solidification| Cast
    
    %% 6. Steel Production (Integral & Secondary)
    Pig --> CombineBOF
    Scraps --> CombineBOF
    CombineBOF -->|BOF Converter| Steel

    %% 7. Direct Production (High Tech)
    Scraps -->|Electric Arc Furnace| Alloy

    %% --- STYLING ---
    classDef raw fill:#e1f5fe,stroke:#01579b,stroke-width:2px;
    classDef inter fill:#fff9c4,stroke:#fbc02d,stroke-width:2px;
    classDef final fill:#e8f5e9,stroke:#2e7d32,stroke-width:4px;
    classDef waste fill:#e0e0e0,stroke:#616161,stroke-width:2px,stroke-dasharray: 5 5;
    classDef node fill:#ffe0b2,stroke:#ef6c00,stroke-width:2px,shape:circle;
    
    class Coal,Ore,Scraps,Flux raw;
    class Coke,Pig inter;
    class Cast,Steel,Alloy,Cement final;
    class Slag waste;
    Separation@{shape: f-circ, label: "Separate"};

    %% Combination Nodes
    CombineBF@{ shape: framed-circle, label: "Burden Mix" }
    CombineBOF@{ shape: framed-circle, label: "Charge Mix" }
```

**BOF = Basic Oxygen Furnace** — a structure that heats up carbon-rich pig iron (4-5%) with the presence of a lot of oxygen, allowing carbon to burn off.