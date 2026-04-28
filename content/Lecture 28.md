# LECTURE 28: Stainless Steelmaking and Tapping Operations

## 1. Introduction to Stainless Steel

### Conceptual Explanation

Stainless steel is defined by its excellent anti-corrosion (rusting) properties. It is increasingly replacing traditional materials (e.g., wood in kitchen cabinets, carbon steel in railway wagons) due to its life-long durability and resistance to environmental degradation.

### Classification of Stainless Steels

Stainless steels are categorized by their principal alloying elements:

- **300 Series (Austenitic):** Chromium-Nickel based (e.g., standard "18-8" contains 18% Cr and 8% Ni). This is the highest quality, most common in premium utensils, and possesses excellent deep drawing qualities. Some premium grades go up to 24% Ni.
    
- **200 Series:** Chromium-Manganese based. Nickel is replaced by Manganese to reduce costs. _Warning / Instructor Note:_ This variety is cheaper but prone to developing cracks and suffers in deep-drawing quality compared to the 300 series.
    
- **400 Series:** Various other chemical compositions exist within this series.
    

### Production Statistics (Representative Values)

- **Global Steel Production:** ~1.5 Billion Tons
    
- **Global Stainless Steel Production:** ~50 MTPA (Million Tons Per Annum)
    
- **Indian Stainless Steel Production:** ~3-4 MTPA (Expected to reach ~10 MTPA by 2030)
    

---

## 2. Raw Materials and Process Economics

### Board Work: Process Economics

Plaintext

```
HC FeCr (High Carbon Ferrochrome)   : ~ 1000 US $/ton
LC FeCr (Low Carbon Ferrochrome)    : ~ 3000 US $/ton
Steel (Carbon Steel)                : ~ 750 - 800 US $/ton
```

_Important Remarks / Instructor Notes:_ Low Carbon Ferrochrome is roughly three times more expensive than High Carbon Ferrochrome. To ensure the process of making stainless steel (or ball bearing steel) remains economically viable, efforts are heavily directed toward substituting LC FeCr with HC FeCr.

### Raw Material Charge

To produce 300-series (Cr-Ni) stainless steel, the charge typically consists of:

1. **Stainless Steel Scrap:** Primary source, but recovery of Cr is < 100% due to oxidation losses.
    
2. **High Carbon FeCr:** Added to replenish Chromium. Contains 6-7% Carbon.
    
3. **Plain Carbon Scrap:** Increases overall melt volume.
    
4. **Primary Nickel:** Added to make up for the Nickel deficit (since plain carbon scrap and FeCr contain no Nickel, diluting the overall Ni percentage).
    

_Physical Interpretation of Alloying Elements:_ Nickel is a **non-oxidizable element**, meaning 100% conservation of Ni from scrap to melt is achieved. Chromium, however, is a **partially oxidizable element** and partitions between the metal and the slag.

---

## 3. Stainless Steel Processing Routes

### Carbon Content Requirements

Chromium is a strong carbide former. High carbon content leads to chromium carbide precipitation at grain boundaries during solidification. Hence, carbon must be kept very low:

- **Low Carbon (C):** $< 0.08\%$
    
- **Ultra-Low Carbon (ULC):** $< 0.02\%$
    

Because of the high carbon influx from the HC FeCr (6-7% C), specialized decarburization steps are required.

### Processing Sequences (Board Work)

- **Duplexing** $\rightarrow$ `EAF -> AOD` (Used for standard $< 0.08\%$ C grades)
    
- **Triplexing** $\rightarrow$ `EAF -> AOD -> VOD` (Used for ULC $< 0.02\%$ C grades)
    
- **EAF (Electric Arc Furnace):** Used purely as a meltdown unit (no oxygen lancing or refining).
    
- **AOD (Argon Oxygen Decarburization):** Gas blowing for primary decarburization.
    
- **VOD (Vacuum Oxygen Decarburization):** Vacuum treatment to achieve ultra-low carbon levels.
    

---

