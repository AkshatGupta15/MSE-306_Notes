# **Lecture 18: Evolution and Thermodynamics of Primary Steelmaking**

## **1. Introduction: The Transition to Steelmaking**

After covering Ironmaking, the course shifts to **Steelmaking** (Primary and Secondary).

- **The Goal of Steelmaking:** To refine Hot Metal (Pig Iron) into Crude Steel by adjusting its composition and ensuring "cleanliness" (removing dissolved impurities like C, Si, Mn, P).
    
- **Autogenous Nature:** Primary steelmaking requires **no external heat source**. The exothermic oxidation of dissolved metalloids (Carbon and Silicon) provides the necessary heat to raise the bath temperature from $\sim1400^\circ\text{C}$ to the tapping temperature of $1600^\circ\text{C} - 1620^\circ\text{C}$.
    
- **Superheat:** The extra heat generated provides a "superheat" (defined as the excess temperature above the liquidus temperature, typically $\sim70-80^\circ\text{C}$). This thermal buffer is critical as it compensates for the heat losses that will occur during subsequent secondary steelmaking processes.
    

![[Pasted image 20260221022300.png]]
---

## **2. Historical Evolution of Steelmaking Processes**

### **A. Early Methods (Pre-1850)**

- **Wrought Iron:** Solid iron was melted and mixed with iron oxide ($FeO$) to oxidize the carbon. The entrapped slag was removed by mechanical hammering (e.g., used for Damascus swords).
    

### **B. The Pneumatic Era (1850s)**

- **The Bessemer Process (~1850-1860):** * Sir Henry Bessemer commercialized the first mass-production pneumatic process.
    
    - _Mechanism:_ Air was blown through the bottom of the molten iron via tuyeres.
        
    - _Lining:_ Used an **Acidic** lining (Silica).
        
    - _Drawback:_ Because air is 79% Nitrogen, the steel absorbed a massive amount of $N_2$ (equilibrium at $1600^\circ\text{C}$ is $\sim 7800 \text{ ppm}$). Nitrogen makes steel hard and brittle, rendering it useless for applications like deep drawing. Nitrogen also acts as a massive thermal sink, carrying heat out of the furnace.
        
- **The Thomas Process (1868):**
    
    - Also known as the "Basic Bessemer" process.
        
    - Used a **Basic** lining (MgO/CaO), which allowed for the addition of lime (CaO) flux. This enabled the removal of Phosphorus (which is impossible in an acidic vessel).
        

### **C. The Open Hearth Era (Siemens-Martin Process)**

- _Mechanism:_ A shallow bath reactor where oxidation was achieved using **Iron Ore ($FeO/Fe_2O_3$)** instead of an air blast.
    
- _Advantage:_ Produced much higher purity steel (free from $N_2$ contamination).
    
- _Disadvantage:_ The reaction with $FeO$ is endothermic (or only weakly exothermic). It was **not autogenous**. It required external fuel/burners and utilized complex brick checker-work (heat recuperators) to save energy. Furthermore, the lack of intense agitation (only occasional $CO$ bubbles rising) meant the kinetics were very slow, leading to long processing times.
    

### **D. Duplex Steelmaking**

- To combine the speed of Bessemer with the quality of Open Hearth, plants used a "Duplex" process: **Acid Bessemer + Basic Open Hearth**. (Tata Steel in Jamshedpur utilized this up to the 1980s).
    

### **E. Electric Arc Furnace (EAF) (1940s)**

- Emerged heavily after WWII to consume the massive amounts of generated steel scrap. Today, it accounts for **35-40%** of global steel production and is highly versatile (capacities from 30 to 300 tons), making it ideal for specialty and alloy steels.
    

---

## **3. The Modern Era: Basic Oxygen Steelmaking (BOS/BOF)**

_Conceptual Explanation:_ While Bessemer knew pure oxygen would be superior to air, pure $O_2$ isolation wasn't viable until 1930, and it took until **1952** (the LD process in Austria) to commercialize the oxygen converter. Injecting pure oxygen into an iron blast furnace is disastrous, and designing a vessel to handle direct oxygen lancing into molten metal required extensive engineering.

Today, **Basic Oxygen Steelmaking (BOS)** accounts for **~60%** of global steel.

- **Basic Lining:** _All_ modern oxygen converters use a basic refractory lining (e.g., Magnesite/MgO) to withstand the high temperatures and highly basic slags needed for dephosphorization.
    
