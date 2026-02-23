# Lecture Notes: Steelmaking Reactions – Dephosphorization and Kinetics

## 1. Introduction to Dephosphorization

**Dephosphorization** refers to the removal of phosphorus from the hot metal. During the ironmaking stage (in the blast furnace), nearly all the phosphorus from the charge material (iron ore) is reduced and joins the molten metal phase.

- **Initial Phosphorus Content:** Depending on the ore quality, hot metal typically contains **0.1% to 0.15% phosphorus** by weight.
    
- **Target Phosphorus Content:** For high-quality steel intended for critical applications, the target phosphorus content is strictly controlled to **$\sim$ 30 ppm (0.003 wt%)** or even as low as 10 ppm.
    
- _Note on Terminology:_ Just as sulfur removal is abbreviated as **De-S**, phosphorus elimination is denoted as **De-P**.
    

---

## 2. Thermodynamics of Dephosphorization

### A. Chemical Reactions

The removal of phosphorus is inherently a slag-metal interface reaction that occurs in an oxidizing and basic environment.

**Molecular Form of the Reaction:**

$$2[P] + 5[O] + 3(O^{2-}) \rightarrow 2(PO_4^{3-}) \ \rightarrow \text{  \,(board written)}$$
$$2[P] + 5[O] + 3(CaO)_{slag} \rightleftharpoons (Ca_3(PO_4)_2)_{slag} \ \rightarrow \text{  \,(AI Gen)}$$

**Ionic Form of the Reaction:**

$$[P] + \frac{5}{2}[O] + \frac{3}{2}(O^{2-})_{slag} \rightleftharpoons (PO_4^{3-})_{slag}$$

### B. Equilibrium Constant ($K_{eq}$)

Assuming chemical equilibrium between the metal and the slag, the equilibrium constant for the ionic reaction is given by:

$$K_{eq} = \frac{(a_{PO_4^{3-}})^2}{[h_P]^2 \cdot [h_O]^5 \cdot (a_{O^{2-}})^3}$$

Where:

- $a_{(PO_4^{3-})}$ = Activity of phosphate ion in the slag.
    
- $h_P, h_O$ = Henrian activities of dissolved phosphorus and oxygen in the melt (which are roughly equal to their weight percentages at standard state).
    
- $a_{(O^{2-})}$ = Activity of oxygen ions in the slag (a measure of slag basicity).
    

### C. Equilibrium Partition Coefficient ($L_P$)

We define the equilibrium partition coefficient for phosphorus, $L_P$, as:

$$L_P = \frac{\text{wt\% } (P)_{slag}}{\text{wt\% } [P]_{metal}}$$

From the $K_{eq}$ expression, we can infer that $L_P$ is proportional to:

$$L_P \propto K_{eq} \cdot (h_O)^5 \cdot (a_{O^{2-}})^3$$

### _Conceptual Explanation: Optimum Conditions for De-P_

To maximize $L_P$ (i.e., push the maximum amount of phosphorus into the slag), the following three thermodynamic conditions must be met:

1. **High Oxygen Potential ($h_O$):** An intense oxidizing environment (high dissolved $[O]$ or high $(FeO)$ in the slag) drives the reaction forward. The exponent of 5 indicates a very strong dependence on oxygen.
    
2. **High Slag Basicity ($a_{O^{2-}}$):** A high concentration of basic oxides (like $CaO$) captures the oxidized phosphorus to form stable calcium phosphate.
    
3. **Low Temperature:** The dephosphorization reaction is strongly **exothermic**. According to Le Chatelier's principle, lowering the temperature increases $K_{eq}$ and shifts the equilibrium to the right (product side).
    

_Instructor Note: Contrast this with Desulfurization (De-S), which requires a highly basic but **reducing** environment. Because De-P requires highly **oxidizing** conditions, De-P is ideally suited for the steelmaking converter, whereas De-S is better handled in the blast furnace or via hot metal pretreatment._

---

## 3. Phosphate Capacity and Empirical Relationships

Just as basic slags possess a "Sulfide Capacity" ($C_S$), they also possess a "Phosphate Capacity" ($C_{PO_4^{3-}}$), which quantifies the slag's intrinsic ability to absorb phosphorus.

![[Pasted image 20260221150504.png]]
**Empirical Equation for $L_P$:**

Researchers have established a quantitative relationship for the partition coefficient as a function of temperature, basicity, and oxygen:

$$[\log L_P = \frac{21000}{T} - 9.87 + 0.07 B_O + 2.5 \log(\text{wt\% } [O]) \ ]   \,- \text{No log on photo}$$

Where $B_O$ is a basicity parameter defined as:
 
$$B_O = \text{wt\% } (CaO) + \text{wt\% } (CaF_2) + 0.3 \cdot \text{wt\% } (MgO)$$

