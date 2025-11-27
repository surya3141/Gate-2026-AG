# 🔢 Plant Protection Equipment PYQ Solutions

> Previous Year Questions with detailed solutions for GATE Agricultural Engineering

---

## 📊 Solutions Summary

| Year | Questions | Difficulty Distribution | Topics Covered |
|------|-----------|-------------------------|----------------|
| 2024 | 3 | Easy: 1, Medium: 1, Hard: 1 | Nozzles, Calibration, Droplet |
| 2023 | 2 | Easy: 1, Medium: 1 | Pumps, Application Rate |
| 2022 | 3 | Medium: 3 | Drift, Boom Height, Discharge |
| 2021 | 2 | Easy: 1, Medium: 1 | Components, Concentration |
| 2020 | 2 | Easy: 1, Medium: 1 | Nozzle Selection, Safety |
| **Total** | **12** | **Easy: 4, Medium: 7, Hard: 1** | **All Major Topics** |

---

## 2024 Questions

### Question 1 (Easy) - Nozzle Type #NozzleType #2024
**Which type of nozzle is most suitable for applying herbicides in a boom sprayer?**

**Options:**
(a) Hollow cone nozzle  
(b) Solid cone nozzle  
(c) Flat fan nozzle  
(d) Mist nozzle

**Solution:**

**Nozzle Characteristics:**

**Hollow Cone:**
- Fine droplets (50-200 microns)
- Good penetration
- For: Insecticides, Fungicides
- High drift risk

**Solid Cone:**
- Medium droplets (100-300 microns)
- Full coverage
- For: Soil application, Fertilizers

**Flat Fan:**
- Coarse droplets (200-400 microns)
- Uniform width distribution
- **For: Herbicides** ✓
- Low drift
- Ideal for boom sprayers

**Mist:**
- Very fine (10-50 microns)
- Extreme drift
- For: ULV, Greenhouses

**Why Flat Fan for Herbicides?**

1. **Coarse droplets** → Less drift (herbicides harmful to nearby crops)
2. **Uniform pattern** → Even coverage across swath
3. **Tapered edges** → Proper overlap on boom
4. **Soil/foliage contact** → Herbicides need good coverage, not penetration

**Answer:** (c) Flat fan nozzle

**Time:** 1 minute | **Marks:** 1

---

### Question 2 (Medium) - Sprayer Calibration #Calibration #2024
**A knapsack sprayer is tested on a 100 m² area. The sprayer initially contained 15 liters of water. After spraying the test area, 9 liters remained. Calculate the application rate in L/ha.**

**Solution:**

Given:
- Test area = 100 m²
- Initial volume = 15 L
- Final volume = 9 L

**Step 1:** Calculate volume used
$$
\text{Volume used} = 15 - 9 = 6 \text{ L}
$$

**Step 2:** Calculate rate per m²
$$
\text{Rate per m}^2 = \frac{6}{100} = 0.06 \text{ L/m}^2
$$

**Step 3:** Convert to per hectare
$$
\text{Application rate (L/ha)} = \frac{\text{Volume used}}{\text{Area (m}^2\text{)}} \times 10000
$$

$$
\text{Rate} = \frac{6}{100} \times 10000 = 60 \times 100 = 600 \text{ L/ha}
$$

**Interpretation:**
- 600 L/ha is MEDIUM VOLUME spraying
- Typical range for most pesticides
- Appropriate for manual sprayers

**Verification:**
If 1 hectare = 10,000 m², and we use 0.06 L/m²:
$$
10000 \times 0.06 = 600 \text{ L/ha} \quad \checkmark
$$

**Answer:** 600 L/ha

**Time:** 2 minutes | **Marks:** 2

---

### Question 3 (Hard) - Droplet Dynamics #Droplet #2024
**A spray droplet of 100 micron diameter is released from 2 m height. Given: droplet density = 1000 kg/m³, air density = 1.2 kg/m³, air viscosity = 1.8 × 10⁻⁵ Pa·s, g = 10 m/s².**