## 4. Thermodynamics of AOD (Argon Oxygen Decarburization)

### Melt Down Composition (Pre-AOD)

- $Cr < 18\%$
    
- $Ni < 8\%$
    
- $C \gg 0.08\%$
    

### The Thermodynamic Challenge

When oxygen is blown into a melt containing both Carbon and Chromium, oxygen must preferentially oxidize Carbon over Chromium.

**Board Work: Ellingham Diagram ($\Delta G^\circ$ vs $T$)**

Plaintext

```
  ΔG° |
      |          Cr - Cr2O3 line
      |       . . . . . . . . . . . .
      |      .                     .
      |     .                       .
      |    .                         .
      |   .                           . 
      |  .     <-- Intersection at ~1800°C -->
      | .                               .  C - CO line
      |---------------------------------------
                                       T
```

_Physical Interpretation:_

Above $1800^\circ C$, the free energy of formation of CO is lower (more stable) than that of Chromium Oxide. At standard steelmaking temperatures ($1600^\circ C$), oxygen will preferentially attack Chromium.

### Board Work: The Primary Reaction

$$(Cr_3O_4) + [C] \rightleftharpoons \{CO\} + [Cr]$$

_(Note: $(...)$ denotes slag phase, $[...]$ denotes metal phase, $\{...\}$ denotes gas phase)._

### Driving the Reaction Forward (Protecting Chromium)

To drive the reaction from left to right (reducing Chromium Oxide back to Chromium by oxidizing Carbon), three conditions must be met:

1. **The Dilution Effect (Argon Injection):** Injecting Argon alongside Oxygen dilutes the gas bubbles. This lowers the partial pressure of CO ($p_{CO}$) inside the bubbles at the melt-gas interface. According to Le Chatelier's principle, lowering $p_{CO}$ drives the reaction to the right, allowing decarburization without oxidizing Cr.
    
2. **High Temperature:** Temperatures must be raised close to $1800^\circ C$ to thermodynamically favor CO formation over Chromium Oxide.
    
3. **High Basic Slag:** A highly basic slag (rich in CaO) eats up acidic compounds (like $SiO_2$). Since $Cr_3O_4$ is also basic, it becomes unstable in a highly basic slag (its activity coefficient increases). Feeling "uncomfortable" in the slag, Chromium is forced back into the metal phase.
    

---

## 5. Slag Management & Winning Back Chromium

### Conversion to Reducing Slag

Even with optimal AOD conditions, chemical efficiency is not 100%, and the basic slag will still trap some $Cr_2O_3$ or $Cr_3O_4$ (giving the slag a greenish color). Before tapping, the oxidizing slag must be converted into a reducing slag to win back this residual Chromium.

- **Mechanism:** The oxygen blow is stopped. Pure Silicon (or Aluminum) is added.
    
- **Reaction:** Silicon dissolves into the metal (not the slag) and vigorously reacts at the interface:
    
    $$2(Cr_3O_4) + 3[Si] \rightarrow 6[Cr] + 3(SiO_2)$$
    
- Because the slag is highly basic, it readily absorbs the generated $SiO_2$, keeping silica activity low and driving Chromium recovery forward.
    

---

## 6. Vacuum Oxygen Decarburization (VOD)

_Conceptual Explanation:_

The AOD process struggles to drive carbon below $0.07-0.08\%$ because doing so would require excessively high temperatures and vast amounts of Argon. To reach Ultra-Low Carbon ($<0.02\%$), the melt is transferred to a VOD unit.

- **Mechanism:** The ladle is placed in a vacuum tank ($~10^1$ millibar pressure). Under vacuum, $p_{CO}$ is virtually zero.
    
- **Heating:** Extra heating is usually unnecessary because the melt arrives extremely hot from the AOD's exothermic oxidation cycles.
    
- Limited oxygen is lanced under vacuum, forcing the remaining carbon to react and leave as CO.
    

---

## 7. Tapping Operations (Post-Primary Steelmaking)

### Ladle Specifications

