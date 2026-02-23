# **Lecture 2: The Blast Furnace – Design, Construction, and Operation**

## **1. The Blast Furnace (BF) Overview**

The Blast Furnace is a massive **counter-current heat and mass exchanger**. It is a tall, refractory-lined shaft furnace where solid materials descend and hot gases ascend.

### **Classification by Size**

- **Giant Blast Furnaces**: Internal volume $4000 - 5000 \ m^3$.
    
- **Modern Large Furnaces**: Volume $2000 - 3000 \ m^3$.
    
- **Mini Blast Furnaces**: Volume $< 1000 \ m^3$.
    
- **Capacity**: A $4000 \ m^3$ furnace produces ~13,000 tonnes of hot metal per day.
    

---

## **2. Furnace Geometry and Construction (Board Work)**

The furnace is not a simple cylinder; its shape changes to accommodate the changing state of materials (solid $\to$ softening $\to$ liquid).

### **Schematic of the Blast Furnace Profile**

Plaintext

```
      [ Charging System ]       <-- Top (Throat)
             |   |
      /      |   |      \       <-- Stack / Shaft
     /       |   |       \      (Widening downwards to accommodate 
    /        |   |        \      thermal expansion of solids)
   |         |   |         |    <-- Belly (Widest Part)
    \        |   |        /     <-- Bosh (Tapering downwards as 
     \       |   |       /       materials melt/shrink)
      |      |   |      |
      |      |   |      |       <-- Hearth (Cylindrical)
      |______|___|______|
       /  \       /  \
  Tuyeres (Air)  Taphole (Metal/Slag)
```

### **Key Components & Dimensions**

1. **Height**: ~30–35 meters (Total structure height including foundation is much higher).
    
2. **Hearth Diameter**: ~12–15 meters (for large furnaces).
    
3. **Lining (Refractories)**:
    
    - **Upper Stack**: Resistance to abrasion (falling solids).
        
    - **Hearth**: Carbon-based refractories.
        
    - _Instructor Note_: Carbon lining is used in the hearth because the liquid iron is already saturated with carbon. Therefore, there is no chemical potential for the carbon lining to dissolve into the metal, ensuring long life.
        

---

## **3. The Counter-Current Principle**

The efficiency of the BF relies on the opposing flows of materials and energy.

### **A. Descending Solids (The Burden)**

- **Input (Charge)**: Iron Ore (Lumps, Sinters, Pellets), Coke, and Limestone (Flux).
    
- **Entry Temperature**: 298 K (Room Temp).
    
- **Mechanics**: Solids descend due to gravity as Coke is consumed at the bottom and liquids are tapped out.
    

### **B. Ascending Gases**

- **Input**: Pre-heated Air (Hot Blast) injected through **Tuyeres**.
    
- **Input Temperature**: ~1200 K (900°C–1200°C).
    
- **Combustion Zone (Raceway)**:
    
    - Reaction: $C + O_2 \to CO_2$ (Exothermic).
        
    - Followed immediately by: $C + CO_2 \to 2CO$ (Endothermic, but overall region is hot).
        
    - **Peak Temperature**: ~1900°C – 2000°C.
        
    - _Note_: At this temp, $CO$ is the stable phase (Referencing Ellingham Diagram principles), not $CO_2$.
        
- **Exit**: The gas cools as it rises, transferring heat to the solids.
    
- **Top Gas (Off-gas) Temperature**: ~200°C – 300°C (Modern efficient furnaces).
    

---

## **4. Internal Zones and Phenomena**

### **The Raceway**

- Located directly in front of the tuyeres.
    
- The force of the hot air creates a physical "void" or cavity amidst the solid coke.
    
- This is the primary heat generation zone.
    

### **The Deadman**

- **Location**: The central core of the hearth.
    
- **Composition**: A pile of unreacted, solid Coke sitting in the liquid iron/slag pool.
    
- **Reason**: The air blast cannot penetrate all the way to the center of a 15m diameter furnace.
    