- **Advantages of Pure Oxygen (Top Lance):**
    
    1. **No Nitrogen Heat Sink:** Generates immense surplus heat, allowing the plant to melt up to 20-30% cold steel scrap.
        
    2. **No Nitrogen Contamination:** Produces deep-drawing quality steel.
        
    3. **Ultra-Low Carbon:** The high oxygen potential can drive carbon down to "dead soft" levels.
        
    4. **Rapid Kinetics:** Intense stirring allows 200–300 tons of crude steel to be refined in just $\sim45$ minutes.
        

---

## **4. Thermodynamics of Refining Reactions**

### **Compositional Shift (Hot Metal to Crude Steel)**

|**Element**|**Hot Metal**|**Crude Steel**|
|---|---|---|
|**Carbon (C)**|$\sim 4.3\%$|$\sim 0.1\%$ (medium C grade)|
|**Silicon (Si)**|$0.4 - 2.5\%$|$\sim 0\%$|
|**Manganese (Mn)**|$0.2 - 0.4\%$|$\sim 0.1\%$|
|**Phosphorus (P)**|Max $0.1\%$|$\sim 0.04\%$|
|**Oxygen (O)**|Traces|$\sim \textbf{0.06\% (600 ppm)}$|

_Instructor Note:_ Primary steelmaking is heavily **oxidizing**. You successfully remove C, Si, Mn, and P, but the "price you pay" is heavily oxygenating the steel ($\sim 600 \text{ ppm}$). This dissolved oxygen must be removed later during secondary steelmaking to reach the final cleanliness target ($\sim 100 \text{ ppm}$ total impurities).

### **Ellingham Diagram Analysis at $1600^\circ\text{C}$**

If oxygen is blown into the hot metal, the thermodynamic affinity dictates the order of oxidation:

1. **Silicon ($Si$)** oxidizes first (very high affinity).
    
2. **Manganese ($Mn$)** and **Phosphorus ($P$)** follow.
    
3. **Iron ($Fe$)** oxidizes to $FeO$. Because the environment is so highly oxidizing, a significant portion of Iron is lost. _Unlike the Blast Furnace slag which contains $<0.1\% FeO$, BOF slag contains $15\% - 25\% FeO$._

![[Pasted image 20260221022116.png]]

---

## **5. Carbon-Oxygen Reactions & Kinetics**

Carbon oxidation is the defining reaction of steelmaking. There are five possible reaction pathways occurring simultaneously in the converter:

**1. Oxygen Dissolution (Gas-Metal):**

$$\frac{1}{2}O_2(g) \rightleftharpoons [O]$$

_(Note: At $1600^\circ\text{C}$, pure iron can dissolve up to $2300 \text{ ppm}$ of oxygen)._

**2. Homogeneous Melt Reaction:**

$$[C] + [O] \rightleftharpoons CO(g)$$

**3. Direct Gas-Metal Oxidation:**

$$\frac{1}{2}O_2(g) + [C] \rightleftharpoons CO(g)$$

_(Probability of this is remote because the melt is 95% Fe atoms and only ~4% C atoms)._

**4. Iron Oxidation (Gas-Metal):**

$$\frac{1}{2}O_2(g) + [Fe] \rightleftharpoons (FeO)$$

**5. Slag-Metal Reaction:**

$$(FeO) + [C] \rightleftharpoons CO(g) + [Fe]$$

_Physical Interpretation:_ Because of the intense agitation in the BOF, reactions **#2** (dissolved C + dissolved O) and **#5** (Slag FeO + dissolved C) are the **predominant mechanisms** for carbon elimination.

**Post-Combustion:** The $CO(g)$ escaping the bath can react with entrained air at the mouth of the converter to form $CO_2$. Harnessing this wasted post-combustion heat back into the melt is a major focus in modern BOF design.

---

## **6. Thermodynamic Equilibrium of the C-O Reaction**

To determine if the C-O reaction inside the highly dynamic BOF is close to equilibrium, we analyze the equilibrium constant ($K_{CO}$) for the reaction $[C] + [O] \rightleftharpoons CO(g)$:

$$K_{CO} = \frac{P_{CO}}{a_C \cdot a_O} = \frac{P_{CO}}{[\%C] \cdot f_C \cdot [\%O] \cdot f_O}$$

**Assumptions for analysis:**

1. Operating at standard steelmaking temperature: $T = 1600^\circ\text{C}$.
    