**(a) Calculate the terminal velocity of the droplet**  
**(b) Calculate the time to reach ground if falling at terminal velocity**  
**(c) Comment on drift potential**

**Solution:**

Given:
- Droplet diameter (d) = 100 microns = 100 × 10⁻⁶ m = 10⁻⁴ m
- Height (h) = 2 m
- Droplet density (ρ_p) = 1000 kg/m³
- Air density (ρ_a) = 1.2 kg/m³
- Air viscosity (μ) = 1.8 × 10⁻⁵ Pa·s
- g = 10 m/s²

**Part (a): Terminal Velocity**

**Using Stokes' Law:**
$$
V_t = \frac{d^2 (\rho_p - \rho_a) g}{18 \mu}
$$

**Substitute values:**
$$
V_t = \frac{(10^{-4})^2 \times (1000 - 1.2) \times 10}{18 \times 1.8 \times 10^{-5}}
$$

$$
V_t = \frac{10^{-8} \times 998.8 \times 10}{18 \times 1.8 \times 10^{-5}}
$$

$$
V_t = \frac{10^{-8} \times 9988}{32.4 \times 10^{-5}}
$$

$$
V_t = \frac{9.988 \times 10^{-5}}{32.4 \times 10^{-5}} = \frac{9.988}{32.4} = 0.308 \text{ m/s}
$$

**Part (b): Time to Reach Ground**

$$
\text{Time} = \frac{\text{Height}}{\text{Terminal velocity}} = \frac{2}{0.308} = 6.49 \text{ seconds}
$$

**Part (c): Drift Potential**

**Analysis:**

**Terminal velocity = 0.308 m/s = 0.3 m/s**

Compare with wind:
- If wind speed = 10 km/h = 2.78 m/s
- Wind speed is ~9 times terminal velocity
- Droplet will move horizontally: 2.78 m/s × 6.49 s = **18 m horizontal drift!**

**Drift Classification:**

| Droplet Size | Terminal Velocity | Drift Potential |
|--------------|-------------------|-----------------|
| 50 microns | 0.08 m/s | Very High |
| **100 microns** | **0.3 m/s** | **Medium-High** |
| 200 microns | 1.2 m/s | Low |
| 400 microns | 4.8 m/s | Very Low |

**Conclusion:**
- 100-micron droplets have MEDIUM drift risk
- Suitable for insecticides (need penetration)
- NOT suitable for herbicides (use 200-400 microns)
- Avoid spraying in wind >10 km/h

**Answers:**
- (a) Terminal velocity = 0.31 m/s (or 0.3 m/s)
- (b) Time = 6.5 seconds
- (c) Medium drift potential; horizontal drift ~18 m in 10 km/h wind

**Time:** 8 minutes | **Marks:** 2

---

## 2023 Questions

### Question 4 (Easy) - Pump Type #PumpType #2023
**Which pump is most suitable for high-pressure spraying in a motorized power sprayer?**

**Options:**
(a) Centrifugal pump  
(b) Piston pump  
(c) Gear pump  
(d) Submersible pump

**Solution:**

**Pump Comparison:**

| Pump Type | Pressure Range | Self-priming | Flow | Application |
|-----------|----------------|--------------|------|-------------|
| **Centrifugal** | 2-8 bar | No | High | Boom sprayers |
| **Piston** | **10-30 bar** | **Yes** | **Medium** | **Power sprayers** ✓ |
| **Diaphragm** | 5-15 bar | Yes | Low-Medium | Knapsack |
| **Gear** | 5-10 bar | Yes | Medium | Low pressure |

**Why Piston Pump for Power Sprayers?**

**Requirements for Power Sprayers:**
- HIGH pressure (15-30 bar) for atomization ✓
- Self-priming capability ✓
- Can handle chemicals ✓
- Reliable operation ✓

