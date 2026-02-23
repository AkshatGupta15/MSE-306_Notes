# Lecture 21: Kinetics of Steelmaking, Slag Properties, and Process Overview

## 1. Correction: Dicalcium Silicate Formation Equation

At the beginning of the lecture, a correction is made to the stoichiometric representation of the lime-dissolution reaction discussed in the previous lecture.

**Corrected Chemical Equation:**

$$4CaO_{(s)} + [2FeO \cdot SiO_2]_{(l)} \rightarrow 2[CaO \cdot FeO]_{(l)} + [2CaO \cdot SiO_2]_{(s)}$$

- **Reactants:** Solid lime ($CaO$) reacts with liquid iron silicate ($2FeO \cdot SiO_2$, known as fayalite/ferrous silicate). Note that ferrous silicate contains 2 moles of $FeO$ for every 1 mole of $SiO_2$.
    
- **Products:** Liquid "calciowüstite" ($CaO \cdot FeO$ in equimolar proportions) and solid dicalcium silicate ($2CaO \cdot SiO_2$, containing 2 moles of $CaO$ per mole of $SiO_2$).
    

---

## 2. Kinetics of Steelmaking Reactions

Steelmaking involves multiphase, heterogeneous reactions (gas-metal, slag-metal). The overall rate of processes like decarburization, desulfurization, or dephosphorization is a combination of two phenomena:

1. **Mass Transport:** Movement of species via diffusion and convection to the reaction interface.
    
2. **Chemical Reaction:** Breaking and rearrangement of atomic bonds at the interface.
    

### A. Rate Control Mechanisms

At steelmaking temperatures ($\sim 1600^\circ\text{C}$), chemical reaction rates obey the Arrhenius rate law, meaning they are extremely fast due to exponential temperature dependence.

- _Exception:_ Certain reactions, like nitrogen dissolution from air or specific gasification reactions, may be chemically sluggish.
    
- _General Rule:_ Chemical reactions approach equilibrium almost instantaneously. Therefore, interfacial concentrations are dictated purely by thermodynamics (equilibrium).
    

**Rate Expressions:**
![[Pasted image 20260222202418.png]]

- **Chemical Rate:** $\dot{n}_c = k [C]^n$
    
    _(where $k$ = reaction rate constant, $n$ = reaction order)_
    
- **Mass Transfer Rate:** $\dot{n}_m = k_m \cdot A \cdot \Delta C$
    
    _(where $k_m$ = convective mass transfer coefficient in $\text{m/s}$, $A$ = interfacial area in $\text{m}^2$, $\Delta C$ = concentration gradient in $\text{kg/m}^3$)_
    
    _Dimensional analysis:_ $(\text{m/s}) \times (\text{m}^2) \times (\text{kg/m}^3) = \text{kg/s}$ (mass removal rate).
    

### _Instructor Notes: Transport Control_

Because chemical reactions are near-instantaneous, steelmaking kinetics are overwhelmingly **Transport Controlled** (specifically, Convective Mass Transfer). The rate of refining is not limited by chemistry, but by how fast you can physically push the reactants to the slag-metal or gas-metal boundary.

### B. The Role of Stirring

To maximize the mass transfer rate ($\dot{n}_m$), you must maximize $k_m$ and $A$. Both are achieved through intense stirring.

- **Increasing $k_m$:** Stirring increases fluid velocity, which directly increases the mass transfer coefficient.
    
- **Increasing $A$ (Interfacial Area):** In a stagnant bath, the interfacial area is just the cross-sectional area of the vessel ($\pi r^2$). With vigorous stirring, the interface becomes wavy, and phases entrain into one another (like an emulsion of oil and water). This expands the active reaction area exponentially.
    

---

## 3. Chemistry and Properties of Steelmaking Slags

Steelmaking slags are highly dynamic and predominantly **Quaternary Systems** made of four primary oxides:

- $CaO$ + $SiO_2$ ($\sim 75-80\%$ combined)
    
- $FeO$ ($\sim 15-20\%$)
    
- $MgO$ ($\sim 5\%$)
    
- _Trace impurities:_ Phosphorus, sulfur, etc.
    

### A. Basicity Definitions

Basicity is a critical chemical parameter dictating the slag's capacity to absorb impurities (like sulfide and phosphate capacities). Depending on precision needs, different definitions are used in the industry:

1. **Simple V-Ratio:**
    
    $$V = \frac{\text{wt\% } CaO}{\text{wt\% } SiO_2}$$
    
2. **Modified Basicity (All basics over all acids):**
    
    $$V_{mod} = \frac{\text{wt\% } CaO + \text{wt\% } MgO}{\text{wt\% } SiO_2 + \text{wt\% } P_2O_5}$$
    
