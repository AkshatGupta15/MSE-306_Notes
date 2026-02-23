# **Lecture 8: Blast Furnace Productivity & Modern Practices**

## **1. Productivity: Definition and Optimization**

The productivity of a Blast Furnace (BF) is defined as the **Rate of Production ($R$)**, typically measured in **Tonnes of Hot Metal (THM) per day**.

### **The Governing Formula**

To understand how to maximize production, we express $R$ as:

$$R \ (\text{thm/day}) = \frac{\text{Total Volume of Gas Blown in a Day} \ (m^3/\text{day})}{\text{Specific Blast Rate} \ (m^3/\text{thm})}$$

- **Numerator**: The total wind/air pumped into the furnace per day.
    
- **Denominator**: The amount of air required to produce **one tonne** of hot metal.
    

### **Optimization Strategy**

To increase Productivity ($R$), we have two options:

1. **Increase the Numerator**: Blow more air.
    
2. **Decrease the Denominator**: Make the process more efficient so less air is needed per tonne of iron.
    

---

## **2. Constraints on Gas Flow (The Numerator Limit)**

We cannot simply blow infinite air into the furnace. Increasing the gas velocity beyond a critical limit triggers dangerous aerodynamic phenomena.

### **Aerodynamic Limits (Step-by-Step Failure)**

1. **Fluidization**: High gas velocity causes smaller particles to become suspended/dance in the gas stream.
    
2. **Elutriation**: Extremely high velocity carries fine particles out of the furnace top (dust loss).
    
3. **Loading**:
    
    - Occurs in the **Cohesive Zone** (where solids and liquids coexist).
        
    - The upward gas drag balances the downward gravity of the liquid (slag/metal).
        
    - _Result_: Liquid stops descending and accumulates.
        
4. **Flooding**:
    
    - Gas drag exceeds gravity. Liquid is pushed _upward_.
        
    - Liquid enters cooler upper regions, solidifies, and blocks the pores.
        
5. **Hanging**:
    
    - The final catastrophic state.
        
    - The burden ceases to descend ("hangs" in the shaft).
        
    - Production stops completely.
        

> **Instructor Note**: Because of these limits, most furnaces operate at a **maximum critical gas velocity** (within ~5-10%). Therefore, the only _real_ way to increase productivity is to **reduce the Specific Blast Rate (Denominator)**.

---

## **3. Factors Affecting Specific Blast Rate**

The Specific Blast Rate depends heavily on raw material quality and thermal efficiency.

### **Case Study: High Grade vs. Low Grade Ore**

Consider two scenarios:

- **Case A**: Ore with 80% $Fe_2O_3$ (20% Gangue).
    
- **Case B**: Ore with 70% $Fe_2O_3$ (30% Gangue).
    

**Why Case A has higher productivity:**

1. **Less Slag**: Case B has 50% more gangue per tonne of Fe $\rightarrow$ Higher slag volume.
    
2. **Less Heat Load**: Slag must be melted to 1450°C. More slag = More heat required.
    
3. **Less Coke**: More heat needed in Case B means burning more Coke.
    
4. **Less Blast**: Burning more Coke requires more Air (Blast).
    
5. **Result**: Case B has a higher Specific Blast Rate $\rightarrow$ Lower Productivity.
    

---

## **4. Modern Blast Furnace Practices (The 8 Pillars)**

Modern ironmaking has evolved 8 distinct practices aimed specifically at **reducing Coke Rate** and **Specific Blast Rate**.

### **1. Giant Blast Furnaces**

- **Concept**: Move from 1000 $m^3$ to 4000–5000 $m^3$ furnaces.
    
- **Physics**: Heat loss is proportional to Surface Area ($A$), while heat generation is proportional to Volume ($V$).
    
- **Benefit**: Larger furnaces have a smaller $A/V$ ratio $\rightarrow$ Less relative heat loss through walls $\rightarrow$ Lower Coke Rate.
    

### **2. High Blast Temperature**

- **Practice**: Preheating air to **~1200 K** (limit imposed by Stove refractories).
    
- **Benefit**: Sensible heat enters with the air, reducing the need to burn Coke for heat.
    
- **Equipment**: Modern Stoves or Metallic Blast Heaters.
    

### **3. High Top Pressure**

- **Practice**: Operating the furnace top at 1.5–2.5 atm (vs. near atmospheric).
    
- **Benefit**:
    
    - Reduces gas velocity (Volume $\propto$ 1/P).
        
    - Increases residence time $\rightarrow$ Better Gas-Solid heat transfer $\rightarrow$ Lower top gas temperature (Waste Heat reduction).
        
    - Suppresses the **Boudouard Reaction** ($C + CO_2 \to 2CO$), which is solution loss (carbon waste).
        

### **4. Oxygen Enrichment**

- **Practice**: Increasing $O_2$ in blast from 21% to ~24%.
    
- **Benefit**:
    
    - Reduces Nitrogen volume (which is an inert heat sink).
        
    - Increases flame temperature and combustion efficiency.
        
    - _Note_: We cannot use 100% pure oxygen yet as it would overheat the raceway uncontrollably.
        

### **5. Coal Dust Injection (PCI - Pulverized Coal Injection)**

- **Practice**: Injecting non-coking coal dust (cheap) directly into tuyeres.
    
- **Typical Rate**: 150–200 kg/thm (Record ~260 kg).
    
- **Benefit**: Replaces expensive Metallurgical Coke.
    
- **Challenge**: Coal ash adds to slag volume; incomplete combustion can generate soot.
    

### **6. Humidification of Blast**

- **Practice**: Injecting Steam ($H_2O$) into the blast.
    
- **Reaction**: $C + H_2O \to CO + H_2$ (Endothermic).
    
- **Role**:
    
    - Generates **Hydrogen**: $H_2$ is a smaller molecule than $CO$, diffuses faster, and reduces ore more efficiently.
        
    - **Control Tool**: Used to fine-tune the **RAFT** (Raceway Adiabatic Flame Temperature). If the raceway gets too hot (due to $O_2$ enrichment), steam cools it down.
        

### **7. Lime Dust Injection**

- **Practice**: Injecting flux powder through tuyeres.
    
- **Benefit**:
    
    - Lime reacts immediately with Ash/Sulfur in the raceway.
        
    - Removes the thermal burden of calcining limestone inside the stack.
        

### **8. Engineered Raw Materials (Burden Preparation)**

- **Practice**: 80-90% Sinter/Pellet burden (vs. Lump Ore).
    
- **Benefit**:
    
    - **Channeling Prevention**: Uniform size prevents gas from finding "easy paths" (Channeling).
        
    - **Reducibility**: Sinter/Pellets have engineered porosity, allowing gas to penetrate and reduce iron oxides faster.
        

---

## **5. Summary: The Interconnected Goal**

All 8 practices aim to lower the **Coke Rate** ($kg_{coke}/thm$).

- **Relationship**:
    
    $$\downarrow \text{Coke Rate} \implies \downarrow \text{Blast Rate} \implies \uparrow \text{Productivity}$$
    
- **Evolution**:
    
    - **1970s**: Coke Rate ~800 kg/thm.
        
    - **Today**: Coke Rate ~350–400 kg/thm.
        
    - **Productivity**: Increased from ~1.5 to **2.5–3.5 thm/day/m³**.
        