**Piston Pump Advantages:**
1. **Highest pressure** among options (up to 30 bar)
2. Self-priming (can suck from tank)
3. Positive displacement (consistent flow)
4. Durable construction

**Why NOT Others:**

**Centrifugal:**
- Low pressure (2-8 bar) - insufficient
- Not self-priming
- Better for boom sprayers (high volume, low pressure)

**Gear:**
- Medium pressure only
- Less common in sprayers

**Submersible:**
- For water wells, not sprayers

**Answer:** (b) Piston pump

**Time:** 2 minutes | **Marks:** 1

---

### Question 5 (Medium) - Application Rate #ApplicationRate #2023
**A boom sprayer with 8 m width travels at 8 km/h. The total flow rate from all nozzles is 32 L/min. Calculate the application rate in L/ha.**

**Solution:**

Given:
- Boom width (W) = 8 m
- Travel speed (S) = 8 km/h
- Total flow rate (Q) = 32 L/min

**Formula for application rate:**
$$
\text{Application rate (L/ha)} = \frac{Q \times 600}{W \times S}
$$

**Why 600?**
- Converting units: L/min to L/ha
- 1 hour = 60 minutes
- 1 hectare = 10,000 m²
- Factor: (60 × 10000) / 1000 = 600

**Calculate:**
$$
\text{Rate} = \frac{32 \times 600}{8 \times 8} = \frac{19200}{64} = 300 \text{ L/ha}
$$

**Verification using basic approach:**

**Area covered per minute:**
$$
\text{Area/min} = \frac{W \times S \times 1000}{60} = \frac{8 \times 8 \times 1000}{60} = \frac{64000}{60} = 1066.67 \text{ m}^2\text{/min}
$$

**Application rate:**
$$
\text{Rate} = \frac{32 \text{ L}}{1066.67 \text{ m}^2} = 0.03 \text{ L/m}^2 = 300 \text{ L/ha} \quad \checkmark
$$

**Interpretation:**
- 300 L/ha is MEDIUM VOLUME
- Appropriate for herbicide application
- Typical boom sprayer range: 200-500 L/ha

**Answer:** 300 L/ha

**Time:** 3 minutes | **Marks:** 2

---

## 2022 Questions

### Question 6 (Medium) - Drift Control #Drift #2022
**Arrange the following measures in order of effectiveness for reducing spray drift (most effective first):**

I. Reducing boom height  
II. Using larger droplets  
III. Adding drift-control agent  
IV. Reducing wind speed

**Options:**
(a) II → I → III → IV  
(b) IV → II → I → III  
(c) II → IV → I → III  
(d) I → II → III → IV

**Solution:**

**Analyzing Each Factor:**

**Factor I: Reducing Boom Height**
- Effect: MODERATE
- Lower height = less time for drift
- Droplets reach target faster
- Limitation: Still limited by droplet size
- Practical: Can control (40-60 cm typical)

**Factor II: Using Larger Droplets**
- Effect: VERY HIGH (MOST IMPORTANT)
- Terminal velocity ∝ d² (droplet diameter squared)
- 200-micron droplet falls 4× faster than 100-micron
- Directly addresses root cause
- Practical: Easy (change nozzle/pressure)

**Factor III: Adding Drift-Control Agent**
- Effect: MODERATE
- Increases droplet size slightly
- Reduces fine droplets
- Practical: Requires additional cost

**Factor IV: Reducing Wind Speed**
- Effect: VERY HIGH (when possible)
- Wind is primary drift cause
- Limitation: CANNOT CONTROL WEATHER
- Practical: Can only choose timing (spray in calm conditions)

**Ranking by Controllability and Effectiveness:**

**Most Effective that WE CAN CONTROL:**
1. **Using larger droplets (II)** - Direct solution, easy to implement
2. **Reducing boom height (I)** - Secondary benefit, always controllable
3. **Adding drift agent (III)** - Helps but costs more
4. **Reducing wind speed (IV)** - Uncontrollable (we can only avoid windy times)