- **Shape:** Cylindrical with a slight taper ($2^\circ$ to $5^\circ$ at the bottom).
    
- **Lining:** Basic refractory (Tar dolomite and magnesite bricks).
    
- **Preheating:** Ladles must be preheated. Otherwise, tapping into a cold ladle causes a massive temperature drop.
    

### Tapping Dynamics

- **Rate:** 7 to 15 tons per minute.
    
- **Fall Height:** The metal falls from 7 to 8 meters.
    
- **Thermal Loss:** A standard temperature drop ($\Delta T$) of $60^\circ C$ to $70^\circ C$ occurs during tapping due to radiation (governed by Stefan-Boltzmann Law: $E \propto T^4$). Tapping temperatures are kept around $1600^\circ C$ to compensate.
    
- **Gas Pick-up:** Significant Nitrogen absorption occurs (~500 ppm gets dissolved from the entrained air). Minimal oxygen transfers from the air because the melt is already highly saturated with dissolved oxygen (~600 ppm) from the primary steelmaking process.
    
 
### Slag Carryover Prevention

_Important Remarks:_ Permitting primary oxidizing slag (which contains 20-25% FeO) into the ladle is highly detrimental. It will consume downstream deoxidizers and create dirty steel full of oxide inclusions.

- **Mitigation:** Slag detection systems (floating darts, electromagnetic sensors, thermal imaging) are used to tilt the converter upward the exact moment slag begins to drain, ensuring carryover slag is kept below 0.1%.
    

### Synthetic Slag & Deoxidation

1. Empty ladles are pre-loaded with specific synthetic slag-forming agents (CaO, Al2O3, etc.).
    
2. The immense kinetic momentum of the falling metal stream perfectly churns and mixes these agents, creating a synthetic slag floating on top, which prevents further radiation heat loss.
    
3. **Deoxidizers:** Added when the ladle is half-full, close to the tapping stream to exploit the maximum velocity and turbulent mixing, ensuring rapid dissolution to strip the 600 ppm of dissolved oxygen down to the required 10-20 ppm final product specification.
   
# Audio V2


# LECTURE NOTES: Stainless Steelmaking and Tapping Operations

## 1. Introduction and Process Economics

Electric Arc Furnaces (EAF) are primarily used as melting and refining units. However, for alloy steels (like ball-bearing or stainless steel), the EAF is mostly used just to **melt the scrap**, and the melt is then transferred to a separate reactor for decarburization and alloying.

**Economic Considerations (Representative Prices):**

- **High Carbon Ferrochrome (HC FeCr):** Much cheaper to use.
    
- **Low Carbon Ferrochrome (LC FeCr):** Approximately **3 times more expensive** than HC FeCr.
    
- **Carbon Steel:** Costs roughly **$750 to $800 USD per ton**.
    
- _Process Strategy:_ To keep the process economical, steelmakers substitute LC FeCr with HC FeCr.
    

## 2. Properties and Applications of Stainless Steel

Stainless steel is prized for its excellent **anti-corrosion** and **anti-rusting** properties.

- **Applications:** Home utensils, medical instruments, railway wagons, and car components.
    
- **Modern Trends:** Kitchen cabinets in North America are increasingly made of stainless steel due to embargoes on chopping wood and to prevent degradation/insect attacks. Stainless steel can also be rolled "paper-thin" for lightweight furniture (e.g., beach chairs with Italian leather).
    

**Global and Indian Production Statistics:**

- **Global Total Steel Production:** ~1.5 billion tons.
    
- **Global Stainless Steel Production:** ~50 million tons.
    
- **Indian Stainless Steel Production:** ~3 to 4 million tons per annum (expected to reach ~10 million tons by the time total production reaches 250-300 million tons in 2030).
    
- **Key Indian Producers Mentioned:** Jindal (plants in Jajpur/overseas), Viraj Profiles (near Bombay), and Mukand Steel.
    

## 3. Classification of Stainless Steels

