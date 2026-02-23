# **Lecture Notes: Blast Furnace Ironmaking – The Rist Diagram (Operating Line)**

**Source:** Lecture 13, Prof. Dipak Mazumdar (IIT Kanpur)

**Topic:** Analytical and Graphical Modeling of Blast Furnace Operations (Rist Diagram Construction & Interpretation)

---

## **1. Introduction & Context**

This lecture continues the development of a **predictive mathematical model** for the Blast Furnace (BF). Having previously established the material and enthalpy balance equations, the focus shifts to:

1. **Solving for the three key unknowns** of the BF process:
    
    - **Top Gas Composition** ($O/C$ ratio or $\%CO/\%CO_2$).
        
    - **Coke Rate** ($N_{AC}$, active carbon required).
        
    - **Blast Rate** ($N_{OB}$, blast oxygen required).
        
2. **The Rist Diagram:** Visualizing these equations as an **Operating Line** on a specific coordinate system to analyze furnace efficiency and productivity.
    

---

## **2. Governing Equations (Recap & Consolidation)**

The model is built upon three fundamental balance equations applied to the **Bottom Segment** (Wustite Reduction Zone - WRZ) and the overall furnace.

### **A. The Balance Equations**

1. **Overall Oxygen Balance**  $$n_{O}^B + 1.5 = n_{c}^A(O/C)^g$$
    
2. **Wustite Reduction Zone (WRZ) Oxygen Balance** 
   $$n_{O}^B + 1.06 = 1.3n_{c}^A$$
    
3. **WRZ Enthalpy Balance**
   $$D^{wrz} = E_Bn_O^B + 198000n_C^A$$
   where 
4. $$  D^{wrz} = 330,000 KJ/kg-mole of Fe$$
5. $$ D^{wrz} = E_Bn_O^B - n_C^A [ \{2- (O/C)^{g,wrz} \}  H^f_{CO,1200K} + \{ (O/C)^{g,wrz} - 1 \}H^f_{CO2,1200K} ]$$
    $$H^f_{CO,1200K}=113000 KJ/mole$$
    $$ H^f_{CO2,1200K} = 395000KJ/mole $$

For an **idealized operation** (Hematite feed, no impurities), the thermal demand of the bottom zone is quantified as:

$$D^{wrz} \approx 330,000 \text{ kJ/kg mole Fe}$$