**BUT if ranked by PURE EFFECTIVENESS:**
1. Wind speed (if we could control)
2. Droplet size
3. Boom height
4. Additives

**Question asks: "Effectiveness for REDUCING drift"**

The practical interpretation: What measures can operator take?

**II (Droplet) → I (Height) → III (Agent) → IV (Wind - not controllable)**

**Answer:** (a) II → I → III → IV

**Alternative interpretation:** If "reducing wind speed" means "choosing calm conditions", then:
**IV → II → I → III** would also be valid

**Most likely answer:** **(a) II → I → III → IV** (based on controllable measures)

**Time:** 4 minutes | **Marks:** 2

---

### Question 7 (Medium) - Boom Height #BoomHeight #2022
**A boom sprayer uses flat fan nozzles with 110° spray angle. Nozzles are spaced 50 cm apart on the boom. Calculate the recommended boom height above the target for 100% overlap.**

**Solution:**

Given:
- Spray angle (θ) = 110°
- Nozzle spacing (W) = 50 cm

**Formula for boom height:**
$$
h = \frac{W}{2 \times \tan(\theta/2)}
$$

**Step 1:** Calculate θ/2
$$
\frac{\theta}{2} = \frac{110°}{2} = 55°
$$

**Step 2:** Find tan(55°)
$$
\tan(55°) = 1.428
$$

**Step 3:** Calculate height
$$
h = \frac{50}{2 \times 1.428} = \frac{50}{2.856} = 17.5 \text{ cm}
$$

**Geometric Interpretation:**

At height h, spray cone from nozzle covers width:
$$
\text{Swath width} = 2h \times \tan(55°) = 2 \times 17.5 \times 1.428 = 50 \text{ cm}
$$

For 100% overlap, adjacent nozzle patterns must meet at target height.

**Practical Considerations:**

**Theoretical height:** 17.5 cm

**Actual recommended height:** 40-60 cm

**Why difference?**
- Spray pattern not perfect cone
- Need some overlap for uniformity
- Crop canopy height
- Boom movement/bounce

**Standard practice:** Height = 30-40% of nozzle spacing above canopy
$$
h = 0.3 \times 50 = 15 \text{ cm minimum above canopy}
$$

If canopy is 30 cm, boom height = 30 + 15 = 45 cm above ground

**Answer:** 17.5 cm (theoretical) or 40-50 cm (practical above canopy)

**Time:** 4 minutes | **Marks:** 2

---

### Question 8 (Medium) - Nozzle Discharge #Discharge #2022
**A nozzle has a discharge constant K = 1.2. What will be the discharge at 9 bar pressure?**

**Solution:**

Given:
- Nozzle constant (K) = 1.2
- Pressure (P) = 9 bar

**Formula for nozzle discharge:**
$$
Q = K\sqrt{P}
$$

Where:
- Q = Discharge (L/min)
- K = Nozzle constant (L/min/√bar)
- P = Pressure (bar)

**Calculate:**
$$
Q = 1.2 \times \sqrt{9} = 1.2 \times 3 = 3.6 \text{ L/min}
$$

**Understanding K constant:**

The nozzle constant depends on orifice size:
- Larger orifice → larger K
- At 1 bar: Q = K × 1 = K
- At 4 bar: Q = K × 2 = 2K
- At 9 bar: Q = K × 3 = 3K

**Verification with physics:**

$$
Q = C_d \times A \times \sqrt{2gH}
$$

Where H ∝ P, so Q ∝ √P

**If pressure changes:**

From P₁ to P₂:
$$
\frac{Q_2}{Q_1} = \sqrt{\frac{P_2}{P_1}}
$$

**Example:** If Q = 1.8 L/min at 4 bar, what is Q at 9 bar?
$$
Q_9 = 1.8 \times \sqrt{\frac{9}{4}} = 1.8 \times 1.5 = 2.7 \text{ L/min}
$$

