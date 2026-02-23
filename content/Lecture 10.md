### **1. Recap & Model Framework**

The goal is to develop a fully predictive steady-state model for the Blast Furnace (BF) to calculate performance indicators based on input parameters.

- **Basis of Calculation:** 1 kg-mole of Iron ($Fe$) product.
    
- **Known Parameters (4):**
    
    1. Iron Input: $n_{Fe}^{in} = 1$ (since output is 1 mole).
        
    2. Iron Output: $n_{Fe}^{out} = 1$.
        
    3. Ore Composition: $(O/Fe)_{ore}$ (e.g., 1.5 for Hematite).
        
    4. Metal Composition: $(C/Fe)_{metal}$ (Dissolved carbon, $\approx 0.21$ for saturated hot metal).
        
- **Unknown Variables (The "Big Three"):**
    
    1. **Coke Rate ($n_C^{active}$ or $N_{AC}$):** Moles of carbon participating in gas-phase reactions per mole $Fe$.
        
    2. **Blast Rate ($n_O^{blast}$ or $N_{OB}$):** Moles of oxygen supplied by the blast per mole $Fe$.
        
    3. **Top Gas Composition ($(O/C)_{gas}$):** The atomic oxygen-to-carbon ratio in the top gas.
        
- **Objective:** Derive **3 Characteristic Equations** to solve for these 3 unknowns.
    
    - _Lecture 10 focuses on the first two equations derived from Oxygen Balances._
        

---

### **2. Equation 1: Overall Oxygen Balance**

This equation conserves oxygen across the entire furnace.

#### **2.1. Derivation**

Consider the control volume of the entire Blast Furnace:

- **Inputs of Oxygen:**
    
    1. **From Blast:** $N_{OB}$ (Atomic oxygen moles).
        
    2. **From Ore:** $(O/Fe)_{ore}$ (Stoichiometric oxygen associated with iron).
        
        - For Hematite ($Fe_2O_3$): $(O/Fe) = 1.5$.
            
- **Outputs of Oxygen:**
    
    1. **In Top Gas:** All oxygen leaves as $CO$ or $CO_2$.
        
    2. The amount is defined by the total active carbon ($N_{AC}$) and the gas composition ratio $(O/C)_{gas}$.
        
    
    - $\text{Output Oxygen} = N_{AC} \times (O/C)_{gas}$
        

**Equation 1 (Standard Form):**

$$N_{OB} + (O/Fe)_{ore} = N_{AC} \cdot (O/C)_{gas}$$

_For Ideal Hematite Operation:_

$$N_{OB} + 1.5 = N_{AC} \cdot (O/C)_{gas}$$

#### **2.2. Graphical Representation (The Operating Line)**

This equation can be rearranged into a linear form $y_2 - y_1 = m(x_2 - x_1)$ to be plotted on an **Rist Diagram** (Oxygen vs. O/C Ratio).

- **Rearrangement:**
    
    $$1.5 - (-N_{OB}) = N_{AC} \cdot [(O/C)_{gas} - 0]$$
    
    - _Slope ($m$):_ $N_{AC}$ (Active Coke Rate).
        
    - _Point 1 (Bottom/Blast):_ Coordinates $(0, -N_{OB})$.
        
    - _Point 2 (Top/Gas):_ Coordinates $((O/C)_{gas}, 1.5)$.
        
- **Interpretation:**
    
    - The slope of the line connecting the Blast point and the Top Gas point represents the **Coke Rate**.
        
    - **Efficiency:** A flatter slope indicates a lower Coke Rate (Higher efficiency). A steeper slope indicates high fuel consumption.
        

#### **2.3. Handling Impurities (Non-Ideal Case)**

In real operations, other elements (Si, Mn, P) are reduced, consuming carbon and releasing oxygen.

- _Example: Silicon Reduction ($SiO_2 \to Si + 2O$)_
    
    - If Hot Metal contains 1 wt% Si:
        
    - This requires extra carbon (Endothermic load) and releases extra oxygen into the gas.
        
    - **Modification:** The term $(O/Fe)_{ore}$ increases to account for oxygen from silica.
        
    - **Revised Eq:** $N_{OB} + [1.5 + \Delta O_{Si}] = N_{AC}' \cdot (O/C)_{gas}'$.
        

---

### **3. The Conceptual Line of Division (CLD)**

To derive the second equation, the furnace is conceptually divided into two zones based on temperature and reaction types.

#### **3.1. The Line of Division**

- **Location:** Located at the **Thermal Reserve Zone**, approximately **1200 K (approx. 900-1000°C)**.
    
