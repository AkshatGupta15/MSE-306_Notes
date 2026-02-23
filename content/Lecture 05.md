### **Lecture 5: Thermodynamics & Kinetics of Iron Making**

**(Physical, Chemical, and Thermal Characteristics of the Blast Furnace)**

---

#### **1. Overview of the Process**

The Blast Furnace (BF) is primarily an **Indirect Gaseous Reduction** process.

- **Direct Reduction:** Reduction by solid Carbon ($C$) – happens in the lower, hotter zones.
    
- **Indirect Reduction:** Reduction by Carbon Monoxide ($CO$) gas – happens in the upper stack.
    
- **Overall Reaction:**
    
    $$Fe_2O_3(s) + 3CO(g) \rightarrow 2Fe(s) + 3CO_2(g)$$
    

---

#### **2. Blast Furnace Environment (Thermal & Chemical)**

**A. Thermal Profile**

- **Tuyere/Raceway Zone (Bottom):** $\approx 1900^\circ C - 2000^\circ C$ (Combustion Zone).
    
- **Stock Line (Top):** $\approx 500^\circ C$.
    
- **Heat Transfer:** Ascending hot gases transfer heat to the descending cold solids (Counter-current exchange).
    

**B. Gas Composition Profile (Critical Exam Correction)**

- **At Tuyeres:**
    
    - The gas is **not** 100% CO by volume because of Nitrogen from the air blast.
        
    - **Actual Composition:** $\approx 35\text{-}45\% \text{ CO}$ and $\approx 55\text{-}60\% \text{ } N_2$ (Inert).
        
    - **Reducing Potential:** Although diluted by $N_2$, the chemical potential is extremely high because the $CO_2$ content is effectively **zero**. Any $CO_2$ formed immediately reverts to $CO$ via the Boudouard Reaction ($C + CO_2 \rightarrow 2CO$).
        
- **Ascending Gas:** As it rises and reduces the ore, $CO$ is consumed and $CO_2$ is generated.
    
- **Top Gas:** Contains $CO$, $CO_2$, and $N_2$.
    

**C. The "Layering" Effect**

The furnace is charged in alternate layers of **Coke** and **Ore/Flux**.

1. **Ore Layer:** Gas passes through $\rightarrow$ Reduces Iron Oxide $\rightarrow$ $CO_2$ increases.
    
2. **Coke Layer:** Gas enters hot coke $\rightarrow$ Boudouard Reaction ($C + CO_2 \rightarrow 2CO$) $\rightarrow$ $CO$ regenerated.
    
3. **Result:** The gas exiting a coke layer is "refreshed" to high reducing potential before hitting the next ore layer.
    

---

#### **3. Thermodynamics of Reduction (Fe-O-C System)**

Iron ore reduces in steps. The pathway depends strictly on temperature.

**A. The Reduction Hierarchy**

- **Step 1:** $Fe_2O_3 \rightarrow Fe_3O_4$ (Hematite to Magnetite). _Easy, occurs at top._
    
- **Step 2 (The Temperature Split):**
    
    - **If Temp < 570°C:** Reduction goes directly $Fe_3O_4 \rightarrow Fe$. (Wustite is unstable).
        
    - **If Temp > 570°C:** Reduction goes $Fe_3O_4 \rightarrow FeO$ (Wustite).
        
- **Step 3:** $FeO \rightarrow Fe$ (Wustite to Iron). _Most difficult step, requires high CO and Temp > 1000°C._
    

**B. Equilibrium Logic**

- For the reaction: $FeO + CO \rightleftharpoons Fe + CO_2$
    
- Equilibrium Constant: $K_{eq} = \frac{pCO_2}{pCO}$.
    
- **Condition for Reduction:** The actual gas ratio in the furnace must be "richer" in CO than the equilibrium value.
    
    $$\left(\frac{pCO}{pCO_2}\right)_{actual} > \left(\frac{pCO}{pCO_2}\right)_{equilibrium}$$
    

---

#### **4. Kinetics of Reduction (Rate of Production)**

Thermodynamics tells us _if_ it reacts; Kinetics tells us _how fast_.

**A. Topochemical (Shrinking Core) Model**

- Assumption: Iron ore particle is spherical.
    
- Reaction proceeds from the **surface inward**.
    
- **Structure:**
    
    - **Outer Shell:** Porous reduced Iron ($Fe$).
        
    - **Inner Core:** Unreacted Oxide ($FeO$).
        
    - **Interface:** Moves toward the center over time.
        

**B. The 5 Kinetic Resistance Steps**

The reaction must overcome 5 resistances in series. The slowest step controls the rate.

1. **Gas Transport:** CO diffuses through the **Gas Boundary Layer** surrounding the particle.
    
2. **Pore Diffusion (In):** CO diffuses through pores of the **reacted Iron shell**.
    
3. **Chemical Reaction:** Interfacial reaction ($FeO + CO \rightarrow Fe + CO_2$).
    
4. **Pore Diffusion (Out):** $CO_2$ diffuses back out through the shell.
    
5. **Gas Transport (Out):** $CO_2$ diffuses away through the boundary layer.
    

---

#### **5. Factors Influencing Reduction Rate**

1. **Gas Flow Velocity:**
    
    - Higher velocity $\rightarrow$ Thinner boundary layer $\rightarrow$ Faster external diffusion (Step 1 & 5).
        
    - _Significance:_ Critical if the process is "Mass Transfer Controlled."
        
2. **Temperature:**
    
    - Increases reaction rate constant ($k$) exponentially (Arrhenius Law).
        
    - _Significance:_ Critical if the process is "Chemically Controlled."
        
3. **Particle Porosity:**
    
    - More pores = Faster internal diffusion (Step 2 & 4).
        
    - _Note:_ Fluxed sinters are highly porous $\rightarrow$ Faster reduction than dense lumps.
        
4. **Gas Pressure:**
    
    - Higher pressure $\rightarrow$ Increases gas density and residence time (contact time).
        
    - Improves reduction rate by increasing effective concentration of reducing agents.
        

---

#### **6. Mathematical Representation**

- **Fraction Reacted ($f$):**
    
    $$f = 1 - \left( \frac{r_i}{r_0} \right)^3$$
    
    - $r_0$: Initial radius of the pellet.
        
    - $r_i$: Radius of the unreacted core at time $t$.
        
- **Rate:** $df/dt$ (measured in lab by weight loss / oxygen loss over time).