- **300 Series (Austenitic):** Based on **Chromium and Nickel**.
    
    - _Example:_ 18/8 stainless steel (18% Cr, 8% Ni).
        
    - _High-end:_ Can contain up to 24% Nickel. Excellent deep drawing quality and lifespan.
        
- **200 Series:** Based on **Chromium and Manganese** (Nickel is replaced by Manganese to reduce cost).
    
    - _Drawback:_ Cheaper variety, prone to developing cracks, and the deep drawing quality suffers.
        
- **400 Series:** Another grade briefly mentioned.
    

## 4. Raw Materials and Oxidation Behavior

**Charge Materials for 300 Series:**

1. **Stainless Steel Scrap:** Main ingredient.
    
2. **High Carbon Ferrochrome (HC FeCr):** Used as a Cr source but brings in massive amounts of carbon (6-7% C).
    
3. **Plain Carbon Scrap:** Used to increase melt volume.
    
4. **Primary Nickel (Pure Nickel Shots):** Required because plain carbon scrap and FeCr contain no Nickel, diluting the overall Ni percentage.
    

**Oxidation Behavior of Elements:**

- **Nickel:** Classified as a **non-oxidizable element**. 100% of the Nickel in the scrap is conserved and recovered in the melt.
    
- **Chromium:** Classified as a **partially oxidizable element**. Recovery is less than 100% because it partitions between the metal and the slag (forms Chromium Oxide).
    

## 5. The Need for Decarburization

Chromium is a **strong carbide-forming element**. If carbon is high, chromium carbide precipitates at the grain boundaries during solidification. Therefore, carbon must be kept extremely low.

- **Standard Low Carbon SS:** $< 0.08\% \text{ C}$ (Produced via **Duplexing**: EAF $\rightarrow$ AOD)
    
- **Ultra-Low Carbon (ULC) SS:** $< 0.02\% \text{ C}$ (Produced via **Triplexing**: EAF $\rightarrow$ AOD $\rightarrow$ VOD)
    

_Note: At meltdown in the EAF, the composition is typically: Cr < 18%, Ni < 8%, and C is significantly higher than 0.08%._

---

## 6. AOD (Argon Oxygen Decarburization) Process

After melting in the EAF, the melt is transferred to the AOD converter. The goal is to preferentially oxidize Carbon without oxidizing Chromium.

### Thermodynamic Challenges (Ellingham Diagram Context)

- Above **1800°C**, Carbon Monoxide (CO) is more stable than Chromium Oxide.
    
- At standard steelmaking temperatures (**1600°C**), Chromium Oxide is more stable, meaning oxygen will preferentially attack Chromium instead of Carbon.
    
- **The Target Reaction (Forward Direction):** $Cr_3O_4 + [C] \rightarrow CO + [Cr]$
    

### Three Conditions Required to Protect Chromium in AOD:

1. **Dilution Effect (Argon Injection):** Argon is blown with Oxygen. The argon dilutes the gas bubbles, drastically lowering the partial pressure of CO ($P_{CO}$) inside the bubble. Lower $P_{CO}$ thermodynamically drives the reaction forward to remove carbon without oxidizing Cr.
    
2. **High Temperature:** Pushing temperatures closer to 1800°C favors CO formation.
    
3. **High Basic Slag:** A highly basic slag (rich in CaO) eats up silica. Since Chromium Oxide ($Cr_3O_4$) is also basic, its **activity coefficient increases** in a basic slag. Because it is unstable/uncomfortable in the slag phase, it is driven back into the metal melt.
    

### AOD Operational Details

- **Gas Injection:** Side-blown tuyeres (Argon, Nitrogen, Oxygen) provide stirring. Top lances lack supersonic jets and transfer momentum poorly, so the system is not perfectly stirred compared to a BOF or Q-BOP.
    
- **Processing Time:** Decarburization rates are slower due to lower interfacial area. Tap-to-tap time is long (e.g., 70–90 minutes for a 30–50 ton batch).
    
- **Slag Color:** The presence of Chromium Oxide gives the AOD slag a distinctive **greenish appearance** (unlike blackish BOF slag).
    