- **Physical Significance:**
    
    - At this boundary, the descending solids and ascending gases are in **Thermal Equilibrium** ($T_{gas} \approx T_{solid} \approx 1200 K$).
        
    - Below this line: High temperature (Endothermic reactions active).
        
    - Above this line: Lower temperature (Exothermic/Mildly Endothermic reactions).
        

#### **3.2. Upper Segment (Preparation Zone)**

- **Reactions:** Indirect reduction of higher oxides ($Fe_2O_3 \to Fe_3O_4 \to Fe_xO$).
    
- **Key Assumption:** **Carbon is INERT.**
    
    - Temperature is too low for the Boudouard Reaction (Solution Loss: $C + CO_2 \to 2CO$).
        
    - Therefore, the moles of active carbon entering the top ($N_{AC}$) equal the moles crossing the CLD into the bottom.
        

#### **3.3. Bottom Segment (Wustite Reduction Zone - WRZ)**

- **Reactions:**
    
    - Final reduction of Wustite to Iron: $Fe_xO + CO \to Fe + CO_2$.
        
    - Coke gasification (Solution Loss) and combustion occur here.
        
- **Iron Input Form:** Iron enters this zone not as $Fe_2O_3$, but as **Wustite (Non-stoichiometric FeO)**.
    

---

### **4. Equation 2: Bottom Segment Oxygen Balance**

We perform an oxygen balance specifically for the Bottom Segment (below the CLD).

#### **4.1. Wustite Stoichiometry**

- Wustite is iron-deficient: $Fe_{0.947}O$.
    
- To produce **1 mole of Fe product**, we need more than 1 mole of $Fe_{0.947}O$.
    
- **Moles of Oxygen in Wustite per mole Fe:**
    
    $$(O/Fe)_{wustite} = \frac{1}{0.947} \approx 1.056 \to \textbf{1.06}$$
    
- _Input Oxygen from Ore term becomes 1.06._
    

#### **4.2. Chemical Equilibrium Constraint**

In the Thermal Reserve Zone (at the CLD), the gas composition is fixed by the **Chemical Equilibrium** of wustite reduction:

$$FeO + CO \rightleftharpoons Fe + CO_2$$

- At ~1200 K (1000°C), thermodynamics dictate the equilibrium ratio of $CO$ to $CO_2$.
    
- **Equilibrium Gas Composition:**
    
    - $\%CO \approx 70\%$
        
    - $\%CO_2 \approx 30\%$
        
- **Equilibrium O/C Ratio ($(O/C)_{WRZ}$):**
    
    $$(O/C)_{WRZ} = \frac{1 \cdot n_{CO} + 2 \cdot n_{CO_2}}{n_{CO} + n_{CO_2}} \approx 1 + 0.3 = \textbf{1.3}$$
    

#### **4.3. Derivation**

Balance Oxygen for the Bottom Segment:

- **Input:**
    
    1. Blast Oxygen: $N_{OB}$ (Same as overall).
        
    2. Wustite Oxygen: $1.06$ (Oxygen entering with solid).
        
- **Output:**
    
    1. Gas leaving the bottom segment (at equilibrium).
        
    2. Oxygen = $N_{AC} \times (O/C)_{WRZ}$.
        

**Equation 2 (Bottom Segment Balance):**

$$N_{OB} + 1.06 = N_{AC} \cdot 1.3$$

---

### **5. Summary of Derived Equations**

We now have two linear equations linking the unknowns:

1. **Overall Oxygen Balance:**
    
    $$N_{OB} + 1.5 = N_{AC} \cdot (O/C)_{gas}$$
    
    _(Note: Contains 3 unknowns: $N_{OB}, N_{AC}, (O/C)_{gas}$)_
    
2. **Bottom Segment Oxygen Balance (Wustite Reduction Zone):**
    
    $$N_{OB} + 1.06 = 1.3 \cdot N_{AC}$$
    
    _(Note: Contains 2 unknowns: $N_{OB}, N_{AC}$. This fixes the linear relationship between Coke Rate and Blast Rate.)_
    

**Instructor's Note:**

These equations are "Conceptually Fabulous." They demonstrate that for large blast furnaces, the existence of a **Chemical and Thermal Reserve Zone** allows us to fix the gas composition at the zonal boundary ($O/C \approx 1.3$), significantly simplifying the complex reactor into solvable algebraic expressions.

_Next Step:_ The third equation (Enthalpy Balance) will be derived in the next lecture to fully solve the system.