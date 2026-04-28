# Lecture Notes: Ingot and Continuous Casting of Steel

## 1. Ingot Casting: Process Setup and Solidification

### Conceptual Explanation

The traditional ingot casting process is a batch operation where molten metal is fed into molds and allowed to solidify over several hours . Once mostly solidified, the mold is removed (a process known as stripping). The newly exposed red-hot ingot loses heat primarily via radiation. To prevent rapid cooling and the onset of severe thermal stresses, the ingot is sometimes covered with an insulating material like sand. Molds are never pre-heated because their primary purpose is to absorb heat; however, due to continuous recycling in the plant, molds are typically warm (e.g., 60–65°C) rather than at true room temperature [.

### Board Work: Solidification Kinetics

**Equation: Parabolic Rate Law for Solidification**

$$x = A + B\sqrt{t}$$

_Where:_

- $x$ = Distance of the solidification front from the mold wall (thickness of the solidified shell)
    
- $t$ = Time
    
- $A, B$ = Constants characteristic of the mold material and the specific solidification process .
    

### Board Work: Bottom-Pouring Setup Diagram



```
       [Ladle]
          |
          v
      [Trumpet]
          |
   -------+------- (Horizontal Runners)
   |             |
  [M1]          [M2]
  WEU           NEU
```

- **M1**: Wide End Up (WEU) Mold
    
- **M2**: Narrow End Up (NEU) Mold
    
- **Hot Top**: A specialized reservoir placed at the top of the mold.
    

### Physical Interpretation

The **Hot Top** is utilized to maintain a pool of liquid steel at the top of the ingot for a prolonged time . "Anti-piping compounds" (a mixture of aluminum and oxides) are added here; the exothermic reaction between these compounds provides sustained heat to keep the metal molten. This liquid pool continuously feeds the shrinkage cavity (pipe) forming below it. The hot top section is not accounted for in the ingot yield and is eventually discarded.

---

## 2. Classification of Ingots (Based on Deoxidation)

### Board Work: Ingot Types

- **Killed Ingot**: [O] lowest
    
- **Semi-Killed Ingot**
    
- **Rimming Ingot**: [O] highest 
    

### Conceptual Explanation

- **Killed Steel**: Deoxidized extensively, typically with Aluminum, leaving negligible dissolved oxygen (e.g., ~10 ppm)  Because there is no carbon-oxygen gas evolution to offset volumetric shrinkage, a deep primary pipe forms at the top (unless a hot top is used).
    
- **Semi-Killed Steel**: Contains intermediate residual oxygen levels. During solidification, carbon and oxygen are rejected into the liquid ahead of the solidification front. It is only after 70–80% of the ingot has solidified that the local concentrations cross the required threshold to initiate a Carbon-Oxygen reaction . This late-stage carbon monoxide (CO) bubble formation occurs deep inside the ingot, efficiently compensating for shrinkage. This is also called _ladle-balanced steel_.
    
- **Rimming Steel**: Low carbon and very high dissolved oxygen. CO bubbling (the "rimming" action) starts early, usually after ~10% solidification .
    
    - **Important Remarks / Instructor Notes**: The bubbles must be deep-seated so they do not oxidize during later rolling operations (oxidized bubbles will not weld shut). The rimming action is sustained by atmospheric oxygen reacting with ejected iron droplets. Rimming creates a very pure, soft, solid outer crust (the "rim"). It is highly specialized and extremely difficult to produce a rimming structure in a continuous casting machine .
        

---

## 3. Defects in Ingot Casting

### Board Work: Defect Categories

1. **Pipes** $\rightarrow$ Primary & Secondary pipes
    
2. **Inclusions** $\rightarrow$ Endogenous / Exogenous
    
3. **Blowholes & pinholes**
    
4. **Segregation** $\rightarrow$ +ve Segregation, -ve Segregation
    
5. **Cracks**
    

### Physical Interpretation

- **Pipes**: Massive shrinkage cavities. Primary pipes are eliminated via hot tops. Secondary pipes form deeper but are usually free of oxidation, meaning they will safely weld shut under the immense pressure of hot rolling .
    
- **Inclusions**:
    
    - _Endogenous_: Originate internally from deoxidation products (e.g., alumina) .
        
    - _Exogenous_: Originate externally. For example, sodium/potassium traces indicate entrapped mold powder; magnesium indicates eroded refractory materials from the runners or trumpet. These particles get trapped in the large mushy zone of the solidifying steel.
        
- **Blowholes & Pinholes**: Internal blowholes are manageable, but surface blowholes are major defects. Pinholes are an immediate indication of high hydrogen content, leaving the final steel highly susceptible to hydrogen embrittlement 
    
- **Segregation**:
    
    - _Micro-segregation_: A fundamental thermodynamic property of alloy solidification (the first metal to solidify is pure; the last to solidify is impure) 
        
    - _Macro-segregation_: Bulk compositional changes caused by violent fluid flow dislodging micro-segregated crystals.
        
        - **Negative Segregation**: Found at the bottom. High-purity crystals have a higher density and physically settle downward
            
        - **Positive Segregation**: Found at the upper parts. Impure, solute-rich liquid is lighter and naturally rises.
            

---

## 4. Continuous Casting of Steel

### Important Remarks / Instructor Notes

Continuous casting bypassed ingot casting largely due to the advent of the BOF (Basic Oxygen Furnace) . Ingot casting is a batch process that simply cannot match the massive turnover rates of a BOF. Furthermore, rolling massive 10-ton ingots into usable sheets is extremely energy-intensive. Switching to continuous casting saves between **200 to 500 Mega Joules per ton of steel** by producing "near net shapes" that require minimal subsequent hot working

### Board Work: Sections Produced

1. **Billets**: Square cross-section (e.g., $100\text{ mm} \times 100\text{ mm}$) .
    
2. **Blooms**: Larger rectangular/square sections (e.g., $250\text{ mm} \times 300\text{ mm}$).
    
3. **Slabs**: Wide rectangles (e.g., $200\text{-}250\text{ mm}$ thick, $1600\text{ mm}$ wide).
    
4. **Thin Slabs**: $50\text{ mm}$ thick.
    
5. **Strip**: $2\text{-}5\text{ mm}$ thick (revolutionary because it bypasses nearly all hot working).
    

### Board Work: Continuous Casting Setup

Plaintext

```
[Ladle]
   | (Slide Gate)
   v
[Tundish]
   | (Stopper Rod)
   v
 [SEN] (Submerged Entry Nozzle)
   |
[Copper Mold] (Water-Cooled, Reciprocating)
   |
[Solidifying Strand] (Liquid Core + Solid Shell)
   |
[Sprays & Bending Rolls]
```

### Physical Interpretation: Process Mechanics

- **SEN (Submerged Entry Nozzle)**: Delivers molten metal from the tundish directly into the mold below the surface level to absolutely prevent air contact. Nozzle geometry (straight bore, twin-port, 4-port) is explicitly designed to optimize fluid flow within the mold. A constant mold level must be maintained; a drop in the mold level usually indicates SEN clogging 
    
- **Mold Reciprocation (Oscillation)**: The water-cooled copper mold continuously moves up and down by a few centimeters. This cyclic movement prevents the hot, solidifying steel shell from welding and sticking to the copper walls.
    
- **Mold Powder**: Added to the free surface of the mold. It melts and flows into the minute gap between the shrinking steel casting and the rigid copper mold. It acts as a vital lubricant and critically controls the rate of heat extraction across the gap.
    
- **Bulging and Breakouts**: If the mold powder design is incorrect or cooling is insufficient, the solid shell exiting the mold will be too thin. Under immense internal ferrostatic pressure, the thin shell bulges. If it ruptures, liquid steel jets out in a catastrophic and highly dangerous event known as a **breakout** .
    
- **Metallurgical Length**: Complete solidification does not occur within the mold. It occurs far downstream in the secondary cooling zone via intensive water sprays. The linear distance from the meniscus in the mold to the exact point of 100% complete solidification is defined as the metallurgical length.
  
# Audio v2: 

### **Part 1: Ingot Casting Setup & Process**

- **Mold Types:**
    
    - **Narrow End Up (NEU)**
        
    - **Wide End Up (WEU)**
        
- **The Hot Top:** * Added to the top of the mold to keep steel liquid for a prolonged time to feed shrinkage cavities (pipes).
    
    - Utilizes **anti-piping compounds** (a mixture of aluminum and oxides). The oxides react exothermically with the aluminum to produce heat.
        
    - The hot top section is eventually rejected/cut off and does not count toward the final ingot yield.
        
- **Stripping and Cooling:**
    
    - Complete solidification takes several hours depending on the ingot's size.
        
    - Once mostly solidified, the mold is removed (a process called **stripping**).
        
    - The exposed ingot is red-hot (molds are at **800–900°C** at the time of stripping) and loses heat predominantly via **radiation**.
        
    - To prevent rapid cooling and severe thermal stresses, the ingot is sometimes covered with insulating materials like **sand** to ensure a compatible cooling rate.
        
- **Solidification Kinetics:**
    
    - Solidification obeys a **parabolic rate law**.
        
    - The growth of the solidification front is governed by the equation where **x** (distance of the solidification front from the wall / thickness) is a function of **t** (time), modified by constants **a** and **b** (which depend on the mold material and solidification process).
        
    - Solidification advances from both sides until the fronts merge in the center.
        
- **Mold Preheating (Crucial Distinction):**
    
    - Reactors like ladles and tundishes are _always_ preheated before use.
        
    - **Ingot Molds are NEVER preheated.** Their purpose is to absorb and extract heat from the liquid steel.
        
    - However, due to constant recycling, cleaning, and inspection in the plant, molds are practically never at true room temperature (25–29°C); they typically retain residual heat from previous campaigns and sit around **60–65°C**.
        

---

### **Part 2: Classification of Ingots (Based on Deoxidation)**

Ingots are classified by their carbon and dissolved oxygen content:

**1. Killed Steel**

- **Characteristics:** Extremely low dissolved oxygen (approx. **10 ppm**).
    
- **Process:** Extensively deoxidized (killed) using large amounts of aluminum.
    
- **Result:** High carbon content relative to oxygen, hard steel, large inclusion content.
    

**2. Semi-Killed Steel (Ladle-Balanced Steel)**

- **Characteristics:** Intermediate oxygen levels (approx. **70–80 ppm**) and medium carbon.
    
- **Process:** Deoxidation is precisely controlled so residual oxygen remains. During solidification, carbon and oxygen are rejected into the liquid.
    
- **Result:** A carbon-oxygen reaction (forming CO bubbles) only triggers after **70% to 80%** of the ingot has solidified. These deep-seated bubbles perfectly compensate for solidification shrinkage.
    

**3. Rimming Steel**

- **Characteristics:** Highest dissolved oxygen, lowest carbon content. Soft steel.
    
- **Process:** Vigorous carbon-oxygen reaction (bubbling/rimming action) begins early, after only **10%** solidification.
    
- **Result:** Creates a thick, pure solid crust (the "rim"). The CO bubbles must be deep-seated. If bubbles form too close to the surface, they will oxidize when exposed to air, and oxidized bubbles will not weld shut during rolling, causing severe defects.
    
- **Note:** The rimming action is sustained by atmospheric oxygen reacting with ejected iron droplets. It is nearly impossible to produce true rimming steel via continuous casting.
    

---

### **Part 3: Defects in Ingot Casting**

The main challenge in steelmaking is conversion without introducing defects, which drastically lower the ingot's yield (salability).

- **Pipes:** Shrinkage cavities. **Primary pipes** form at the top and are eliminated by using a hot top. **Secondary pipes** form deeper inside but are less concerning because they lack oxygen exposure and will weld shut under the pressure of rolling mills.
    
- **Inclusions (Endogenous vs. Exogenous):**
    
    - Inclusions get trapped because steel has a very large "mushy zone" during solidification, preventing them from floating up.
        
    - **Endogenous:** Originate internally from deoxidation products.
        
    - **Exogenous:** Originate from outside sources.
        
        - _Mold Powder entrapment:_ Indicated by the presence of **Sodium (Na)** or **Potassium (K)**.
            
        - _Refractory wear:_ Indicated by **Magnesium (Mg)**, coming from worn runners or trumpet refractories.
            
- **Blowholes and Pinholes (Micro-porosity):**
    
    - Internal blowholes are acceptable; surface blowholes are major defects.
        
    - **Pinholes:** Extremely dangerous. They indicate **high hydrogen content** in the steel, making the final product highly susceptible to **hydrogen embrittlement** and cracking.
        
- **Segregation (Micro vs. Macro):**
    
    - **Micro-segregation:** Natural characteristic of alloy solidification (first metal to freeze is pure; last is impure). Requires thermal homogenization to fix.
        
    - **Macro-segregation:** Occurs when fluid flow (pouring rates of 0.5 tons/minute) physically dislodges micro-segregated crystals over large distances.
        
    - **Negative Segregation:** Occurs at the **bottom** of the ingot. Pure metal has a higher density, so it settles downward.
        
    - **Positive Segregation:** Occurs at the **top** of the ingot. Impure, solute-rich metal is lighter and rises.
        
- **Cracks:** Often caused by thermal stress or physical weakness during early solidification.
    

---

### **Part 4: Continuous Casting (CC) vs. Ingot Casting**

- **Why transition to CC?** Ingot casting is a batch process that cannot keep up with the high production turnover rates of the **BOF (Basic Oxygen Furnace)**. BOF commercialization started in **1952**, making CC a necessity by the 1960s/70s.
    
- **Energy Savings:** Rolling massive 10-ton, 900mm diameter ingots down to final shapes is intensely energy-demanding. CC produces "near net shapes" (closer to the final product), saving roughly **200 to 500 Mega Joules per ton of steel**.
    
- **Common CC Sections:**
    
    - **Billets:** Square cross-sections (e.g., **100 mm x 100 mm**).
        
    - **Blooms:** Larger rectangular sections (e.g., **250–300 mm x 300 mm**).
        
    - **Slabs:** Wide rectangles (e.g., **200–250 mm thick** by 800 mm, 1200 mm, or up to **1600 mm wide**).
        
    - **Thin Slabs:** Only **50 mm thick**.
        
    - **Strip Casting:** The newest technology. Strips are incredibly thin (**2 to 5 mm thick**), requiring practically zero hot-working to produce sheet metal/coils.
        

---

### **Part 5: Continuous Casting Setup and Mechanics**

- **Mold Design:**
    
    - Made of **copper** and extensively **water-cooled** (massive water flow rates cause a ~6°C temperature difference between input/output water).
        
    - Can be straight, vertical with horizontal discharge, or **curved** (most common, utilizes a multi-curvature design).
        
- **SEN (Submerged Entry Nozzle):**
    
    - Delivers metal from the tundish into the mold while protecting it from atmospheric air.
        
    - Geometry varies based on the cast shape: Bloom casters may use a straight bore or 4-port nozzle; Slab casters generally use complex twin-port nozzles.
        
- **Tundish Flow Control:** Liquid steel is fed into the mold via a slide gate or a **monoblock stopper rod** moving up and down.
    
- **Mold Level Control & Clogging:** * The depth/level of liquid steel in the mold must be maintained at a strict constant.
    
    - If SEN nozzle clogging/blockage occurs, metal flow into the mold drops. Because the machine withdraws the solidifying strand at a constant speed (usually less than 1 meter per minute), the mold level will immediately drop, signaling a blockage.
        
- **Mold Powder / Slag:**
    
    - Dropped onto the top of the molten steel in the mold.
        
    - As the steel solidifies and shrinks, a tiny gap (up to 1 mm) forms between the steel shell and the copper mold. The mold powder liquefies and fills this gap.
        
    - **Functions:** Provides **lubrication** and strictly **controls the rate of heat extraction**.
        
    - Powder composition is highly grade-specific. The wrong powder will cause improper cooling and severe thermal cracks.
        
- **Mold Reciprocation (Oscillation):**
    
    - The mold is not stationary; it constantly moves up and down (reciprocates) by a few centimeters (driven by a cam attachment).
        
    - **Purpose:** Prevents the hot, newly solidified steel shell from welding or sticking to the copper mold walls. (Sometimes molds are also coated with ceramics to aid this).
        

---

### **Part 6: Below the Mold (Secondary Cooling & Dangers)**

- **Dummy Block:** Used to initially plug the bottom of the empty mold to start the casting process. Molten metal freezes to it, and it is slowly withdrawn by mechanical rolls.
    
- **Solidified Shell & Bulging:**
    
    - As steel exits the mold, it is a liquid core surrounded by a solid outer shell.
        
    - If the shell is too thin (due to improper withdrawal speed or bad mold powder limiting heat extraction), the internal **ferrostatic pressure** pushes outward, causing the strand to **bulge**.
        
- **Breakouts:** * If bulging becomes extreme, the thin shell ruptures. The liquid steel core jets out violently into the machine.
    
    - This is a disastrous, hazardous event called a **breakout**. Even top-tier plants occasionally suffer 1-3 breakouts a year.
        
- **Secondary Cooling Zone:**
    
    - Below the mold, the strand passes through guide rolls and bending rolls.
        
    - It is aggressively cooled by **water sprays/jets** on all sides to solidify the remaining liquid core.
        
- **Metallurgical Length:** * The total linear distance from the top of the mold down to the exact point where the strand achieves 100% complete, internal solidification.