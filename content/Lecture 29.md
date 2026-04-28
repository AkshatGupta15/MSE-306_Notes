# Lecture 29: Deoxidation of Steel

## 1. Introduction: Tapping and Initial Deoxidation

The primary deoxidation of steel is carried out during the tapping operation, where liquid steel is poured from the primary steelmaking furnace into a ladle.

- **Physical Interpretation:** The initial bulk reduction of dissolved oxygen brings levels down from $\approx 600 \text{ ppm}$ to around $50 - 100 \text{ ppm}$. Deoxidation is done in stages, but tapping handles the largest bulk removal. Final precision adjustments (trimming) are left for downstream Ladle Refining Furnace (LRF) operations. 
    

### Redrawn Board Work: Ladle Deoxidation Mechanism

_The instructor illustrates the tapping process and how stirring drives deoxidation._

Plaintext

```
                  Tap Stream
                 [From Furnace] 
      [Deoxidizers]    |   
             \         |        
              \        |     Slag Layer
   ____________\_______V________________
  |                 o o o o             |
  |               o   |  |   o          |
  |  Ladle      o     |  |     o        |
  |            o      |  |      o       |
  |           o       |  |       o      |
  |           ^       v  v       |      |
  |           |       |  |       |      |
  |           o       |  |       o      |
  |            o      |  |      o       |
  |             o     |  |     o        |
  |               o   |  |   o          |
  |                 o |  | o            |
  |___________________|__|______________|
                      / \
                    Ar Gas 
                (Porous Plug)
```

- **Mechanism:** Deoxidizers in solid form are added directly into the tapping stream. Argon gas is simultaneously bubbled through a porous plug at the ladle's bottom. The bubbles create a vigorous circulatory stirring pattern (plume rising, downward flow near walls), which violently mixes the dissolved deoxidizers with the dissolved oxygen.
    

---

## 2. Selection Criteria for Deoxidizers

To remove dissolved oxygen, elements are added that have a stronger thermodynamic affinity for oxygen than iron does.