But using K:
$$
K = \frac{Q_4}{\sqrt{4}} = \frac{1.8}{2} = 0.9
$$
$$
Q_9 = 0.9 \times \sqrt{9} = 0.9 \times 3 = 2.7 \text{ L/min} \quad \checkmark
$$

**Answer:** 3.6 L/min

**Time:** 2 minutes | **Marks:** 2

---

## 2021 Questions

### Question 9 (Easy) - Sprayer Component #Component #2021
**What is the primary function of the pressure chamber in a knapsack sprayer?**

**Options:**
(a) To store the spray liquid  
(b) To filter impurities  
(c) To maintain constant pressure and smooth spray  
(d) To atomize the liquid

**Solution:**

**Knapsack Sprayer Components:**

**Tank:**
- Stores spray liquid ❌ (not pressure chamber)
- Main reservoir

**Strainer/Filter:**
- Removes impurities ❌
- Prevents nozzle clogging

**Pump:**
- Creates pressure
- Lever-operated

**Pressure Chamber:**
- Air-filled vessel
- Connected to pump and tank
- **Function: Maintains constant pressure** ✓

**Nozzle:**
- Atomizes liquid ❌
- Creates spray pattern

**How Pressure Chamber Works:**

**Without Pressure Chamber:**
- Pump creates pressure only when lever pressed
- Pressure fluctuates with each stroke
- Spray is pulsating
- Uneven application

**With Pressure Chamber:**
1. Pump compresses air into chamber
2. Chamber stores compressed air
3. Air pushes on liquid continuously
4. **Constant, smooth pressure to nozzle**
5. Uniform spray even between pump strokes

**Analogy:** Like a capacitor in electronics - smooths fluctuations

**Benefits:**
- ✓ Smooth, continuous spray
- ✓ Uniform droplet size
- ✓ Consistent application
- ✓ Less pumping frequency

**Answer:** (c) To maintain constant pressure and smooth spray

**Time:** 2 minutes | **Marks:** 1

---

### Question 10 (Medium) - Concentration Calculation #Concentration #2021
**A farmer needs to prepare 2% insecticide solution for spraying. The spray volume required for 1 hectare is 500 liters. Calculate:**
**(a) Amount of insecticide concentrate needed**
**(b) Amount of water needed**

**Solution:**

Given:
- Required concentration = 2%
- Total spray volume = 500 L

**Understanding 2% solution:**
- 2% means 2 liters (or kg) of concentrate in 100 liters of final solution
- Or: 2 parts concentrate + 98 parts water = 100 parts solution

**Part (a): Amount of Insecticide**

**Formula:**
$$
\text{Amount of chemical} = \frac{\text{Required \%} \times \text{Total volume}}{100}
$$

$$
\text{Insecticide} = \frac{2 \times 500}{100} = \frac{1000}{100} = 10 \text{ L}
$$

**Part (b): Amount of Water**

$$
\text{Water} = \text{Total volume} - \text{Insecticide}
$$

$$
\text{Water} = 500 - 10 = 490 \text{ L}
$$

**Verification:**
$$
\text{Concentration} = \frac{10}{500} \times 100 = 2\% \quad \checkmark
$$

**Mixing Procedure:**

1. Fill tank with 250 L water (half)
2. Add 10 L insecticide concentrate
3. Agitate thoroughly
4. Add remaining 240 L water
5. Agitate again
6. Total = 500 L of 2% solution

**Alternative scenario:**

If label says: "Use 2 L/ha of concentrate in 500 L water"
- Then: Concentration = 2/500 = 0.4% (different from above)
- Always read label carefully!

**Answers:**
- (a) Insecticide concentrate = 10 L
- (b) Water = 490 L

**Time:** 3 minutes | **Marks:** 2

---

## 2020 Questions

### Question 11 (Easy) - Nozzle Selection #Selection #2020
**For spraying insecticides in a dense crop canopy requiring good penetration, which nozzle is most appropriate?**

