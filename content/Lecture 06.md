### **Lecture 6: Thermal Aspects, Internal Zones & Slag-Metal Reactions**

#### **1. Raceway Adiabatic Flame Temperature (RAFT)**

The **Raceway** is the combustion zone in front of the tuyeres where the hot blast reacts with coke.

- **Reaction:** $C + \frac{1}{2}O_2 \rightarrow CO$ (Exothermic).
    
    - This generates intense heat ($\approx 1900^\circ\text{C} - 2000^\circ\text{C}$).
    - The gas environment here is effectively **100% CO**; any $CO_2$ formed is instantaneously converted to CO due to the high temperature and presence of coke.
- **RAFT Concept:** It is the theoretical maximum temperature achieved under adiabatic conditions (no heat loss).    
- **Board Formula (Simplified Approximation):**

    The professor presented a simplified linear expression to estimate RAFT based on input parameters (Blast Temp, Coke Temp, etc.):
    
    $$RAFT \approx \frac{\text{Heat form Combustion} + \text{Sensible Heat of Blast} + \text{Sensible Heat of Coke}}{\text{Volume of Gas} \times \text{Specific Heat}}$$
    
    _Key Takeaway:_ **Increasing Blast Temperature ($T_B$) increases RAFT.**
    
- **Factors Affecting RAFT:**
    
    - **Oxygen Enrichment:** Increases RAFT.
    - **Moisture ($H_2O$):** Decreases RAFT (due to endothermic reaction $C + H_2O \rightarrow CO + H_2$).

#### **2. Blast Furnace Thermal & Gas Profile**

- **Gas:** Rises from Tuyeres ($\approx 2000^\circ\text{C}$) to Top ($\approx 300^\circ\text{C}$).
    - Moves very fast (seconds).
- **Solids:** Descend from Top ($\approx 25^\circ\text{C}$) to Hearth ($\approx 1500^\circ\text{C}$).
    - Moves very slowly (hours).  
- **Efficiency Indicator:**
    
    - **Lower Top Gas Temperature** = Better Thermal Efficiency (more heat transferred to solids).
    - **Lower CO in Top Gas** = Better Chemical Efficiency (more CO utilized for reduction).

---

#### **3. Internal Structure of the Blast Furnace (The 4 Zones)**

_Board Work Description:_ The professor drew a cross-section of the furnace dividing it into four distinct physical zones based on the state of the materials.

**Zone 1: The Granular Zone (Upper Stack)**

- **State:** Solid particles only.
- **Materials:** Lump Ore, Coke, Limestone remains solid.
- **Reactions:** Indirect reduction ($Fe_2O_3 \rightarrow Fe_3O_4 \rightarrow FeO$).

**Zone 2: The Cohesive Zone (Middle/Lower Stack)**

- **State:** Softening and Melting (Mushy Zone).
- **Process:**
    
    - Iron ore and gangue start to soften and fuse.
    - Formation of primary slag (Fayalite: $2FeO \cdot SiO_2$) and liquid iron.
    - **Coke remains solid:** Acts as the only permeable window for gas to pass through (Critical for aerodynamics).
    
- **Shape:** Often inverted V or W shape (though not explicitly drawn in this specific clip, it is implied by the zone description).
    

**Zone 3: The Active Coke & Deadman Zone (Lower Bosh)**

- **Active Coke:** Coke descending into the raceway to be burned.
    