- **Thermodynamic Basis (Ellingham Diagram):** Elements whose metal-oxide lines sit lower on the Ellingham diagram form highly stable oxides and act as excellent theoretical deoxidizers [
    
- **Candidates Listed on Board:** $Al, Si, Ca, Na, Mg$
    

**Important Remarks / Instructor Notes:**

- **Affinity Isn't Everything:** While Sodium (Na) and Magnesium (Mg) have massive theoretical affinity for oxygen, they are generally impractical. For example, Sodium has a low boiling point and vaporizes instantly at liquid steel temperatures ($1600^\circ \text{C}$). It evaporates before it can dissolve and react, proving hazardous and completely inefficient. 
    
- **Carbon Restriction:** Carbon reacts with oxygen to form CO gas (a clean, gaseous deoxidation product that easily escapes without leaving inclusions). However, because the overarching goal is usually to produce low-carbon steel, carbon cannot be used as a bulk deoxidizer here.
    
- **Industry Choice:** Due to a balance of moderate price, high recovery rate, lower hazard, and high affinity, **Aluminum (Al)** and **Silicon (Si)** are the principal commercial deoxidizers.
    

---

## 3. Thermodynamics of Deoxidation

Deoxidation involves a physical phase change followed by a chemical reaction.

_Phase Progression:_ $Al_{(s)} \rightarrow Al_{(l)} \rightarrow [Al]_{dissolved}$

_Reaction:_ $2[Al] + 3[O] \rightleftharpoons (Al_2O_3)_{(s)}$

### Extracted Board Work: Equilibrium Constants 

The assumption of thermodynamic equilibrium is highly accurate due to the high temperatures ($1600^\circ \text{C}$) and rapid rates of mass transfer, heat transfer, and heterogeneous nucleation.

**General Equilibrium Equation:**

$$K_{eq} = \frac{a_{Al_2O_3(s)}}{h_{[Al]}^2 \cdot h_{[O]}^3}$$

_(Where $a$ is activity, assumed to be 1 for pure solid $Al_2O_3$, and $h$ is the Henrian activity of dissolved species)_

**Equations on Board at $1600^\circ \text{C}$:**

General Form: $\log K_{eq} = \frac{A}{T} - B$

1. **Aluminum:** $\log K_{eq, Al-Al_2O_3} = 17.32$
    
2. **Silicon:** $\log K_{eq, Si-SiO_2} = 4.62$
    

- **Physical Interpretation:** The equilibrium constant for Aluminum ($10^{17.32}$) is exponentially larger than that of Silicon ($10^{4.62}$). This mathematically proves Aluminum is a far more powerful deoxidizer. To achieve an ultra-low target oxygen level (e.g., $10 \text{ ppm}$), only Aluminum is strong enough; Silicon would require an unacceptably high residual concentration in the steel to drive the equilibrium that far. 
    

---

## 4. Types of Deoxidation: Simple vs. Complex

The instructor defines two distinct methods of treating the steel, written on the board around 

**1. Simple Deoxidation**

Using a single element (e.g., adding pure Aluminum or Ferrosilicon) to drive out oxygen. The resulting solid product ($Al_2O_3$ or $SiO_2$) is a pure phase, meaning its thermodynamic activity is unity ($a = 1$).

**2. Complex Deoxidation**

Using two or more elements combined, typically Silicon and Manganese added via Silico-Manganese ($SiMn$).

- _Reaction:_ $SiO_2 + MnO \rightarrow MnO\cdot SiO_2$ (Liquid Manganese Silicate)
    
- **Conceptual Explanation of Advantage:** When $SiO_2$ and $MnO$ combine into a liquid silicate, they are no longer in their pure standard states, meaning their individual activities drop **below 1** ($a_{SiO_2} < 1$).
    
- Looking at the silicon equilibrium constant: $K_{eq} = \frac{a_{SiO_2}}{h_{[Si]} \cdot h_{[O]}^2}$. Because $a_{SiO_2}$ is lowered, the reaction is forced to shift to the right. This allows the operator to reach the target $[O]$ level using _less_ total silicon, reducing the unwanted residual silicon contamination in the final steel.
    

---

## 5. Material Balance for Deoxidizer Additions

A theoretical material balance determines exactly how much deoxidizer must be added to a ladle to hit target oxygen ppm. 

**Total Aluminum Requirement Equation (Expanded):**

$$W_{Al,\text{ Total}} = W_{Al \text{ in } Al_2O_3} + W_{[Al] \text{ dissolved}} + W_{Al \text{ lost}}$$

**Step-by-step Calculation:**

1. **Find Oxygen Removed:** Calculate $\Delta [O] = [O]_{initial} - [O]_{target}$ (e.g., $600 \text{ ppm} \rightarrow 20 \text{ ppm} = 580 \text{ ppm}$ removed).
    
2. **Stoichiometric Aluminum:** Convert the $580 \text{ ppm}$ of removed oxygen into the stoichiometric mass of Aluminum tied up in the newly formed $Al_2O_3$.
    
3. **Equilibrium Aluminum:** Use the $K_{eq}$ formula (with $[O] = 20 \text{ ppm}$) to solve for the residual $h_{[Al]}$. This dictates the mass of Aluminum that will remain permanently dissolved in the steel.
    
4. **Buffer for Losses:** Add an empirical buffer (approx. $\pm 5\%$) to account for Aluminum oxidizing against reducible oxides in the slag (e.g., reacting with $FeO$) rather than the melt.
    

- **Important Remark for Complex Deoxidation:** Calculating the required addition for $SiMn$ is far more mathematically rigorous. Because $a_{SiO_2} \neq 1$, engineers must consult an **Activity-Composition Phase Diagram** for the $MnO-SiO_2$ binary system to deduce the exact activities before solving the $K_{eq}$ expression.
    

---

## 6. Flotation Kinetics and Steel Cleanliness

Deoxidation products must float out of the steel into the slag. Products that remain permanently trapped in the solid steel are called **inclusions**, which severely impair mechanical performance and fatigue life (e.g., in ball bearing steels).

**Stokes' Law (Visual & Audio Extraction):**

The terminal rise velocity of an inclusion particle dictates if it will float out in time.

$$v_{rise} \propto g \cdot d_p^2 \cdot \Delta \rho$$

_(Where $d_p$ is particle diameter and $\Delta \rho$ is the density difference between the inclusion and liquid steel)_

**Physical Interpretation of Product Phase:**

- **Liquid Products (Highly Preferred):** Products like liquid Manganese Silicate easily undergo _coalescence_ (coagulation). When droplets collide, they merge, drastically increasing $d_p$. Because rise velocity scales with the **square** of the diameter ($d_p^2$), liquid inclusions float out of the ladle rapidly.
    
- **Solid Products (Problematic):** Solid $Al_2O_3$ particles do not coalesce upon collision. They remain as small individual particles ($\approx 10 - 20 \mu m$) with very low rise velocities, meaning they often fail to reach the slag and remain entrapped.
    
- _Note:_ Particles reaching $\approx 100 - 140 \mu m$ boast nearly a $100\%$ removal efficiency, clearing the bath in just 4 to 5 minutes.
    

---

## 7. Classification of Inclusions

Inclusions in steel are categorized by their physical origin: 

1. **Endogenous Inclusions:**
    
    - Originate from _within_ the melt via internal chemical reactions.
        
    - **Examples:** $Al_2O_3$ and $SiO_2$ formed directly as a result of the deoxidation process.
        
    - _Challenge:_ The primary hurdle in achieving "clean steel," requiring heavy process engineering (like future calcium injection) to remove.
        
2. **Exogenous Inclusions:**
    
    - Originate from _outside_ the melt system.
        
    - **Examples:** Entrapped pieces of slag or eroded ladle refractory material.
        
    - _Identification:_ Usually identified spectroscopically by tracing compounds not added intentionally (e.g., observing $MgO$ inclusions, which strictly come from ladle refractory linings).
        
    - _Challenge:_ In modern steelmaking with advanced refractory wear resistance, these are significantly less problematic than endogenous inclusions.
      
# Audio V2 

# Lecture Notes: Deoxidation of Steel

## 1. Overview of Deoxidation (During Tapping)
Deoxidation is the process of removing dissolved oxygen from liquid steel. 
* **Primary Stage:** The first bulk reduction of dissolved oxygen is carried out in the ladle during the tapping operation from the furnace. 
* **Target Reduction:** Oxygen levels are typically brought down from around **600 ppm** to **50 - 100 ppm** during this stage. Final "trim" adjustments are made in subsequent ladle refining stages (LRF).
* **Ladle Environment:** The molten metal fills the ladle, leaving a "freeboard height." Argon gas (non-reactive) is bubbled through a porous plug to create vigorous **gas stirring**, which mixes the deoxidizers with the dissolved oxygen.

## 2. Selection Criteria for Deoxidizers
Deoxidizers are elements added to steel that have a stronger affinity for oxygen than iron does.

* **The Ellingham Diagram:** Elements whose metal/metal-oxide lines are situated lower on the Ellingham diagram (meaning they form highly stable oxides) are theoretical candidates. 
    * *Candidates include:* $Al$, $Si$, $Ca$, $Na$, $Mg$.
* **Practical Considerations (Why Affinity Isn't Enough):**
    * **Vaporization & Hazards:** Sodium ($Na$) has great oxygen affinity but a very low boiling point. If added to steel at **1600°C**, it vaporizes instantly, acting hazardously and escaping the system before reacting.
    * **Price and Recovery:** The cost of the material and how much actually dissolves into the steel (recovery) are critical.
* **Industry Standard:** **Aluminum ($Al$)** and **Silicon ($Si$)** are the primary choices because they balance high oxygen affinity, moderate price, less hazardous addition, and high recovery rates. Carbon is not used because the goal is usually to produce low-carbon steel.

## 3. Mechanism of Addition and Reaction
Deoxidizers are added as solids into the liquid steel. 
* **Phase Progression:** $Solid \rightarrow Liquid \rightarrow Dissolved$
* **Reaction Sequence:** The solid element melts (e.g., Al melts around **800°C**), dissolves into the melt via convection, and then collides with dissolved oxygen.
* **Nucleation and Growth:** The reaction forms a completely new phase (a solid or liquid oxide, e.g., $Al_2O_3$). This requires critical nuclei to form and grow.
* **Purity of Additives:** * Aluminum is usually added in pure commercial form.
    * Silicon is **never** added as pure silicon; it is added as **Ferrosilicon** (high or low carbon) or **Silico-manganese**. 
    * *Important Note:* The impurities in ferrosilicon matter. For example, the trace calcium content in ferrosilicon will heavily influence the efficacy of later calcium injection treatments.

## 4. Thermodynamics: Simple vs. Complex Deoxidation

### Simple Deoxidation
Using a single powerful element, typically Aluminum.
* **Reaction:** $2[Al] + 3[O] \rightleftharpoons Al_2O_3$
* **Equilibrium Constant:**
  $$K_{eq} = \frac{a_{Al_2O_3}}{h_{[Al]}^2 \cdot h_{[O]}^3}$$
  *(Where $a$ is activity and $h$ is Henrian activity).* * Because pure solid $Al_2O_3$ forms, its activity is equal to $1$ ($a_{Al_2O_3} = 1$).
* **Strength of Al:** At **1600°C**, the $\log K_{eq}$ for Aluminum is $\approx 17.32$, while for Silicon it is $\approx 4.62$. Aluminum is vastly more powerful. 
    * *Example:* To achieve **10 ppm** oxygen, it would take nearly **10 wt%** Manganese, but only about **400 ppm** Aluminum.
* **LCAK Steel:** "Low Carbon Aluminum Killed" steel. "Killing" means completely removing free dissolved oxygen to prevent carbon-oxygen gas reactions during solidification.

### Complex Deoxidation
Using two or more elements combined, typically Silico-manganese ($SiMn$).
* **Mechanism:** $Si$ and $Mn$ react with oxygen simultaneously to form $SiO_2$ and $MnO$. These two oxides combine to form **Manganese Silicate** ($MnO \cdot SiO_2$).
* If engineered correctly (approx. **55 wt%** $MnO$ to **45 wt%** $SiO_2$), this produces a **liquid** deoxidation product.
* **Thermodynamic Advantage:** Because the $SiO_2$ is consumed by the $MnO$, its activity drops below $1$ ($a_{SiO_2} < 1$). This shifts the chemical equilibrium to the right, driving out more oxygen while leaving *less* residual Silicon in the steel. 

## 5. Material Balance and Calculations
To calculate the exact amount of deoxidizer needed, engineers use a mass balance equation:
* **Total Aluminum Required =** $(Al \text{ tied up in } Al_2O_3) + (Al \text{ dissolved in steel}) + (\text{Losses})$
* **Step-by-Step Breakdown:**
    1. **Stoichiometric conversion:** Calculate how much $Al$ is consumed based on the target oxygen drop (e.g., dropping from **600 ppm** to **20 ppm** means **580 ppm** of oxygen reacts to form $Al_2O_3$).
    2. **Equilibrium calculation:** Calculate the necessary residual dissolved $Al$ required to keep the remaining oxygen at the target **20 ppm** using the $K_{eq}$ formula.
    3. **Account for losses:** Add an empirical buffer (e.g., $\approx \pm 5\%$) to account for Al reacting with reducible oxides in the slag, like $FeO$.
* **Complex Calculation Requirement:** If using Silico-manganese, you cannot assume an activity of $1$ for the products. You must consult an **Activity-Composition Phase Diagram** (for the $MnO-SiO_2$ binary system) to find the correct activities of $SiO_2$ and $MnO$ before solving the equilibrium equations.

## 6. Flotation Kinetics and Steel Cleanliness
Deoxidation products are lighter than liquid steel and naturally float to the top to be absorbed by the liquid slag. Clean steel is defined by the absence of trapped deoxidation products.

* **Stokes' Law:** Controls the terminal rise velocity of the products:
  $$v \propto g \cdot d_p^2 \cdot \Delta\rho$$
  *(Where $g$ is gravity, $d_p$ is particle diameter, and $\Delta\rho$ is the density difference between the inclusion and liquid steel).*
* **Liquid vs. Solid Products:**
    * **Liquid Products** (e.g., Manganese Silicate): Highly preferred. Liquid droplets easily collide and **coalesce** (merge together). If particle diameter doubles, the rise velocity increases by a factor of 4, meaning they float out rapidly.
    * **Solid Products** (e.g., $Al_2O_3$): Disadvantageous. They do not easily coalesce upon collision. They remain as small particles and float out very slowly, risking entrapment.
* **Removal Efficiency:** Particles that reach $\approx$ **100 to 140 microns** have nearly $100\%$ removal efficiency, clearing the bath to the slag in roughly **4 to 5 minutes**. 

## 7. Types of Inclusions
Particles that fail to float out and remain permanently trapped in the steel are called **inclusions**. They degrade mechanical properties, service life, and fatigue strength (e.g., ball bearing steel strictly requires inclusions to be $< \mathbf{20 \text{ microns}}$).

1. **Endogenous Inclusions:** * Originate from *within* the melt due to internal chemical reactions. 
   * *Example:* The $Al_2O_3$ particles generated strictly by the deoxidation process. This is the primary challenge in modern clean steelmaking.
2. **Exogenous Inclusions:** * Originate from *outside* the melt system.
   * *Example:* A piece of eroded refractory lining from the ladle walls falling into the steel. These can be identified under a microscope if they contain compounds not added to the steel (like $MgO$, which comes strictly from refractory bricks). Good steelmaking practices have largely minimized exogenous inclusions.