2. Total pressure $P_T = P_{CO} \approx 1 \text{ atm}$.
    
3. In dilute solutions, the activity coefficients approach unity ($f_C \approx 1, f_O \approx 1$).
    

Substituting these into the equilibrium expression gives a simplified hyperbolic relationship:

$$[\%C] \times [\%O] = \text{Constant}$$

### **Board Graph: $[\%O]$ vs. $[\%C]$**

Plaintext

```
  [%O]
   |
   |
   | * (Data point)
   |  \
   |   \  * (Data point)
   |    \
   |     \   *
   |      \____ * ____ * ______ Theoretical Hyperbola 
   |                           ([%C] * [%O] = 2.25 x 10^-3)
   |_________________________________ [%C]
```

**Verification against actual plant data:**

Using oxygen determinators and spectroscopic samples taken directly from active Oxygen Converters, metallurgists plotted actual plant data against this theoretical curve.

- **Conclusion:** The real-world data points lie almost perfectly on the theoretical curve. This proves that despite the violent, highly kinetic environment of the oxygen converter, **the Carbon-Oxygen reaction operates very close to thermodynamic equilibrium.**


# V2: Detailed 

Here are the detailed, exhaustive notes extracted from the lecture transcript, capturing every concept, historical context, and technical explanation provided.

# **Lecture 18: Evolution and Thermodynamics of Primary Steelmaking**

## **1. Course Roadmap & Introduction to Steelmaking**

- **Course Progress:** 17 lectures were dedicated to Ironmaking. The next 17-18 lectures will cover Steelmaking. The final 3-4 lectures will be tutorials solving problems related to material balance, energy balance, and thermodynamics/kinetics.
    
- **The Goal of Steelmaking:** Hot metal (pig iron) is an intermediate product. Primary steelmaking refines it into crude steel by adjusting its composition. Secondary steelmaking follows to control the final composition and "cleanliness" (removing dissolved impurities to very low ppm levels).
    
- **Autogenous Nature:** Primary steelmaking requires **no external heat source**. The exothermic oxidation of dissolved metalloids (like Carbon and Silicon) provides the necessary heat to raise the bath temperature from $\sim1400^\circ\text{C}$ to the tapping temperature of $1600^\circ\text{C} - 1620^\circ\text{C}$.
    
- **Superheat:** The extra heat generated provides a "superheat" (defined as the excess temperature above the liquidus temperature, typically $\sim70-80^\circ\text{C}$). This thermal buffer is critical to compensate for heat losses during subsequent secondary steelmaking processes, ensuring the metal remains liquid.
    

---

## **2. Historical Evolution of Steelmaking**

### **A. Early Methods (Pre-1850s)**

- **Wrought Iron:** Solid iron was melted and mixed with iron oxide ($FeO$) to oxidize the carbon. The entrapped slag was removed mechanically by hammering (e.g., Damascus swords).
    

### **B. The Pneumatic Era (1850s - 1860s)**