Combined Bottom Segment Oxygen & Enthalpy Balance: 
$$ D^{wrz} = n_C^A[1.3E_B + 198,0000 - 1.06E_B$$

**Components of $D_{WRZ}$ (Idealized):**

1. Enthalpy to break $Fe-O$ bonds (Reduction of Wustite to Iron).
    
2. Enthalpy to heat Iron from $1200^\circ C$ (Reserve Zone temp) to $1800^\circ C$ (Tapping temp).
    
3. Enthalpy to dissolve $4.3\%$ Carbon into liquid Iron.
    

### **B. Combined Enthalpy & Oxygen Balance**

To create a graphical representation, the enthalpy and oxygen balance equations are combined. The instructor derives a linear relationship containing terms related to the **Heat of Formation** ($\Delta H_f$) of $CO$ and $CO_2$.

**Key Thermodynamic Values (at 1200 K):**

- $\Delta H_f(CO) \approx -113,000 \text{ kJ/mole}$
    
- $\Delta H_f(CO_2) \approx -395,000 \text{ kJ/mole}$
    

Using these values, two specific constants appear in the derived equation:

- **282,000** (Derived from $\Delta H_f(CO_2) - \Delta H_f(CO)$)
    
- **169,000** (Derived from $2 \times \Delta H_f(CO) - \Delta H_f(CO_2)$)
    

---

## **3. The Rist Diagram (Operating Line Construction)**

The Rist Diagram is a graphical tool that plots the **Oxygen-to-Iron Ratio ($O/Fe$)** against the **Oxygen-to-Carbon Ratio ($O/C$)**.

### **A. Coordinate System**

- **Y-Axis (Ordinate):** $O/Fe$ (Moles of Oxygen per Mole of Iron).
    
    - Range: $0$ (Liquid Iron) to $1.5$ (Hematite $Fe_2O_3$).
        
- **X-Axis (Abscissa):** $O/C$ (Moles of Oxygen per Mole of Carbon in gas).
    
    - Range: $1.0$ (Pure $CO$) to $2.0$ (Pure $CO_2$).
        

### **B. The Operating Line**

The Blast Furnace operation is represented by a straight line passing through two characteristic points: **Point W** and **Point H**.

#### **1. Point W (The Pinch Point)**

Represents the chemical and thermal equilibrium in the Reserve Zone (approx. $1000^\circ C - 1200^\circ C$).

- **Coordinates $(X_W, Y_W)$:**
    
    - **$X_W \approx 1.3$:** Thermodynamic equilibrium gas composition ($O/C$) for Wustite reduction.
        
    - **$Y_W \approx 1.06$:** The atomic ratio of Oxygen to Iron in Wustite ($FeO_{1.05-1.06}$).
        
- _Note:_ These coordinates are fixed for an "Ideal" operation but shift slightly with real ore mineralogy.
    

#### **2. Point H (The Enthalpy/Heat Balance Point)**

This theoretical point is derived from the enthalpy balance. Its coordinates depend on the heat demand ($D_{WRZ}$) and the heat supplied by the blast ($E_B$).

**Derived Coordinates for Point H $(X_H, Y_H)$:**

$$X_H = \frac{169,000}{282,000 + E_B}$$

$$Y_H = \frac{1.06 \cdot D_{WRZ} + 1.06 \cdot E_B}{282,000}$$

_(Note: The exact form of $Y_H$ involves the algebraic manipulation of the $D_{WRZ}$ and enthalpy terms shown on the board.)_

### **C. Properties of the Line**

- **Slope ($N_{AC}$):** The slope of the line connecting H and W represents the **Coke Rate** (Active Carbon per mole Fe).
    
    - **Steeper Slope** $\rightarrow$ Higher Coke Rate (Less Efficient).
        
    - **Flatter Slope** $\rightarrow$ Lower Coke Rate (More Efficient).
        
- **Intercepts:** Extrapolating the line gives the Top Gas Composition (at $Y=1.5$) and the Blast Rate.
    

---

## **4. Visual Representation (Board Work Reconstruction)**

Below is a reconstruction of the **Rist Diagram** as drawn on the board, showing the Operating Line and the shift directions for efficiency.

Plaintext

```
      Y-Axis (O/Fe)
        ^
    2.0 +
        |
    1.5 +--------- Top Gas Composition (Exit)
        |         \
        |          \  <-- Operating Line
    1.06+           \ W (Pinch Point: ~1.3, 1.06)
(Wustite)|            \
        |             \
    0.0 +--------------\-------------------->
(Liq Fe)|               \
        |                \
   -Nob +                 \ H (Enthalpy Point)
        |                  \
        +---------+---------+---------+----> X-Axis (O/C)
       1.0       1.5       2.0       (Gas Composition)
      (CO)               (CO2)

```

---

## **5. Factors Affecting Blast Furnace Efficiency**

The power of the Rist Diagram lies in visualizing how operational changes "move" Points W and H, thereby changing the slope (Coke Rate).

### **A. Blast Temperature (Enthalpy $E_B$)**

- **Effect:** Increasing Blast Temperature increases the enthalpy input ($E_B$).
    
- **Movement on Graph:** Point **H** moves **upward/left** (towards the Y-axis).
    
- **Result:** The operating line becomes **less steep**.
    
- **Benefit:** **Lower Coke Rate** and **Higher Productivity**.
    
- _Limitation:_ Practical limits on stove materials restrict blast temp (typically max $\sim 1200-1300^\circ C$).
    

### **B. Thermal Demand ($D_{WRZ}$)**

- **Effect:** Reducing the thermal demand (e.g., using better quality ore with less gangue/slag, lower heat losses).
    
- **Movement on Graph:** Point **H** moves **down/right** (favorable direction).
    
- **Result:** The operating line becomes **less steep**.
    
- **Benefit:** **Lower Coke Rate**.
    
- _Note:_ Large furnaces have lower surface-area-to-volume ratios, reducing heat loss components of $D_{WRZ}$.
    

### **C. Ore Quality & Impurities (Point W)**

- **Effect:** Presence of impurities (Silica, Alumina, Phosphorus) or metalloids requiring reduction changes the initial oxygen ratio.
    
- **Movement on Graph:** Point **W** shifts (specifically, the Y-intercept $1.06$ increases to e.g., $1.16$ or $1.17$).
    
- **Result:** The pivot point W moves up, forcing a **steeper slope**.
    
- **Penalty:** **Higher Coke Rate** (Lower Efficiency).
    
- _Mitigation:_ Charging metallic iron (scrap) lowers the effective input $O/Fe$, moving W down (beneficial).
    

### **D. Oxygen Enrichment**

- **Effect:** Reduces Nitrogen volume, alters enthalpy carried by blast, and changes gas transport.
    
- **Movement:** Moves Point H favorably.
    
- **Benefit:** **Increases Productivity** significantly.
    

---

## **6. Productivity & Blast Rate**

The instructor defines a specific relationship for productivity based on blast volume:

$$\text{Productivity} \propto \frac{1}{\text{Blast Rate per Ton of Hot Metal}}$$

- **Goal:** Minimize the Blast Rate ($N_{OB}$) required to produce a ton of iron.
    
- **Mechanism:** Any parameter change (High Blast Temp, Low $D_{WRZ}$) that flattens the operating line reduces the required blast volume per unit iron, thereby **increasing the daily production rate** (TPD).
    
    $$\text{Productivity} \propto \frac{\text{Total vol of blast supplied in a day}}{\text{Blast Rate per Ton of Hot Metal}}$$

---

## **7. Summary & Instructor's Closing Remarks**

- **The "Operating Line"** is a straight line passing through the Reserve Zone equilibrium point (**W**) and the Heat Balance point (**H**).
    
- **To Improve Efficiency (Lower Coke Rate, Higher Productivity):**
    
    1. Maximize Blast Temperature.
        
    2. Minimize Thermal Demand ($D_{WRZ}$) (e.g., control slag volume, reduce heat loss).
        
    3. Control Burden Chemistry (minimize impurities that raise the W point).
        
- The Rist Diagram analytically solves the three simultaneous balance equations without needing iterative numerical calculation, providing a powerful visual guide for process engineers.