_(Note: Calcium fluoride ($CaF_2$) is historically used to fluidize slags, but its use is declining due to environmental restrictions on fluoride contamination)._

### _Visual Extraction: Graphical Relationships_

**Graph 1: Effect of Temperature and Basicity on $L_P$**

![[Pasted image 20260221150809.png]]

```
  log(L_P)
     ^
     |         /  Line A (e.g., 1600 °C) -> Lower T
     |        /
     |       /         / Line B (e.g., 1690 °C) -> Higher T
     |      /         /
     |     /         /
     |    /         /
     |   /         /
     |______________________ V_o (Basicity)
```

_Physical Interpretation:_ For any given basicity ($V_O$ or $B_O$), the partition coefficient ($L_P$) is higher on Line A than Line B. Because the De-P reaction is exothermic, Line A must represent the lower temperature condition.

**Graph 2: Effect of $(FeO)$ Content on Dephosphorization**

![[Pasted image 20260221150830.png]]

```
(wt% P2O5 / wt% [P])
     ^
     |         ___
     |       /     \
     |      /       \
     |     /         \
     |    /           \
     |   /             \
     |__/_______________\_______ wt% (FeO) in slag
             ~ 15%
```

_Physical Interpretation:_ De-P initially increases as $(FeO)$ increases (higher oxygen potential). However, beyond $\sim 15\text{ wt\% } FeO$, the dephosphorization efficiency suddenly drops. To understand why, we must examine the kinetics of slag formation.

---

## 4. Slag Formation and Lime Dissolution Kinetics

The basicity of the slag doesn't magically reach $V = 4$; lime ($CaO$) must physically dissolve into the liquid slag.

- Early in the blow, silicon and iron oxidize rapidly, forming a relatively low-melting acidic/neutral liquid slag: $(FeO \cdot SiO_2)$.
    
- Solid lime ($CaO$) particles are added. They are lighter than the molten metal and float in this initial liquid slag phase.
    

**The Dicalcium Silicate Problem:**

When the solid $CaO$ reacts with the liquid iron-silicate slag, an intermediate chemical reaction occurs at the solid-liquid interface:

$$\text{Solid } CaO + \text{Liquid } (FeO \cdot SiO_2) \rightarrow \text{Liquid Calcium Wüstite} (CaO.FeO)+ \text{Solid Dicalcium Silicate }(Ca_2SiO_4)$$
![[Pasted image 20260221152623.png]]
_Important Remarks:_ Dicalcium silicate precipitates as a fine solid powder exactly at the boundary of the lime particle. This solid precipitate completely coats the unreacted lime particle with an **impervious layer**.

Because the $CaO$ is trapped inside a solid shell, it can no longer dissolve into the bulk slag. Consequently, the bulk slag basicity stops increasing. This is why De-P drops at very high initial $(FeO)$—the $CaO$ cannot dissolve to capture the phosphorus!

### _Phosphorus Reversion_

Towards the end of the steelmaking blow, carbon levels are extremely low. Oxygen instead reacts heavily with iron to form $(FeO)$, releasing a massive amount of heat.

- The sudden spike in bath temperature (exothermic iron oxidation).
    
- Because De-P is favored at low temperatures, this extreme heat forces the phosphate ions to dissociate.
    
- Phosphorus moves from the slag _back_ into the metal (Phosphorus Reversion).
    
- **Conclusion:** Precise "End-Point Control" (stopping the oxygen blow at the exact right moment) is critical to prevent reversion.
    

---

## 5. Kinetics of Steelmaking Reactions

