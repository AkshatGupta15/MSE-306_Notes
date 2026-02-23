### **1. Recap & Objective**

Following the derivation of the **Bottom Segment Enthalpy Balance** in Lecture 11, the objective of this lecture is to:

1. Define the **Heat Demand ($D_E$)** and **Heat Supply ($S_E$)** terms explicitly.
    
2. Combine the **Enthalpy Balance** and **Oxygen Balance** equations to create a unified framework.
    
3. Map these equations onto the **Rist Diagram** (Operating Line) to allow for graphical solution of the Blast Furnace variables.
    

---

### **2. The Heat Demand Term ($D_E$)**

The **Heat Demand** represents the energy required by the process per mole of Iron ($Fe$) produced. It is a specific property of the bottom segment (Wustite Reduction Zone to Hearth).

#### **Formula for $D_E$**

$$D_E = D_{WRZ} = \sum (\text{Endothermic Requirements}) - \sum (\text{Sensible Heat Inputs})$$

**Components:**

1. **Reduction of Wustite:** Energy to break $Fe-O$ bonds ($Fe_{0.947}O \to Fe + O$).
    
2. **Sensible Heat of Iron:** Heating Iron from $1200 \text{ K}$ (Solid) to $1800 \text{ K}$ (Liquid).
    
3. **Sensible Heat of Dissolved Carbon:** Heating Carbon from $1200 \text{ K}$ to $1800 \text{ K}$ and dissolving it in Iron.
    
4. **Impurities (Non-Ideal Case):** Reduction of $SiO_2, MnO, P_2O_5$, and calcination of limestone.
    
5. **Slag Formation:** Sensible heat to raise slag components to $1800 \text{ K}$.
    

**Numerical Value (for Ideal Hematite Operation):**

For the standard case discussed (Pure Hematite, no Slag):

$$D_E \approx 116,000 \text{ kJ/kg-mole Fe}$$

_(Note: The instructor approximates this value in derivations. In real operations with slag, $D_E$ is significantly higher.)_

---

### **3. The Heat Supply Term ($S_E$)**

The **Heat Supply** is the energy provided by the Blast and the Combustion of Coke per mole of Active Carbon ($N_{AC}$).

#### **Formula for $S_E$**

$$S_E = \text{Blast Enthalpy Term} + \text{Combustion Enthalpy Term}$$

**Derivation steps from Board:**

1. **Combustion Heat:**
    
    - Formation of $CO$: Exothermic ($C + \frac{1}{2}O_2 \to CO$).
        
    - Formation of $CO_2$: Exothermic ($C + O_2 \to CO_2$).
        
2. **Weighted Average by Gas Composition:**
    
    The gas leaving the bottom segment is at equilibrium with Wustite at $1200 \text{ K}$.
    
    - $O/C_{gas} \approx 1.3$
        
    - This implies $\approx 70\% \ CO$ and $30\% \ CO_2$.
        
    - **Heat Evolution:**
        
        $$0.7 \times \Delta H_f(CO) + 0.3 \times \Delta H_f(CO_2) \approx 198,000 \text{ kJ/kg-mole C}$$
        
3. **Blast Contribution ($E_B$):**
    
    Sensible heat brought in by the hot blast (above $1200 \text{ K}$).
    

**Combined Supply Equation:**

$$\text{Total Supply} = N_{AC} \times [ 283,000 + E_B ]$$

_(Note: The coefficients depend on the precise heats of formation used. The transcript mentions `198,000` as the combustion part.)_

---

### **4. The Combined Characteristic Equation**

We now have two equations describing the bottom segment:

1. **Oxygen Balance:** $N_{OB} + 1.06 = 1.3 \cdot N_{AC}$
    
2. **Enthalpy Balance:** $D_E = N_{OB} \cdot E_B + N_{AC} \cdot 198,000$
    

By eliminating $N_{OB}$ (Blast Rate) between them, we solve for **Coke Rate ($N_{AC}$)** directly.

