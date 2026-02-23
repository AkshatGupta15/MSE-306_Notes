### **1. Introduction & Context**

To solve for the three operating variables of the Blast Furnace (Coke Rate, Blast Rate, Top Gas Composition), we need three characteristic equations.

- **Equation 1:** Overall Oxygen Balance (Derived in Lecture 10).
    
- **Equation 2:** Bottom Segment Oxygen Balance (Derived in Lecture 10).
    
- **Equation 3:** **Enthalpy Balance** (Subject of this lecture).
    

#### **Why "Bottom Segment" Enthalpy Balance?**

We avoid performing an enthalpy balance over the _entire_ furnace because the **Top Gas Temperature ($T_{top}$)** is an unknown process variable.

- If we used the whole furnace, we would introduce a 4th unknown ($T_{top}$).
    
- By focusing on the **Bottom Segment** (bounded by the Thermal Reserve Zone at the top and the Hearth at the bottom), all boundary temperatures are fixed:
    
    - **Upper Boundary:** Gas and Solids are at Thermal Equilibrium $\approx 1200 \text{ K}$.
        
    - **Lower Boundary:** Liquid products leave at $\approx 1800 \text{ K}$.
        

---

### **2. Control Volume & Boundary Conditions**

**Control Volume:** The region from the Thermal Reserve Zone (TRZ) down to the Hearth.

**Basis of Calculation:** 1 mole of Fe product.

#### **Inputs (Entering the Control Volume)**

|**Material**|**Composition / Species**|**Moles**|**Temperature**|
|---|---|---|---|
|**Solids (from Top)**|Wustite ($Fe_{0.947}O$)|$1.06$|$1200 \text{ K}$|
||Carbon (Coke)|$N_{IC}$|$1200 \text{ K}$|
|**Gases (from Bottom)**|Blast Oxygen ($O_2$)|$\frac{1}{2}N_{OB}$|$T_{blast}$ (Variable)|
||Blast Nitrogen ($N_2$)|$\frac{1}{2}N_{N_2}^{blast}$|$T_{blast}$|

#### **Outputs (Leaving the Control Volume)**

|**Material**|**Composition / Species**|**Moles**|**Temperature**|
|---|---|---|---|
|**Liquids (to Hearth)**|Liquid Iron ($Fe_{(l)}$)|$1.0$|$1800 \text{ K}$|
||Dissolved Carbon ($\underline{C}$)|$(C/Fe)_m$|$1800 \text{ K}$|
|**Gases (to Top)**|Carbon Monoxide ($CO$)|$n_{CO}^{gas}$|$1200 \text{ K}$|
||Carbon Dioxide ($CO_2$)|$n_{CO_2}^{gas}$|$1200 \text{ K}$|
||Nitrogen ($N_2$)|$\frac{1}{2}N_{N_2}^{blast}$|$1200 \text{ K}$|

---

### **3. Formulation of the Heat Balance**

At steady state: **Total Enthalpy Input = Total Enthalpy Output**

$$\sum (n_i H_i)_{in} = \sum (n_i H_i)_{out}$$

#### **3.1. The Raw Equation**

**Left Hand Side (Heat Input):**

$$\begin{aligned} \text{Input} &= \underbrace{1.06 \cdot H^\circ(Fe_{0.947}O, 1200)}_{\text{Wustite}} + \underbrace{N_{IC} \cdot H^\circ(C, 1200)}_{\text{Coke Carbon}} \\ &+ \underbrace{\frac{1}{2} N_{OB} \cdot H^\circ(O_2, T_{blast})}_{\text{Blast Oxygen}} + \underbrace{\frac{1}{2} N_{N_2} \cdot H^\circ(N_2, T_{blast})}_{\text{Blast Nitrogen}} \end{aligned}$$

**Right Hand Side (Heat Output):**

$$\begin{aligned} \text{Output} &= \underbrace{1.0 \cdot H(Fe_{(l)}, 1800)}_{\text{Liquid Iron}} + \underbrace{(C/Fe)_m \cdot H(\underline{C}, 1800)}_{\text{Dissolved Carbon}} \\ &+ \underbrace{n_{CO} \cdot H^\circ(CO, 1200)}_{\text{Gas CO}} + \underbrace{n_{CO_2} \cdot H^\circ(CO_2, 1200)}_{\text{Gas } CO_2} \\ &+ \underbrace{\frac{1}{2} N_{N_2} \cdot H^\circ(N_2, 1200)}_{\text{Gas Nitrogen}} \end{aligned}$$