- **Deadman Zone (Central Column):** A stagnant cone of coke at the very center-bottom that does not move much and does not burn (because gas doesn't penetrate deep enough).
    
    - Liquid Iron and Slag must trickle down _through_ this permeable coke bed (like water through a filter).
    - Carbon pickup (Carburization) happens here as iron touches the coke.

**Zone 4: The Hearth**

- **State:** Liquid Pool.
- **Stratification:**
    
    - **Slag (Top Layer):** Lighter oxides ($CaO, SiO_2, Al_2O_3, MgO$).
    - **Hot Metal (Bottom Layer):** Liquid Fe-C-Si-Mn-S-P alloy.

**(ASCII Representation of Board Diagram: Internal Zones)**

Plaintext

```
      |   Granular Zone    |  <-- Solids (Ore+Coke)
      |     (Solids)       |
      \                    /
       \   Cohesive Zone  /   <-- Softening/Melting
        \    (Mushy)     /        (Coke is the only solid)
         \              /
          |  Active    |
          |   Coke     |
      ----|            |----  <-- Tuyeres (Blast Injection)
     |    |  Deadman   |    |
     |    | (Stagnant) |    |
     |____|____________|____|
     |      Slag Layer      |
     |____Hot_Metal_Layer___|
```

---

#### **4. Chemical Reactions by Zone (Board Work Table)**

The professor tabulated reactions occurring as the burden descends.

| **Region**      | **Primary Reactions**                                                                                                                                                                                                                                                                                       | **Notes**                                                                                                                                                                                          |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Upper Stack** | $Fe_2O_3 \rightarrow Fe_3O_4$<br><br>  <br><br>$3Fe_2O_3 + CO \rightarrow 2Fe_3O_4 + CO_2$                                                                                                                                                                                                                  | Low Temp, Indirect Reduction.                                                                                                                                                                      |
| **Lower Stack** | $CaCO_3 \rightarrow CaO + CO_2$ (Calcination)<br><br>  <br><br>$FeO + CO \rightarrow Fe + CO_2$<br><br>  <br><br>$C + CO_2 \rightarrow 2CO$ (Solution Loss)<br>Gasification rxn vol & pressure change<br><br>overall $Fe + C  -> Fe + CO$ (Feels like Direct)<br><br>                                       | Solution Loss is endothermic. Combined with FeO reduction, it mimics "Direct Reduction."<br>but actual 2step rxn <br><br>pressure & temp  --> influence on rxn <br>pressure - gasification control |
| **Bosh**        | $SiO_2 + 2C \rightarrow \underline{Si} + 2CO$<br><br>$SiO_2(g)+ S(g) + C \rightarrow SiS(g) + CO(g)$<br><br>$SiS \rightarrow [S] + [Si]$<br>Decomposes unstable and [] indicate dissolve into metal   <br><br>$MnO + C \rightarrow \underline{Mn} + CO$<br><br>  <br><br>$CaO + S + C \rightarrow CaS + CO$ | High Temp & High Reduction Potential. Slag formation begins.                                                                                                                                       |
| **Hearth**      | Slag-Metal Reactions (Desulfurization)                                                                                                                                                                                                                                                                      | Final adjustment of Si, S, Mn.                                                                                                                                                                     |
|                 |                                                                                                                                                                                                                                                                                                             |                                                                                                                                                                                                    |

$Fe + SiO2  -> FeO.SiO2(l)$ Mainly Stack 
$Fe.SiO2 + C + CaO -> CaO.SiO2 + CO + Fe$(As $CaO$ More Basic Oxi. e and $SiO2$ acidic huge amount of attraction ) In Bosh 

$CaO.SiO_2 -- Al_2O_3 + TiO_2$  Gets mix in it 

**Bosh + Lower Stack / Upper Hearth Region**

$( )$ Means in oxide phase $[ ]$ in dissolved phase

_Note: Underlined elements ($\underline{Si}, \underline{Mn}$) indicate they are dissolved in the liquid metal._

---

#### **5. Slag-Metal Partitioning & Chemistry**

**The Behavior of Elements (Exam Critical):**

1. **Phosphorus (P):**
    
    - Thermodynamics: P-oxide line is very close to Fe-oxide line.
    - Result: **100% of Phosphorus** in the ore reduces and goes into the **Hot Metal**. It cannot be removed in the Blast Furnace.
        
2. **Manganese (Mn):**
    
    - Behaves similarly to Iron. Most MnO reduces to Mn and enters the metal.
    - Blast furnace slag contains very little MnO or FeO (<1%).
        
3. **Silicon (Si):**
    
    - Reaction: $(SiO_2) + 2C \rightleftharpoons [\text{Si}] + 2CO$ (Endothermic).
      Take place at lower part of furnace 
    - **Partitioning:** Partial. Some stays in slag as $SiO_2$, some enters metal as Si.
    - **Control:** Higher Temperature (High RAFT) $\rightarrow$ Drives reaction forward $\rightarrow$ **High Silicon in Metal.**
        
4. **Sulfur (S):**
    
    - Reaction: $[S] + (CaO) + C \rightarrow (CaS) + CO$.
    - **Requirement:** Reducing atmosphere + High Basicity (CaO) + High Temperature.
    - **Result:** The Blast Furnace is the _ideal_ place to remove Sulfur (unlike the Basic Oxygen Furnace).

**Slag Basicity:**

- Defined as the "V-Ratio": $V = \frac{\%CaO}{\%SiO_2}$.
- Changes dynamically as the slag trickles down and assimilates ash from the coke.


$CaO, Al_2O_3, SiO_2, CaS$ + $(FeO)$ if any left then will react with C(rxn below)
$----------------$  Slag-Metal Interface 
$Fe,C,Si,Mn,S,P,Ti$ 

$[C] + (Fe) \rightarrow {CO} + [Fe]$
Same for MnO if present any 
So HM never contains <0.01% FeO and MnO 
Oxygen Partial Pressure -> $10^{-19}$ atm no free oxygen can exist 






---

### **Final Data Check (Verification)**

1. **RAFT Formula:** The specific coefficients (4.6, 1.4 etc.) mentioned by the professor are empirical approximations for the adiabatic heat balance. The concept (Energy In / Heat Capacity) is physically correct.
2. **Phosphorus:** The statement that "All P goes to metal" is a standard metallurgical fact for Blast Furnaces.
3. **Internal Zones:** The division into Granular, Cohesive, Active Coke, and Hearth is the standard "Dissection Analysis" model (pioneered by Japanese researchers).

**Conclusion:** The notes are accurate to the lecture content.