![Bessemer converter, AI generated](https://encrypted-tbn1.gstatic.com/licensed-image?q=tbn:ANd9GcT333nLytZYB8HjWVukgsV-jGkMCGo_2RSBF235Uw7y_j91KzH9NjUmhQPcS4knYI3Z2Na1CrlH4dc0hyFmVL-YmLGBWzElZBHB3Vafc-tWh4WQYi8)


![[Pasted image 20260220235617.png]]

- **The Bessemer Process (~1850-1860):** Sir Henry Bessemer commercialized the first mass-production pneumatic steelmaking process.
    
    - **Mechanism:** Air was blown through the bottom of the molten iron via tuyeres (vertical tubes).
        
    - **Lining:** Used an **Acidic** lining (Silica).
        
    - **Drawback (Nitrogen Contamination):** Because air is 79% Nitrogen, the steel absorbed a massive amount of $N_2$ (equilibrium at $1600^\circ\text{C}$ with air is $\sim 7800 \text{ ppm}$). Nitrogen makes steel hard and brittle, rendering it useless for applications like deep drawing. Nitrogen also acted as a massive thermal sink, carrying heat out of the furnace.

    - heat economy not favourable - heat loss 
        
- **The Thomas Process (1868):**
    
    - Also known as the "Basic Bessemer" process.
        
    - **Modification:** Used a **Basic** lining (MgO/CaO). This allowed for the addition of basic fluxes like lime (CaO), which enabled the removal of Phosphorus (which is chemically impossible in an acidic vessel because basic fluxes would destroy an acidic silica lining).
        

### **C. The Open Hearth Era (Siemens-Martin Process)**

![Open Hearth furnace, AI generated](https://encrypted-tbn0.gstatic.com/licensed-image?q=tbn:ANd9GcQVjGoTLkfWuWv0YKGtTYbexlw-9lOdy4tes_qNC-RjOGmyQuhZbJgElv83UNdwGabGIyyPd77IF7D4l5u-O4KukTl20dfg0jcYVxhUwsh_jfsWKtM)


- **Mechanism:** A shallow bath reactor where oxidation was achieved using **Iron Ore ($FeO/Fe_2O_3$)** instead of an air blast.
    
- **Advantage:** Produced much higher purity steel because it eliminated Nitrogen contamination and reduced dissolved oxygen.
    
- **Disadvantage (Heat & Time):** The reaction with $FeO$ is endothermic (or only very weakly exothermic compared to pure oxygen). It was **not autogenous**. It required external fuel/burners.
    
- **Heat Recovery:** It utilized complex brick checker-work (heat recuperators/regenerators, similar to blast furnace stoves) to capture heat from exiting $CO$ gas to preheat incoming air.
    
- **Kinetics:** Very slow. There was no intense gas-induced stirring (only occasional $CO$ bubbles rising "like a Coca-Cola bottle"). The slow kinetics meant long processing times per heat.
    

### **D. Duplex Steelmaking**

- To combine the rapid production speed of the Bessemer process with the high quality of the Open Hearth process, plants used "Duplexing": **Acid Bessemer + Basic Open Hearth**. (Tata Steel in Jamshedpur utilized this up to the 1980s).
    

### **E. Electric Arc Furnace (EAF) (1940s)**

- Emerged heavily after WWII (1940s-1945) to consume the massive amounts of steel scrap generated during the war. Open hearths couldn't easily melt this scrap without burning excessive fuel.
    

---

## **3. The Modern Era: Basic Oxygen Steelmaking (BOS/BOF)**

While Bessemer knew pure oxygen would be superior to air, pure $O_2$ isolation wasn't viable until 1930. Injecting pure oxygen directly into blast furnaces or early converters was disastrous without proper engineering. It took until **1952** (commercialized in Austria) for the modern oxygen converter (top-blown) to emerge.

Today, only two technologies dominate, producing ~98% of global steel:

1. **Basic Oxygen Steelmaking (BOS / BOF):** ~60% of global production. (Capacities: 250–500 tons).
    
2. **Electric Arc Furnace (EAF):** ~35-40% of global production. Handles smaller batches (30–300 tons) and specializes in recycling scrap/DRI and producing high-end/specialty steels.
    

**Note on Terminology:** Today, _all_ primary steelmaking is basic. Acidic steelmaking is completely obsolete. Therefore, "Oxygen Steelmaking" inherently implies a basic lining (MgO-based) to handle basic slags.

$O_2$ Added from top unlike old from bottom
### **Advantages of Pure Oxygen Injection (BOF)**

1. **No Nitrogen Heat Sink:** Without nitrogen stealing heat, there is an immense surplus of thermal energy.
    
2. **Scrap Melting:** This surplus heat allows the plant to charge and melt cheap, in-house steel scrap (up to 20-30% of the charge).
    
3. **High Quality:** Zero nitrogen contamination allows for the production of deep-drawing quality steel.
    
4. **Ultra-Low Carbon:** The extremely high oxygen partial pressure can drive carbon down to "dead soft" levels.
    
5. **Rapid Kinetics:** The intense gas-metal-slag stirring allows 200–300 tons of crude steel to be refined in a flat 45 minutes, dramatically improving process economics.
   (Even faster than Bessemers as pure $O_2$)
    

---

## **4. Thermodynamics of Refining Reactions**

### **Ellingham Diagram Analysis at $1600^\circ\text{C}$**

Primary steelmaking is a highly **oxidizing** environment (unlike the reducing environment of the Blast Furnace).

- Oxygen has a great thermodynamic affinity for the impurities: **Silicon, Manganese, Carbon, and Phosphorus.**
  _(Sulphur not written steelmaking oxidising environment where iron making carried out in reducing environment)_
    
- Upon injecting oxygen:
    
    - **Silicon** oxidizes first forming $SiO_2$ (fixed into slag by $CaO$).
        
    - **Phosphorus** oxidizes to $P_2O_5$ (fixed by $CaO$ into Calcium Phosphate).
        
    - **Manganese** oxidizes to $MnO$.
        
    - **Carbon** oxidizes to $CO$ gas.
        
- **Iron Loss:** Because the environment is so highly oxidizing, Iron ($Fe$) also oxidizes. While Blast Furnace slag contains $<0.1\% FeO$, **BOF slag contains a massive 15% to 25% $FeO$**, representing a significant yield loss.
    

---

## **5. Carbon-Oxygen Reaction Mechanisms**

Carbon oxidation is the defining reaction of steelmaking. There are five possible reaction pathways occurring simultaneously in the converter bath:

1. **Oxygen Dissolution (Gas-Metal):** $\frac{1}{2}O_2(g) \rightleftharpoons [O]$ _(At $1600^\circ\text{C}$, liquid iron can dissolve up to 2300 ppm of oxygen)._
    
2. **Homogeneous Melt Reaction:** $[C] + [O] \rightleftharpoons CO(g)$
    
3. **Direct Gas-Metal Oxidation:** $\frac{1}{2}O_2(g) + [C] \rightleftharpoons CO(g)$ _(Probability is remote because the melt is 95% Fe atoms and only ~4-5% C atoms)._
    
4. **Iron Oxidation (Gas-Metal):** $\frac{1}{2}O_2(g) + [Fe] \rightleftharpoons (FeO)$
    
5. **Slag-Metal Reaction:** $(FeO) + [C] \rightleftharpoons CO(g) + [Fe]$
    

**Predominant Mechanisms:** Due to intense agitation in the BOF, reactions **#2** (dissolved C + dissolved O) and **#5** (Slag FeO + dissolved C) are the primary drivers for carbon elimination.

**Post-Combustion:** The $CO(g)$ that escapes the bath carries away massive sensible heat. If it reacts with entrained atmospheric oxygen at the mouth of the converter, it undergoes post-combustion: $CO + \frac{1}{2}O_2 \rightarrow CO_2$. Modern engineering attempts to force this post-combustion to happen _inside_ the furnace vessel to harness this heat back into the melt.

---

## **6. Thermodynamic Equilibrium o

$$\frac{1}{2}O_2 \rightleftharpoons [O] \rightarrow \Delta G_1$$
$$[O] + [C] \rightleftharpoons \{CO\} \rightarrow \Delta G_2$$ $$\frac{1}{2}O_2  + [C] \rightleftharpoons \{CO\} \rightarrow \Delta G_1 + \Delta G_2$$

To evaluate if the Carbon-Oxygen reaction is operating near equilibrium inside the highly dynamic BOF, we analyze the equilibrium constant ($K_{CO}$) for the reaction $[C] + [O] \rightleftharpoons CO(g)$:

$$K_{CO} = \frac{\{P_{CO}\}}{[h_C] \cdot [h_O]} = \frac{P_{CO}}{[wt \%C] \cdot f_C \cdot [wt \%O] \cdot f_O}$$
$$\Delta G_2^\circ = -RT \cdot ln K_{CO}$$

**Conditions and Assumptions:**

1. **Standard Temperature:** $T = 1600^\circ\text{C}$ (Standard benchmark for analysis, though operations span $1550^\circ\text{C}$ to $1650^\circ\text{C}$).
    
2. **Pressure:** Total pressure $P_T = P_{CO} \approx 1 \text{ atm}$.
    
3. **Dilute Solutions:** For low concentrations (roughly ~1 wt% scale), there is linearity, and the activity coefficients ($f_C, f_O$) approximate to $1$.
    

Substituting these conditions into the expression yields a hyperbolic relationship:

$$[\%C] \times [\%O] = \text{Constant}$$

_At $1600^\circ\text{C}$, thermodynamic handbooks (using standard free energy $\Delta G^\circ = -RT \ln K$) define this constant as:_

$$[\%C] \times [\%O] = 2.25 \times 10^{-3}$$
![[Pasted image 20260221021941.png]]

**Plant Validation:**

When metallurgists take live samples from active oxygen converters using oxygen determinators and spectroscopic methods, the actual plotted data points (Actual $[\%O]$ vs. $[\%C]$) lie almost perfectly on this theoretical hyperbolic curve.

**Conclusion:** This proves that despite the violent, highly kinetic, fast-paced environment of the oxygen converter, the **Carbon-Oxygen reaction operates very close to true thermodynamic equilibrium.**