---

### **4. Simplification & Grouping**

To make this equation solvable and elegant, we perform algebraic manipulations to group terms into meaningful process parameters.

#### **Step 1: Handling Carbon Terms ($N_{IC}$)**

The input carbon ($N_{IC}$) splits into Active Carbon ($N_{AC}$) which becomes gas, and Passive Carbon ($(C/Fe)_m$) which dissolves in iron.

$$N_{IC} = N_{AC} + (C/Fe)_m$$

- The passive carbon term on the LHS is grouped with the dissolved carbon term on the RHS.
    
- The active carbon ($N_{AC}$) is grouped with the gas terms ($CO, CO_2$).
    

#### **Step 2: Simplifying Gas Composition**

Using the relationships derived in Lecture 1:

- $n_{CO} = N_{AC} \cdot (2 - O/C_{gas})$
    
- $n_{CO_2} = N_{AC} \cdot (O/C_{gas} - 1)$
    

#### **Step 3: The "Blast Enthalpy" ($E_B$) Transformation**

This is the most critical derivation step. We aim to group all Blast-related terms ($O_2$ and $N_2$) into a single parameter $E_B$.

1. **Nitrogen Terms:** Group Input ($T_B$) and Output ($1200$) Nitrogen terms.
    
    $$\text{Net } N_2 \text{ Heat} = \frac{1}{2} N_{N_2} [ H^\circ(N_2, T_B) - H^\circ(N_2, 1200) ]$$
    
2. **Oxygen Terms:** The $O_2$ enters at $T_B$ but "leaves" as $CO/CO_2$. To mathematically group it like Nitrogen, we **add and subtract** a dummy term: $\frac{1}{2} N_{OB} H^\circ(O_2, 1200)$.
    
    This allows us to form a similar difference term for Oxygen:
    
    $$\text{Net } O_2 \text{ Sensible Heat} = \frac{1}{2} N_{OB} [ H^\circ(O_2, T_B) - H^\circ(O_2, 1200) ]$$
    
3. **Defining $E_B$:**
    
    We define the **Enthalpy of Blast ($E_B$)** per mole of Oxygen ($N_{OB}$):
    
    $$E_B = \frac{1}{2} \left[ (H^\circ_{O_2, T_B} - H^\circ_{O_2, 1200}) + \frac{0.79}{0.21} (H^\circ_{N_2, T_B} - H^\circ_{N_2, 1200}) \right]$$
    
    - _Note:_ The factor $\frac{0.79}{0.21}$ accounts for the ratio of $N_2$ to $O_2$ in air.
        

#### **Physical Interpretation of $E_B$**

- **If $T_{blast} = 1200 \text{ K}$:** $E_B = 0$. The blast brings no "extra" heat relative to the control volume boundary temperature.
    
- **If $T_{blast} > 1200 \text{ K}$:** $E_B > 0$. The blast acts as a **Heat Supply**.
    
- **If $T_{blast} < 1200 \text{ K}$:** $E_B < 0$. The blast creates a **Heat Demand** (needs heating).
    

---

### **5. Intermediate Result: The Transposed Equation**

After rearranging terms, grouping the blast enthalpy, and substituting carbon fractions, the equation takes the form:

$$\begin{aligned} \underbrace{E_B \cdot N_{OB}}_{\text{Heat Supply from Blast}} \&+ \text{ [Remaining Reaction \& Solid Terms] } \\ \&= \text{ [Liquid Output Terms] } \end{aligned}$$

- The derivation essentially separates terms into **Heat Supply** (Combustion + Hot Blast) and **Heat Demand** (Reduction of FeO + Melting/Heating Products).
    
- _Instructor's Note:_ The final "Supply = Demand" form ($D_E = S_E$) will be finalized in the next lecture.
    

### **6. Summary of Key Concepts**

1. **The W Point:** The intersection of the Overall and Bottom Segment operating lines on the Rist Diagram occurs at $W(1.3, 1.06)$. This point is a characteristic constant for a stable Thermal Reserve Zone.
    
2. **Adiabatic Assumption:** The derivation assumes no heat loss through walls (Adiabatic).
    
3. **Reference State:** The choice of 1200 K as the reference for gas separation simplifies the math significantly, avoiding the unknown Top Gas Temperature.