3. **Weighted Basicity (Accounting for relative acidic/basic strengths):**
    
    $$V_{weighted} = \frac{\text{wt\% } CaO + 1.4(\text{wt\% } MgO)}{\text{wt\% } SiO_2 + 0.4(\text{wt\% } P_2O_5)}$$
    
![[Pasted image 20260222202557.png]]
### B. Silicate Network and Slag Fluidity

- **Structure:** Pure silica ($SiO_2$) forms a rigid, continuous 3D network of $SiO_4^{4-}$ tetrahedra sharing oxygen bonds.
    
- **Disruption:** When basic oxides ($CaO, MgO$) are added, their cations ($Ca^{2+}, Mg^{2+}$) break the bridging oxygen bonds.
    
- **Fluidity Threshold:** When the ratio of $CaO/SiO_2 \approx 2$, the silicate network is completely fragmented into discrete monomers. The slag becomes highly fluid.
    
![[Pasted image 20260222202457.png]]
### _Physical Interpretation: Kinetic Slag Properties_

Thermodynamics only tells you if a reaction _can_ happen. Kinetics dictates if the slag physically _allows_ it.

- **Fluidity/Viscosity:** A highly viscous slag restricts the movement of ions (like $Ca^{2+}$ or $S^{2-}$), throttling the mass transfer coefficient ($k_m$).
    
- **Melting Point:** If the slag is pasty (contains undissolved solids), mass transfer crashes. Operating in a fully liquid regime is critical.
    
![[Pasted image 20260222202528.png]]
### C. Chemical Potential and Ternary Phase Diagrams

- **Oxygen Potential:** The oxidizing power of the slag is dictated by $(FeO)$ and represented by the chemical potential of oxygen ($\mu_{O_2} = RT \ln P_{O_2}$).
    
- **Activity vs. Concentration:** You cannot use weight percentage directly as "activity" in thermodynamic equations. 15 wt% FeO does _not_ mean $a_{FeO} = 0.15$.
    
- **Slag Atlas:** To find actual activities, metallurgists use experimentally compiled Ternary Phase Diagrams (e.g., $CaO-SiO_2-FeO$ at a fixed $MgO\%$ and temperature).
    
    - These diagrams map out "Iso-activity lines" within the fully liquid phase fields.
        
    - They help operators steer the dynamically evolving slag composition so that it stays out of solid/pasty phase fields (like the dicalcium silicate field) and remains fully liquid.
        

---

## 4. Introduction to Modern Steelmaking Processes

Having established the thermodynamic and kinetic fundamentals, the course transitions to actual plant processes.

### A. Global Steel Production Distribution

Currently, global crude steel ($\sim 1.5$ billion tons/year) is dominated by two routes:

1. **Basic Oxygen Steelmaking (BOS / BOF):** $\sim 60-62\%$ of global production.
    
2. **Electric Arc Furnace (EAF):** $\sim 34-38\%$ of global production.
    
    _(Note: Acidic steelmaking is virtually extinct and will not be covered)._
    

**Metallic Feedstock Distribution:**

- Blast Furnace Hot Metal: $\sim 57\%$
    
- Scrap Steel: $\sim 38\%$
    
- DRI / Alternative Iron (Corex, Midrex, etc.): $\sim 4-5\%$
    

### B. Process Scale Comparison

|**Feature**|**Basic Oxygen Furnace (BOF)**|**Electric Arc Furnace (EAF)**|
|---|---|---|
|**Primary Feed**|Hot Metal (Liquid Pig Iron)|Steel Scrap (Solid)|
|**Plant Type**|Integrated Steel Plants (Giant scale)|Mini-mills (Specialty/regional scale)|
|**Converter Size**|100 to 320 Tons per heat|30 to 50 Tons per heat|
|**Refining Load**|Heavy (Needs to remove C, Si, P, S)|Light (Scrap is already purified steel)|

### C. Historical Context: The Birth of the LD Process

- **The 20-Year Delay:** Sir Henry Bessemer knew pure oxygen would make superior steel compared to air, but commercial pure oxygen wasn't available until 1932. Even then, commercial oxygen steelmaking didn't happen until **1952**.
    
- **The Engineering Challenge:** Why the wait? When pure $O_2$ is injected into a carbon/silicon-rich melt, the local heat generation is so extreme that it melts any submerged injection lances, tuyeres, and the surrounding refractory bricks within minutes.
    
- **The Breakthrough (1952):** In the Austrian cities of **Linz and Donawitz (LD)**, engineers discovered that the lance **did not need to be submerged**. By positioning a water-cooled lance _above_ the bath and blowing oxygen down at supersonic speeds (Mach 1.5 to 2.5), the jet penetrated the slag/metal interface, creating massive internal emulsions and rapid refining without melting the lance. This birthed the modern LD / BOF process.