## 7. Converting Oxidizing Slag to Reducing Slag

Before tapping, you must win back the 3–5% of Chromium trapped in the slag as $Cr_2O_3$ or $Cr_3O_4$.

- **Method:** Stop the oxygen blow (the slag is currently oxidizing). Add **pure Silicon** (or Aluminum).
    
- **Reaction:** Silicon dissolves in the metal (not the slag) and reacts: $2Cr_3O_4 + 3Si \rightarrow 6Cr + 3SiO_2$.
    
- **Result:** The exothermic reaction strips oxygen from the chromium, sending Cr back to the metal. The basic slag safely absorbs the newly formed silica.
    

---

## 8. VOD (Vacuum Oxygen Decarburization) Process

Used to reach **Ultra-Low Carbon (<0.02%)** limits that AOD cannot efficiently achieve.

- **Method:** The melt is tapped into a ladle and placed in a tank degassing arrangement under vacuum (Pressure: ~1 millibar or $10^{-1}$ mbar).
    
- **Mechanism:** Under a vacuum, the CO partial pressure is virtually zero, strongly driving the remaining Carbon and Oxygen to react and leave the melt.
    
- **Temperature:** No additional heating is needed. The melt arrives extremely hot from AOD, leaving a good margin before the casting temperature of **1560°C to 1570°C**.
    

---

## 9. Tapping Operations

Tapping is the process of transferring steel from the primary vessel (BOF/EAF/AOD) to a ladle for secondary metallurgy.

### Ladle Specifications

- **Shape:** Cylindrical with a slight **2° to 5° taper** at the bottom.
    
- **Refractory Lining:** Basic refractories (Tar dolomite and magnesite bricks).
    
- **Preparation:** Must be **preheated** to prevent massive temperature drops.
    

### Tapping Dynamics & Parameters

- **Tapping Rate:** 7, 10, or up to **15 tons per minute**.
    
- **Drop Height:** The metal falls from a height of **7 to 8 meters**.
    
- **Temperature Drop ($\Delta T$):** Typically **60°C to 70°C** drops during tapping due to radiation heat loss.
    
- _Note:_ Heat radiation is proportional to the 4th power of absolute temperature (Stefan-Boltzmann Law: $T^4$). To compensate, tapping temperature from the furnace is kept around **1600°C** ($\pm 10°C$).
    

### Gas Pick-up During Tapping

- **Nitrogen:** Great solubility in steel (approx. **470 to 500 ppm** at 1600°C). Significant nitrogen is absorbed from entrained air during tapping.
    
- **Hydrogen:** Solubility is about **28 ppm**.
    
- **Oxygen:** Pure oxygen solubility is ~2000 ppm. However, minimal oxygen is picked up from the atmosphere because the primary melt already contains **300 to 600 ppm** of dissolved oxygen. The final product target is only **10 to 20 ppm** oxygen to prevent blowholes/porosity.
    

### Synthetic Slag and Deoxidation

- **Synthetic Slag:** Before tapping, the empty ladle is pre-filled with specific amounts of basicity agents (Silica, $Al_2O_3$). The massive kinetic energy of the falling stream rapidly churns, melts, and floats this into a synthetic slag layer, protecting against further heat loss.
    
- **Adding Deoxidizers:** Deoxidizers (elements with high affinity for oxygen) are added when the ladle is **half full**, right near the tapping stream to exploit the maximum velocity and stirring intensity.
    

### Preventing Carryover Slag

- **The Problem:** Primary oxidizing slag contains **20% to 25% FeO**. If this enters the ladle, it will "eat up" the deoxidizers (ruining process economics) and make the steel extremely dirty with oxide inclusions.
    
- **The Solution:** Use slag detection systems (floating darts, electromagnetic, or thermal imaging). Once the slag level approaches the tap hole, the converter is instantly raised. The goal is to keep carryover slag to **< 0.1%**.
    
- **Next Step:** Ladle is put on a railway track and moved to the **Ladle Refining Furnace (LRF)** or treatment station.