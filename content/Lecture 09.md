### **1. Introduction & Process Overview**

The Iron Blast Furnace (BF) is a counter-current reactor designed to reduce iron oxides to metallic iron.

- **Structure:** A tall vertical shaft where solid charge descends and gases ascend.
    
- **Counter-Current Flow:**
    
    - **Descending Phase:** Solid burden (Iron ore, Coke, Flux) charged from the top.
        
    - **Ascending Phase:** Reducing gases ($CO$, $N_2$) generated at the bottom tuyeres by combustion of coke with preheated blast ($O_2$, $N_2$).
        
- **Interaction:** Intense heat and mass transfer occur between the ascending hot gases and the descending solids.
    
    - Solids undergo heating, reduction, melting, and carburization.
        
    - Gases undergo cooling and oxidation ($CO \to CO_2$).
        

#### **Schematic of Inputs and Outputs**

Plaintext

```
                  Off-Gas (Top Gas)
                  (CO, CO2, N2)
                       ^
                       |
            +---------------------+
            |     Charge Input    |
            | (Iron Ore, Coke)    |
            |                     |
            |    BLAST FURNACE    |
            |                     |
            |  (Reaction Zone)    |
            |                     |
   Blast -> |      Tuyeres        | <- Blast
 (O2, N2)   |                     |    (O2, N2)
            +---------------------+
                       |
                       v
                Liquid Outputs
           (Hot Metal + Liquid Slag)
```

---

### **2. Modeling Philosophy: Steady State Assumption**

To control and understand the furnace, we develop a mathematical model. While complex models (aerodynamic, kinetic, granular flow) exist, this lecture focuses on a **Simplified Steady State Material and Enthalpy Balance**.

- **Steady State Definition:** The furnace operates continuously. Averaged over a significant time period (e.g., monthly), inputs equal outputs. There is no accumulation of mass or energy within the control volume.
    
    - _Mathematical implication:_ $\text{Input Rate} = \text{Output Rate}$.
        
- **Model vs. Law:** Laws (e.g., thermodynamics) are exact. Models are approximations based on assumptions.
    

---

### **3. Simplifying Assumptions for the Model**

To make the system solvable, several idealizations are made:

1. **Pure Materials:**
    
    - Iron Ore is pure Hematite ($Fe_2O_3$).
        
    - Coke is pure Carbon ($C$).
        
    - Blast is pure Oxygen and Nitrogen mixture.
        
    - _Note:_ No gangue ($SiO_2$, $Al_2O_3$) implies no slag formation in the ideal case (relaxed later).
        
2. **Product Purity:**
    
    - **Hot Metal:** Contains only $Fe$ and dissolved Carbon ($C$). No $Si, Mn, S, P$.
        
    - **Slag:** Contains no Iron ($Fe$) and no Carbon ($C$).
        
3. **No Losses:**
    
    - No material loss via dust.
        
    - No heat loss through furnace walls (Adiabatic).
        
4. **Oxygen Distribution:**
    
    - No Oxygen in Hot Metal (Carbon saturation prevents dissolved $O$).
        
    - All Oxygen from Ore and Blast manifests in the **Off-Gas**.
        

---

### **4. Material Balance Formulation**

**Basis of Calculation:**

All calculations are performed per **1 kg-mole of Fe product** in the hot metal.

$$n_{Fe}^{product} = 1 \text{ kg-mole}$$

#### **4.1. Iron (Fe) Balance**

Since there is no Fe loss to slag or dust:

$$n_{Fe}^{in (Ore)} = n_{Fe}^{out (Metal)} = 1$$

- _Implication for Hematite ($Fe_2O_3$):_ To get 1 mole of Fe, we need 0.5 moles of $Fe_2O_3$.
    

#### **4.2. Carbon (C) Balance & Distribution**

Carbon input comes from Coke. It splits into two streams inside the furnace:

1. **Passive Carbon ($n_C^{passive}$):**
    
    - Dissolves in the hot metal.
        
    - Does _not_ participate in reduction or combustion reactions.
        
    - Leaves the furnace in the liquid metal.
        
2. **Active Carbon ($n_C^{active}$):**
    
    - Participates in combustion and reduction.
        
    - Leaves the furnace in the Off-Gas (as $CO$ or $CO_2$).
        
    - _Instructor Note:_ This is the quantity we aim to minimize to lower the Coke Rate.
        