- **Role**: It is structurally important; liquid iron trickles through this porous coke bed.
    

### **The Cohesive Zone (Implied)**

- The region where solid iron/slag softens and starts dripping. The coke remains solid (it does not melt at 2000°C).
    

---

## **5. Auxiliary Systems (The "Satellites")**

A Blast Furnace cannot operate alone. It requires an extensive network of supporting plants.

### **A. Hot Blast Stoves (Cowper Stoves)**

- **Purpose**: To preheat the air blast to ~1200°C.
    
- **Structure**: Tall domes (as tall as the BF itself) filled with **Checker Bricks** (Ceramic heat absorbers).
    
- **Operation (Cyclic)**:
    
    1. **On-Gas Mode**: Clean BF gas (CO-rich) is burned inside the stove to heat the bricks.
        
    2. **On-Blast Mode**: Cold air is blown _backwards_ through the hot bricks to absorb heat before entering the BF.
        
    3. **Redundancy**: A BF needs at least 2 (usually 3-4) stoves to ensure continuous hot air supply.
        

### **B. Gas Cleaning Plant (GCP)**

The top gas leaves laden with dust (~200 tonnes/day for a large BF) and toxic CO. It must be cleaned before being reused as fuel.

**Cleaning Stages:**

1. **Dust Catcher**:
    
    - _Principle_: Expansion chamber. Gas velocity drops $\to$ Direction reverses $\to$ Heavy particles fall due to gravity.
        
    - _Efficiency_: Removes 70–90% of coarse dust.
        
2. **Venturi Scrubber (Wet Cleaning)**:
    
    - _Principle_: High-velocity gas mixes with water spray. Dust particles absorb moisture, become heavy, and settle as slurry.
        
3. **Electrostatic Precipitator (ESP)**:
    
    - _Principle_: Uses charged plates to attract fine dust particles.
        

_Instructor Note_: Modern plants prefer **Dry Gas Cleaning** over Wet Scrubbers to preserve the "Sensible Heat" (temperature) of the gas for better energy efficiency.

### **C. Charging System (The Top)**

- **Challenge**: Must dump tonnes of solid rock into the furnace while sealing in high-pressure toxic gas (1.5 – 2.5 atm top pressure).
    
- **Mechanism**: Bell-less top or Bell systems (complex seals).
    
- **Distribution**: It is critical to distribute Ore and Coke layers evenly to ensure **Uniform Permeability**.
    
    - _Permeability_: The ability of gas to flow through the voids between solids. If the burden "crashes" or generates fines, the gas path is blocked, and the furnace "chokes."
        

---

## **6. Instructor Notes & Remarks**

- **Engineered Materials**: We no longer just dump raw iron ore. We use **Sinter** and **Pellets** (Engineered Iron) to guarantee specific strength, porosity, and reducibility.
    
- **Coke vs. Coal**: We cannot use raw coal in the BF. It contains volatiles and lacks the mechanical strength to support the massive weight of the burden column. Coke is strong and porous.
    
- **The "Iron Making" vs. "Steel Making" Distinction**:
    
    - **BF Output**: "Hot Metal" or Pig Iron ($~94\% Fe, 4\% C, 1\% Si/Mn$). It is brittle and not useful for engineering yet.
        
    - **Steel Making**: The process of _refining_ this Hot Metal (removing C, Si, Mn) to produce Steel.
        
- **Slag Management**: Slag is waste (oxides of Si, Al, Ca). Quenching it wastes heat. Modern research focuses on heat recovery from slag.
    

### **Summary of Important Reactions (Verbal & Board)**

1. **Combustion (Heat Source)**: $C + O_2 \to CO_2 + Heat$
    
2. **Gas Generation (Reductant Source)**: $C + CO_2 \to 2CO$ (Boudouard Reaction)
    
3. **Reduction (Iron Production)**: $Fe_xO_y + CO \to Fe + CO_2$
    