Steelmaking involves multiphase, heterogeneous reactions (gas-metal (eg. $O_2 \rightarrow [O] , + Fe \rightarrow (FeO) \ )$, slag-metal (eg. $[S] + (O^{2-}) \rightarrow (S^{2-}) + [O]$, solid-liquid). These reactions _only_ occur at the phase boundaries as heterogeneous .

**The Five Steps of a Heterogeneous Reaction (Example: De-Sulphurization)**

Consider the reaction: $[S] + (CaO)_{slag} \rightarrow (CaS)_{slag} + [O]$

To complete this reaction, the following sequence must occur in series:

1. **Mass Transfer 1:** Transport of dissolved $[S]$ from the bulk metal to the slag-metal interface.
    
2. **Mass Transfer 2:** Transport of basic $(CaO)$ from the bulk slag to the interface.
    
3. **Chemical Reaction:** Breaking and rearranging of bonds precisely at the interface to form $(CaS)$ and release $[O]$.
    
4. **Mass Transfer 3:** Transport of the product $(CaS)$ away from the interface into the bulk slag.
    
5. **Mass Transfer 4:** Transport of the byproduct $[O]$ away from the interface into the bulk metal.
    

### _Rate-Limiting Step_

Because steelmaking operates at exceptionally high temperatures ($\sim 1600^\circ\text{C}$), the Arrhenius dependency of chemical reaction rates means Step 3 (chemical bond rearrangement) occurs almost instantaneously.

- Therefore, the chemical reaction is almost never the bottleneck.
    
- **The rate-limiting steps are the Mass Transfer steps (1, 2, 4, or 5).** Specifically, diffusion across the boundary layers (not the well-mixed bulk) slows the process down.
    
- **Role of Stirring:** This is exactly why pneumatic oxygen steelmaking is infinitely faster than the older Open Hearth process. Vigorous stirring physically destroys the boundary layers and rapidly continuously supplies fresh reactants to the interface.
  
  
# V2: Detailed 

# Lecture 20: Steelmaking Reactions – Dephosphorization and Kinetics

## I. Introduction to Dephosphorization (De-P)

**Dephosphorization** refers to the removal of phosphorus from hot metal during oxidizing refining (steelmaking).

- **Initial State:** In the blast furnace, almost all phosphorus from the charge materials (iron ore) is reduced and dissolves into the hot metal. Depending on the ore grade, hot metal typically contains **0.1% to 0.15% phosphorus** by weight.
    
- **Target State:** For critical applications, modern primary and secondary steelmaking aims for extremely low final phosphorus levels, typically **30 ppm (0.003 wt%)** or even as low as 10 ppm.
    

---

## II. Thermodynamics of Dephosphorization

### A. Chemical Reaction Equations

Phosphorus removal is a **slag-metal interfacial reaction** that requires both an oxidizing and a basic environment.

**Molecular Form:**

$$2[P] + 5[O] + 3(CaO)_{slag} \rightleftharpoons (Ca_3(PO_4)_2)_{slag}$$

**Ionic Form:**

$$2[P] + 5[O] + 3(O^{2-})_{slag} \rightleftharpoons 2(PO_4^{3-})_{slag}$$

> _Instructor Note:_ The reaction is strictly heterogeneous. Phosphorus and oxygen are dissolved in the metal phase ($[P]$, $[O]$), while the calcium oxide and resulting phosphates exist in the slag phase ($(CaO)$, $(PO_4^{3-})$).

### B. Equilibrium Constant ($K_{eq}$)

Assuming slag-metal equilibrium, the equilibrium constant for the ionic reaction can be written as:

$$K_{eq} = \frac{a_{(PO_4^{3-})}^2}{h_P^2 \cdot h_O^5 \cdot a_{(O^{2-})}^3}$$

Where:

- $a_{(PO_4^{3-})}$ = Activity of the phosphate ion in the slag.
    
- $h_P, h_O$ = Henrian activities of dissolved phosphorus and oxygen in the melt (approximately equal to their weight percentages in a 1 wt% standard state).
    
- $a_{(O^{2-})}$ = Activity of oxygen ions in the slag (a direct measure of slag basicity).
    

### C. Equilibrium Partition Coefficient ($L_P$)

To measure the efficiency of phosphorus removal, we define the **Equilibrium Partition Coefficient ($L_P$)**:

$$L_P = \frac{\text{wt\% }(P)_{slag}}{\text{wt\% }[P]_{metal}}$$

From the $K_{eq}$ expression, we can see that $L_P$ is highly dependent on oxygen potential and basicity:

$$L_P \propto K_{eq} \cdot h_O^5 \cdot a_{(O^{2-})}^3$$

### D. Optimum Conditions for Dephosphorization

To maximize $L_P$ (drive phosphorus into the slag), three essential thermodynamic conditions must be met:

1. **High Oxygen Potential ($h_O$):** Synonymous with high dissolved $[O]$ in the melt or high $(FeO)$ in the slag. The exponent of 5 indicates a massive dependence on oxidizing conditions.
    
2. **High Slag Basicity ($a_{O^{2-}}$):** Abundant basic oxides (like $CaO$) are required to capture the oxidized phosphorus and stabilize it in the slag.
    
3. **Relatively Low Temperature:** The De-P reaction is highly **exothermic**. Lower temperatures favor the forward reaction (increasing $K_{eq}$).
    

> _Conceptual Explanation: De-P vs. De-S_
> 
> Desulfurization (De-S) requires a highly basic but **reducing** environment. Because De-P requires a highly **oxidizing** environment, it is best suited for the steelmaking converter, whereas De-S is better handled in the blast furnace or via hot metal pretreatment.

---

## III. Phosphate Capacity and Empirical Models

Just as slags have a "Sulfide Capacity," they also possess a **Phosphate Capacity**—a thermodynamic parameter indicating the slag's intrinsic ability to absorb phosphorus.

### A. Empirical Equation for $L_P$

Extensive industrial experiments yield empirical relationships to calculate $L_P$. A representative equation is:

$$\log L_P = \frac{21000}{T} - 9.87 + 0.07 V_O + 2.5 \log(\text{wt\% }[O])$$

- **Temperature ($T$):** The positive $21000/T$ term confirms that lower temperatures increase $\log L_P$.
    
- **Basicity Parameter ($V_O$):** A common industrial definition is $V_O = \text{wt\%}(CaO) + 0.03 \cdot \text{wt\%}(CaF_2)$. _(Note: $CaF_2$ usage is currently facing worldwide environmental bans)._
    

### B. Phosphorus Reversion

- **The Phenomenon:** Towards the end of the oxygen blow, carbon is heavily depleted. Oxygen begins to heavily oxidize iron, which is an intensely exothermic reaction.
    
- **The Consequence:** The sudden, drastic increase in bath temperature causes the calcium phosphate in the slag to thermodynamically dissociate. Phosphorus leaves the slag and re-enters the metal. This is known as **Phosphorus Reversion**.
    
- **Solution:** Strict "End-Point Control" (stopping the oxygen blow at the precise target carbon/temperature) is mandatory to prevent reversion.
    

---

## IV. Slag Formation and Lime Dissolution Kinetics

Thermodynamics dictates that high $(FeO)$ and high $(CaO)$ increase De-P. However, kinetically, $L_P$ maxes out at around **15 wt% FeO** and then drops. This is due to the physical mechanics of slag formation.

### A. The Dicalcium Silicate Barrier

1. **Initial Slag:** Early in the blow, oxidized silicon and iron form a liquid iron-silicate slag ($(FeO \cdot SiO_2)$).
    
2. **Lime Addition:** Solid lime ($CaO$) particles are added. They float in the liquid iron-silicate slag.
    
3. **Interfacial Reaction:** At the solid-liquid boundary, they react:
    
    $$\text{Solid } CaO + \text{Liquid } (FeO \cdot SiO_2) \rightarrow \text{Liquid Calcium Wüstite} + \text{Solid Dicalcium Silicate }(Ca_2SiO_4)$$
    
4. **The Choke Point:** The dicalcium silicate precipitates as a solid, fine powder directly on the surface of the lime particle. This forms an **impervious coating** that prevents the inner unreacted lime from dissolving into the bulk slag.
    

> _Physical Interpretation:_ If the $(FeO)$ content is too high ($>15\%$), this solid layer rapidly forms and sinters, locking the $CaO$ away. Even though you added enough lime for a basicity of 4, the _effective_ basicity of the liquid slag remains low because the lime cannot dissolve. Therefore, De-P drops.

---

## V. Kinetics of Steelmaking Reactions

Are these reactions fast enough for industrial production? Steelmaking relies heavily on **heterogeneous, multi-phase reactions** (gas-metal, slag-metal, solid-liquid).

### A. The Five Steps of a Heterogeneous Reaction

Using Desulfurization as an example ($[S] + (CaO) \rightarrow (CaS) + [O]$), the reaction must occur at the exact phase boundary and consists of five sequential steps:

1. **Mass Transfer 1:** Transport of reactant $[S]$ from the bulk metal across the boundary layer to the interface.
    
2. **Mass Transfer 2:** Transport of reactant $(CaO)$ from the bulk slag to the interface.
    
3. **Chemical Reaction:** Breaking and rearranging chemical bonds at the interface to form $(CaS)$.
    
4. **Mass Transfer 3:** Transport of product $(CaS)$ away from the interface into the bulk slag.
    
5. **Mass Transfer 4:** Transport of byproduct $[O]$ away from the interface into the bulk metal.
    

### B. The Rate-Limiting Step

- **Chemical Kinetics are Fast:** Because steelmaking occurs at elevated temperatures ($\sim 1600^\circ\text{C}$), the Arrhenius equation dictates that the chemical reaction step (Step 3) happens almost instantaneously.
    
- **Mass Transfer is Slow:** Therefore, the overall speed of the reaction is entirely governed by the slowest step in the sequence—which is universally **Mass Transfer** (diffusion across the boundary layers).
    

> _Physical Interpretation: The Tea and Sugar Analogy_
> 
> If you put sugar in a cup of tea and do not stir it, the sugar will just sit at the bottom. The chemical potential for dissolution is there, but the mass transfer is too slow. The moment you use a spoon to stir, the sugar dissolves rapidly.
> 
> **Conclusion:** In steelmaking, vigorous stirring/agitation (like injecting oxygen at supersonic speeds) physically shreds the boundary layers, expediting mass transfer and making the refining reactions incredibly fast.