**Total Coke Rate ($n_C^{total}$):**

$$n_C^{total} = n_C^{active} + n_C^{passive}$$

**Molar Ratio in Metal ($C/Fe]_m$):**

This represents the passive carbon.

$$(C/Fe)_m = \frac{\text{Moles of C in Metal}}{\text{Moles of Fe in Metal}}$$

- For saturation (approx 4.3 wt% C), $(C/Fe)_m \approx 0.21$.
    
- For 4.0 wt% C, $(C/Fe)_m \approx 0.20$.
    
- _Formula:_ $(C/Fe)_m$ is a fixed parameter based on hot metal chemistry.
    

#### **4.3. Oxygen (O) Balance**

_Convention:_ Moles of Oxygen are expressed as atomic Oxygen ($O$), not molecular ($O_2$).

**Input Sources:**

1. **Iron Ore:** Oxygen combined with Iron.
    
    - Parameter: $(O/Fe)_x$ = Moles of $O$ per mole of $Fe$ in ore.
        
    - For Hematite ($Fe_2O_3$): $(O/Fe)_x = 1.5$.
        
    - For Magnetite ($Fe_3O_4$): $(O/Fe)_x = 1.33$.
        
2. **Blast:** Gaseous Oxygen injected ($n_O^{blast}$).
    

**Output:**

- Entire Oxygen output is in the **Off-Gas** (as $CO$ and $CO_2$).
    

#### **4.4. Off-Gas Analysis ($O/C$ Ratio)**

The composition of the top gas indicates furnace efficiency. We analyze the **Carbonaceous Portion** ($CO + CO_2$).

Define $(O/C)_{gas}$ as the molar ratio of Oxygen to Carbon in the top gas.

$$(O/C)_{gas} = \frac{n_O^{gas}}{n_C^{gas}} = \frac{n_{CO} + 2n_{CO_2}}{n_{CO} + n_{CO_2}}$$

**Mole Fractions:**

Let $x_{CO_2}$ and $x_{CO}$ be mole fractions in the carbonaceous gas mixture.

$$x_{CO_2} = \frac{n_{CO_2}}{n_{CO} + n_{CO_2}}$$

**Derivation of Composition from $(O/C)_{gas}$:**

$$(O/C)_{gas} = \frac{1 \cdot n_{CO} + 2 \cdot n_{CO_2}}{n_{CO} + n_{CO_2}} = \frac{(n_{CO} + n_{CO_2}) + n_{CO_2}}{n_{CO} + n_{CO_2}}$$

$$(O/C)_{gas} = 1 + x_{CO_2}$$

Therefore:

$$x_{CO_2} = (O/C)_{gas} - 1$$

$$x_{CO} = 2 - (O/C)_{gas}$$

- **Range:** $1 \le (O/C)_{gas} \le 2$
    
    - $(O/C)_{gas} = 1 \implies 100\% \text{ CO}$ (Low Efficiency)
        
    - $(O/C)_{gas} = 2 \implies 100\% \text{ CO}_2$ (High Efficiency)
        

---

### **5. Summary of Model Variables**

To solve the system, we identify variables and required equations.

**Known Parameters (4):**

1. $n_{Fe}^{in}$ (Input Fe = 1)
    
2. $n_{Fe}^{out}$ (Output Fe = 1)
    
3. $(C/Fe)_m$ (Metal composition, ~0.21)
    
4. $(O/Fe)_x$ (Ore stoichiometry, 1.5 for hematite)
    

**Unknown Variables (The "Big Three" Performance Indicators):**

1. **Blast Rate:** Amount of Oxygen/Air required.
    
2. **Coke Rate ($n_C^{active}$):** Carbon required for reaction.
    
3. **Top Gas Composition ($O/C$ ratio):** Efficiency of the process.
    

**Instructor's Conclusion:**

We have established the variables. To have a fully predictive model, we need **3 Characteristic Equations** involving these unknowns. These will be derived in the next lecture based on:

1. Overall Oxygen Balance.
    
2. Heat/Enthalpy Balance.
    
3. Chemical Equilibrium (Efficiency constraints).