**Options:**
(a) Flat fan nozzle  
(b) Hollow cone nozzle  
(c) Deflector nozzle  
(d) Flood jet nozzle

**Solution:**

**Requirement Analysis:**

**Insecticides:**
- Need to reach insects hiding in canopy
- Require PENETRATION
- Need FINE DROPLETS for coverage
- Contact action needed

**Nozzle Characteristics:**

| Nozzle Type | Droplet Size | Penetration | Coverage | Best For |
|-------------|--------------|-------------|----------|----------|
| **Flat fan** | Coarse (200-400 μm) | Poor | Uniform | Herbicides |
| **Hollow cone** | **Fine (50-200 μm)** | **Excellent** | **Good** | **Insecticides** ✓ |
| **Deflector** | Very coarse (>400 μm) | Very poor | Limited | Low drift |
| **Flood jet** | Very coarse | Poor | Moderate | Soil |

**Why Hollow Cone?**

**Fine Droplets (50-200 microns):**
- Small size penetrates dense foliage
- High number of droplets
- Better coverage of leaf surfaces
- Reaches undersides of leaves

**High Velocity:**
- Swirl chamber creates high-speed rotation
- Droplets propelled into canopy
- Breaks through dense vegetation

**Spray Pattern:**
- 360° coverage around cone
- Multiple angles of approach
- Covers all leaf orientations

**Why NOT Others?**

**Flat fan:**
- Coarse droplets
- For boom sprayers
- Surface application only
- Poor penetration

**Deflector/Flood:**
- Very large droplets
- Minimal drift (good for herbicides)
- Cannot penetrate canopy
- For soil application

**Answer:** (b) Hollow cone nozzle

**Time:** 2 minutes | **Marks:** 1

---

### Question 12 (Medium) - Safety and PPE #Safety #2020
**A farmer is spraying a moderately toxic pesticide (WHO Class II - Yellow label) using a knapsack sprayer. List the essential Personal Protective Equipment (PPE) required. Explain why each is necessary.**

**Solution:**

**WHO Pesticide Classification:**

| Class | Color | Toxicity | Examples |
|-------|-------|----------|----------|
| Ia | Red (skull) | Extremely toxic | Parathion |
| Ib | Red | Highly toxic | Monocrotophos |
| **II** | **Yellow** | **Moderately toxic** | **Malathion, Dimethoate** |
| III | Blue | Slightly toxic | Glyphosate |
| U | Green | Unlikely hazard | Most biopesticides |

**Essential PPE for Class II Pesticides:**

**1. Protective Clothing (Coveralls):**
- **Why:** Prevents skin contact with spray
- Full-body coverage
- Long sleeves, long pants
- Lightweight, breathable material
- Chemical-resistant fabric

**2. Chemical-Resistant Gloves:**
- **Why:** Hands most exposed (mixing, adjusting)
- Nitrile or neoprene material
- Not leather or cloth (absorbs chemicals)
- Extended cuffs over sleeves

**3. Boots:**
- **Why:** Prevents spills reaching feet
- Rubber or chemical-resistant
- Should cover pant legs
- Easy to clean

**4. Face Shield or Goggles:**
- **Why:** Eye protection from splashes/spray
- Goggles: Side protection
- Face shield: Full face protection
- Must be chemical-resistant, non-fogging

**5. Respirator/Face Mask:**
- **Why:** Prevents inhalation of spray mist
- N95 or chemical cartridge respirator
- Especially important for:
  - Fine droplets
  - Volatile chemicals
  - Prolonged exposure
- Must fit properly (sealed)

**6. Hat/Head Cover:**
- **Why:** Protects head and hair
- Wide-brimmed
- Washable
- Prevents spray accumulation on head

**Optional but Recommended:**

**7. Apron:**
- For mixing operations
- Additional protection

**During Spraying - Safety Practices:**