#### **Final Coke Rate Equation**

$$N_{AC} = \frac{D_E + 1.06 \cdot E_B}{198,000 + 1.3 \cdot E_B}$$

**Physical Interpretation:**

- **Numerator ($D_E + 1.06 E_B$):** Total thermal load adjusted for blast enthalpy carried by the oxygen associated with Wustite reduction.
    
- **Denominator ($198,000 + 1.3 E_B$):** Effective heat generation per mole of carbon, accounting for blast heat.
    

---

### **5. Graphical Representation: The Rist Diagram**

This is the core of the lecture—mapping the math onto the visual operating line.

**Axes:**

- **Y-Axis:** $O/Fe$ (Moles of Oxygen per mole of Iron).
    
- **X-Axis:** $O/C$ (Atomic Ratio in Gas).
    

**Key Points on the Diagram:**

1. **Point W (Wustite Point):**
    
    - Coordinates: $(X=1.3, Y=1.06)$
        
    - Represents the state at the Thermal Reserve Zone (TRZ).
        
    - This is the **Pivot Point** for the bottom segment operating line.
        
2. **Point P (The Pivot/Pole):**
    
    To satisfy the Enthalpy Balance graphically, the operating line must pass through a specific point **P** on the X-axis.
    
    - **Abscissa of P ($X_P$):**
        
        $$X_P = \frac{H_{supply}^{total}}{H_{demand}^{total}}$$
        
    - The instructor derives that the enthalpy balance forces the operating line to rotate around **W** such that it intercepts the X-axis at a specific value determined by $E_B$ and $D_E$.
        

**Construction of the Operating Line:**

1. **Plot Point W** at $(1.3, 1.06)$.
    
2. **Calculate Slope:** The slope of the line is the **Active Coke Rate ($N_{AC}$)**.
    
3. **Draw the Line:** Pass a line through W with slope $N_{AC}$.
    
    - **Intersect with Top ($Y=1.5$):** Gives Top Gas Composition.
        
    - **Intersect with Bottom ($X=0$):** Gives Blast Rate ($-N_{OB}$).
        

#### **Visualizing the Impact of Parameters**

- **Increasing Blast Temp ($T_B \uparrow$):**
    
    - $E_B$ increases (Supply increases).
        
    - Coke Rate ($N_{AC}$) **decreases** (Slope becomes flatter).
        
    - Operating line rotates clockwise around W.
        
- **Increasing Demand ($D_E \uparrow$):**
    
    - E.g., Higher slag volume or adding limestone.
        
    - Coke Rate ($N_{AC}$) **increases** (Slope becomes steeper).
        
    - Operating line rotates counter-clockwise around W.
        

---

### **6. Solution Algorithm (Summary)**

To solve any Steady State Blast Furnace problem:

1. **Calculate Demand ($D_E$):** Sum all endothermic heats (Reduction, Melting, Slag) minus inputs (Sensible heat of Ore/Coke).
    
2. **Calculate Blast Enthalpy ($E_B$):** Based on Blast Temperature ($T_{blast}$) and Moisture.
    
3. **Solve for Coke Rate ($N_{AC}$):** Use the derived algebraic equation:
    
    $$N_{AC} = \frac{D_E + 1.06 \cdot E_B}{198,000 + 1.3 \cdot E_B}$$
    
4. **Solve for Blast Rate ($N_{OB}$):** Use the Bottom Segment Oxygen Balance:
    
    $$N_{OB} = 1.3 \cdot N_{AC} - 1.06$$
    
5. **Solve for Top Gas ($O/C_{gas}$):** Use the Overall Oxygen Balance:
    
    $$(O/C)_{gas} = \frac{N_{OB} + 1.5}{N_{AC}}$$
    

**Instructor's Final Remark:**

"We have now completely solved the Blast Furnace. Give me the inputs (Ore chemistry, Blast Temp), and I will give you the outputs (Coke Rate, Blast Volume, Top Gas Analysis) using these three equations."