**Before:**
- ✓ Check wind direction
- ✓ Read label thoroughly
- ✓ Wear ALL PPE
- ✓ Check equipment for leaks

**During:**
- ✓ Spray with wind (not against)
- ✓ Maintain proper distance
- ✓ No eating/drinking/smoking
- ✓ Stay alert for symptoms

**After:**
- ✓ Wash equipment thoroughly
- ✓ Clean PPE separately from regular clothes
- ✓ Shower immediately
- ✓ Wash hands and face thoroughly
- ✓ Store pesticides safely

**Exposure Routes:**

| Route | Risk | Protection |
|-------|------|------------|
| **Dermal (Skin)** | Highest (90%) | Clothing, gloves |
| **Inhalation** | Medium | Respirator |
| **Oral** | Low (if careful) | Hand washing, no eating |
| **Eye** | Low but severe | Goggles, face shield |

**Symptoms of Moderate Toxicity:**
- Headache, dizziness
- Nausea, vomiting
- Excessive sweating
- Blurred vision
- If occurs: Stop work, wash, seek medical help

**Answer:**

**Essential PPE:**
1. Coveralls (skin protection)
2. Chemical-resistant gloves (hand protection)
3. Boots (foot protection)
4. Goggles/face shield (eye protection)
5. Respirator (inhalation protection)
6. Hat (head protection)

**Time:** 5 minutes | **Marks:** 2

---

## 📈 Difficulty Analysis

| Difficulty | Count | Percentage | Topics |
|------------|-------|------------|--------|
| **Easy** | 4 | 33% | Component ID, nozzle selection, pump type |
| **Medium** | 7 | 58% | Calibration, calculations, drift |
| **Hard** | 1 | 9% | Droplet dynamics (physics) |

---

## 🎯 Topic-wise Breakdown

| Topic | Questions | Key Concepts |
|-------|-----------|--------------|
| **Nozzles** | 3 | Types, selection, discharge formula |
| **Calibration** | 2 | Area method, application rate |
| **Application Rate** | 2 | Q×600/(W×S), flow calculations |
| **Drift** | 2 | Droplet dynamics, control methods |
| **Pumps** | 1 | Types, pressure ranges |
| **Safety** | 1 | PPE, toxicity classes |
| **Components** | 1 | Pressure chamber function |

---

## 💡 Preparation Tips

### For Easy Questions (1 mark):
- Know nozzle types and applications
- Component functions
- Basic pump classification
- Memorize standard values

### For Medium Questions (2 marks):
- Master application rate formula: Q×600/(W×S)
- Calibration calculations
- Nozzle discharge: Q = K√P
- Concentration calculations
- Boom height formula

### For Hard Questions:
- Terminal velocity (Stokes' law)
- Multi-step drift calculations
- Physics concepts
- Unit conversions

---

## 🧮 Formula Quick Reference

### Application Rate
$$
\text{Rate (L/ha)} = \frac{Q \times 600}{W \times S}
$$

### Calibration (Area Method)
$$
\text{Rate} = \frac{\text{Volume used}}{\text{Area (m}^2\text{)}} \times 10000
$$

### Nozzle Discharge
$$
Q = K\sqrt{P}
$$

### Boom Height
$$
h = \frac{W}{2\tan(\theta/2)}
$$

### Terminal Velocity
$$
V_t = \frac{d^2(\rho_p - \rho_a)g}{18\mu}
$$

### Concentration
$$
\text{Chemical} = \frac{\text{\%} \times \text{Total volume}}{100}
$$

---

## 🔗 Quick Links

- [Plant Protection Theory](./README.md)
- [Quick Reference](./CheatSheet.md)
- [Farm Machinery Index](../README.md)

---

**Total Questions:** 12  
**Last Updated:** November 2025  
**Source:** GATE AG Previous Year Papers (2020-2024)

---

*For theory concepts, see [Plant Protection README](./README.md)*  
*For quick revision, see [Plant Protection Cheat Sheet](./CheatSheet.md)*
