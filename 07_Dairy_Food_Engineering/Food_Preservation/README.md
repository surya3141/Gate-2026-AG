# 🧊 Food Preservation

> **Comprehensive Theory for GATE 2026**

---

## 📚 Table of Contents
1. [Water Activity](#water-activity)
2. [Drying & Dehydration](#drying-dehydration)
3. [Freezing](#freezing)
4. [Chemical Preservation](#chemical-preservation)
5. [Modified Atmosphere Storage](#modified-atmosphere)
6. [Hurdle Technology](#hurdle-technology)
7. [Cold Storage](#cold-storage)

---

## 💧 Water Activity (aw) 🔥🔥🔥

### Definition

**Water activity (aw):** Ratio of vapor pressure of food to vapor pressure of pure water at same temperature

$$
a_w = \frac{P}{P_0} = \frac{ERH}{100}
$$

where:
- P = Vapor pressure of food water
- P₀ = Vapor pressure of pure water at same T
- ERH = Equilibrium Relative Humidity (%)

**Range:** 0 to 1.0
- Pure water: aw = 1.0
- Bone-dry food: aw = 0

### Microbial Growth Limits 🔥

| aw Range | Microbial Growth | Food Examples | Storage |
|----------|------------------|---------------|---------|
| **0.95-1.00** | Bacteria, yeast, mold | Fresh meat, milk, vegetables, fruits | Refrigeration needed |
| **0.90-0.95** | Most bacteria, yeast, mold | Bread, cheese, cured meat | Short shelf life |
| **0.80-0.90** | Most yeast, mold | Salami, aged cheese, jam | Moderate shelf life |
| **0.60-0.80** | Mold only | Dried fruits, nuts, flour, honey | Long shelf life |
| **< 0.60** | **MICROBIALLY SAFE** | **Crackers, cereals, milk powder, pasta** | **Very long shelf life** ✓ |

**Critical limits:**
- Most bacteria: > 0.90
- Most yeast: > 0.80
- Most mold: > 0.70
- **Safe storage: < 0.60** (xerophilic molds stopped)

### Factors Affecting aw

**1. Moisture content:** Higher moisture → Higher aw (but not linear!)

**2. Solutes (sugars, salts):**
- **Raoult's Law** (ideal solutions):
  
$$
a_w = X_{water} = \frac{n_{water}}{n_{water} + n_{solute}}
$$

- More solute → Lower aw
- Salt more effective than sugar (ionic dissociation)

**Example:**
- 1 kg water = 55.5 moles
- Add 100 g NaCl = 1.71 moles → 3.42 moles ions (Na⁺, Cl⁻)
- aw = 55.5/(55.5+3.42) = 0.942

**3. Temperature:**
- Generally, aw increases slightly with temperature
- Effect small compared to composition

### aw vs Moisture Content

**Important:** aw ≠ moisture content!

**Moisture sorption isotherm:**
- Plot of aw vs moisture content at constant T
- S-shaped curve (sigmoidal)
- Hysteresis: Adsorption ≠ Desorption

**Same aw, different moisture:**
- Starch: aw 0.5 → 10% moisture
- Protein: aw 0.5 → 15% moisture

### Equilibrium Relative Humidity (ERH)

**Relationship:**
$$
ERH (\%) = a_w \times 100
$$

**Moisture gain/loss:**
- **Storage RH > Food ERH:** Food gains moisture
- **Storage RH < Food ERH:** Food loses moisture
- **Storage RH = Food ERH:** Equilibrium (no change)

**Example:**
- Product: aw = 0.60 (ERH = 60%)
- Storage: 75% RH
- Result: Product **gains moisture** (75 > 60)

---

## ☀️ Drying & Dehydration

### Objectives
1. Lower aw to < 0.60 (microbial safety)
2. Reduce weight/volume (transport, storage)
3. Extend shelf life (6-12 months)

### Drying Curve Phases 🔥

**1. Constant rate period:**
- **Surface moisture evaporation**
- Drying rate = evaporation rate from free water
- Surface acts like pure water
- Short for most foods (hygroscopic nature)

**2. Falling rate period:**
- **Internal moisture diffusion to surface**
- Rate decreases as moisture content decreases
- Dominant period for most foods
- Diffusion is limiting step

**Graph:**
```
Moisture    |     A (initial heating)
Content     |    / 
            |   /  B (constant rate)
            |  /____
            | /      \
            |/        \ C (falling rate)
            |          \_____
            |________________
                Time
```

### Drying Methods

**1. Sun/Solar Drying:**
- Traditional method
- Low cost
- Slow (2-5 days)
- Weather dependent
- Quality: Fair (dust, insects, uneven)

**2. Cabinet/Tray Dryer:**
- Batch operation
- Trays in insulated cabinet
- Hot air circulation (50-80°C)
- Use: Fruits, vegetables
- Capacity: 10-500 kg/batch

**3. Tunnel Dryer:**
- Semi-continuous
- Trolleys move through tunnel
- Counter-current or co-current airflow
- Use: Large-scale fruit/vegetable drying

**4. Spray Dryer:**
- **Continuous, very fast (5-30 seconds)**
- **Atomization → Hot air drying → Powder collection**
- **Inlet:** 180-230°C
- **Outlet:** 70-100°C
- **Use:** Milk powder, coffee, flavors ✓
- **Advantages:** Minimal heat damage, free-flowing powder

**5. Drum Dryer:**
- Thin film on heated drum
- Scrape off dried flakes
- High temperature (120-150°C)
- Use: Mashed potato, baby food
- Quality: Lower (heat damage)

**6. Freeze Dryer:**
- **Sublimation drying (ice → vapor)**
- **-40 to -50°C, high vacuum**
- **Best quality:** Aroma, color, rehydration ✓
- **Disadvantages:** Very expensive, slow
- **Use:** High-value products (coffee, strawberries)

**7. Fluidized Bed Dryer:**
- Particles suspended in hot air
- Good heat/mass transfer
- Use: Grains, peas, particulates

### Moisture Content Expressions

**Wet basis (wb):**
$$
M_{wb} = \frac{W_{water}}{W_{wet}} \times 100
$$

**Dry basis (db):**
$$
M_{db} = \frac{W_{water}}{W_{dry}} \times 100
$$

**Conversion:**
$$
M_{db} = \frac{M_{wb}}{100 - M_{wb}} \times 100
$$

$$
M_{wb} = \frac{M_{db}}{100 + M_{db}} \times 100
$$

(Same as grain drying formulas!)

### Blanching Before Drying 🔥

**Purpose:**
1. **Inactivate enzymes** (prevent browning, off-flavors)
2. Remove air (better color)
3. Soften tissue
4. Reduce microbial load

**Methods:**
- **Water blanching:** 100°C, 2-5 minutes
- **Steam blanching:** Less nutrient loss
- **Microwave blanching:** Rapid

**Test:** Peroxidase test (negative = adequate blanching)

### Sulfuring/Sulfiting

**Purpose:** Prevent enzymatic browning in dried fruits

**SO₂ (Sulfur dioxide):**
- Inhibits polyphenol oxidase
- Preserves bright color (golden raisins, apricots)
- Antimicrobial, antioxidant
- Dosage: 500-2000 ppm

**Methods:**
- Sulfur burning (gaseous SO₂)
- Sodium metabisulfite dip (liquid)

**Concern:** Allergen for some people (labeling required)

---

## ❄️ Freezing

### Principles

**Objectives:**
1. Lower temperature to stop microbial growth (<-18°C)
2. Slow enzyme activity
3. Extend shelf life (6-12 months)

**Microbial limits:**
- -10°C: Most growth stopped
- **-18°C: Standard frozen storage** ✓
- -30°C: Fast freezing

### Freezing Curve

**Phases:**
1. **Cooling (A-B):** Cool to freezing point
2. **Supercooling (B-C):** Below freezing, no ice (metastable)
3. **Nucleation (C):** Ice crystal formation starts
4. **Freezing (C-D):** Latent heat removal (temperature plateau)
5. **Tempering (D-E):** Final cooling to storage temperature

**Heat removed:**
$$
Q = m \times (c_1 \Delta T_1 + L_f + c_2 \Delta T_2)
$$

where:
- c₁ = Specific heat above freezing (~4 kJ/kg·°C)
- L_f = Latent heat of freezing (~335 kJ/kg for water, ~200-280 for foods)
- c₂ = Specific heat below freezing (~2 kJ/kg·°C)

### Freezing Rate Effect 🔥🔥

**Fast freezing:**
- **Many nucleation sites → Small ice crystals**
- **Less cell damage → Better quality** ✓
- Less drip loss on thawing
- Better texture, appearance

**Slow freezing:**
- Few nucleation sites → Large ice crystals
- Pierce cell walls → Cell rupture
- More drip loss (20-30%)
- Mushy texture after thawing

**IQF (Individual Quick Freezing):**
- Very fast freezing (-30 to -40°C)
- Cryogenic (liquid N₂, CO₂)
- Best quality

### Freezing Methods

**1. Air blast freezing:**
- Cold air (-30 to -40°C), high velocity (3-5 m/s)
- Most common commercial method
- Freezing time: 2-6 hours

**2. Plate freezing:**
- Contact with refrigerated plates
- Good for flat packages (fish fillets)
- Fast, efficient

**3. Immersion freezing:**
- Submerge in refrigerated brine/glycol
- Very fast
- Use: Packaged products

**4. Cryogenic freezing:**
- Liquid nitrogen (-196°C) or CO₂ (-78°C)
- Extremely fast (minutes)
- Best quality
- High cost

### Freezing Point Depression

**Pure water:** 0°C

**Foods:** -0.5 to -3°C (due to solutes)

**Raoult's Law:**
$$
\Delta T_f = K_f \times m
$$

where:
- ΔT_f = Freezing point depression
- K_f = Cryoscopic constant (1.86°C·kg/mol for water)
- m = Molality of solution

**Example:**
- Orange juice: 12% sugar
- Freezing point: -2°C

### Thawing

**Methods:**
1. **Refrigerated thawing:** 4°C, slow (24-48 hrs), best quality
2. **Room temperature:** Faster, but microbial risk on surface
3. **Cold water:** Submerge sealed package, faster
4. **Microwave:** Very fast, uneven heating
5. **Cooking from frozen:** No thaw needed (some products)

**Drip loss:** Water lost during thawing
- Fast freeze → 5-10% drip
- Slow freeze → 20-30% drip

---

## 🧪 Chemical Preservation

### Common Preservatives

**1. Sodium benzoate:**
- **Use:** High-acid foods (pH < 4.5)
- Jams, pickles, soft drinks
- **Max:** 0.1% (1000 ppm)
- Mechanism: Inhibits yeasts, molds

**2. Potassium sorbate:**
- **Use:** Cheese, wine, dried fruits
- Effective against yeasts, molds
- **Max:** 0.1-0.3%
- More effective at pH 5-6 than benzoate

**3. Sodium nitrite/nitrate:**
- **Use:** Cured meats
- Pink color, flavor, inhibits *C. botulinum*
- **Max:** 200 ppm (nitrite), 500 ppm (nitrate)
- Concern: Nitrosamine formation

**4. Sulfur dioxide (SO₂):**
- **Use:** Dried fruits, wine
- Prevents browning, antimicrobial
- **Max:** 2000 ppm (dried fruits)
- Allergen concern

**5. Propionic acid:**
- **Use:** Bread (anti-mold)
- Naturally in Swiss cheese
- **Max:** 0.3%

### Salt & Sugar Preservation

**Salt (NaCl):**
- Lowers aw
- Osmotic shock to microbes
- **Concentration:** 10-20% (preservation)
- Use: Pickles, cured meats

**Sugar:**
- Lowers aw
- **Concentration:** 65-70% (jams, jellies)
- Less effective than salt (molecular)

---

## 📦 Modified Atmosphere Storage

### MAP (Modified Atmosphere Packaging) 🔥

**Principle:** Alter gas composition around product

**Typical composition:**
- **O₂:** 2-5% (reduced from 21%)
- **CO₂:** 3-10% (increased from 0.03%)
- **N₂:** Balance (85-95%)

**Benefits:**
1. **Low O₂:** Reduces respiration, delays ripening
2. **High CO₂:** Inhibits microbial growth (especially aerobic bacteria)
3. **Extends shelf life:** 2-4 times

**Applications:**
- Fresh-cut produce
- Bakery products
- Meat, poultry
- Cheese

**Methods:**
1. **Gas flushing:** Replace air with gas mix
2. **Vacuum packaging:** Remove air (0-1% O₂)
3. **Active packaging:** Scavengers (O₂ absorbers, CO₂ emitters)

### CA (Controlled Atmosphere) Storage

**Difference from MAP:**
- **MAP:** One-time gas change (passive)
- **CA:** Continuous monitoring and adjustment (active)

**Use:** Long-term storage (apples, pears)

**Typical conditions:**
- O₂: 1-3%
- CO₂: 0-5%
- Temperature: 0-4°C
- RH: 90-95%

**Benefits:** 6-12 months storage (vs 2-3 months ambient)

---

## 🛡️ Hurdle Technology 🔥

### Concept

**Multiple preservation factors (hurdles) applied together**

Each hurdle stresses microorganisms. Combined effect > individual effects.

**Common hurdles:**
1. **Temperature (T):** Refrigeration, heating
2. **Water activity (aw):** Drying, salt, sugar
3. **pH:** Acidification
4. **Redox potential (Eh):** Vacuum, modified atmosphere
5. **Preservatives:** Benzoate, sorbate, nitrite
6. **Competitive flora:** Fermentation (lactic acid bacteria)

### Example: Jam

**Hurdles:**
1. **High sugar (65-70%):** aw = 0.75-0.80 (mold limit)
2. **Low pH (3.0-3.5):** Acidification with citric/malic acid
3. **Heat treatment:** 85-90°C (pasteurization)
4. **Sealed container:** Prevents recontamination

**Result:** 12-24 months shelf life at room temperature

### Example: Fermented Sausage

**Hurdles:**
1. **Salt (2-3%):** Lowers aw
2. **Nitrite (150 ppm):** Anti-*Clostridium*
3. **Fermentation:** pH drops to 4.5-5.0 (lactic acid)
4. **Drying:** aw drops to 0.85-0.90
5. **Smoking:** Antimicrobial compounds

**Result:** Several months shelf life, no refrigeration

---

## 🏢 Cold Storage

### Refrigerated Storage (0-10°C)

**Objectives:**
- Slow microbial growth (not stop)
- Slow biochemical reactions
- Extend shelf life (days to weeks)

**Temperature zones:**
- **0-2°C:** Meat, fish, dairy
- **2-5°C:** Cooked foods, fruits, vegetables
- **5-10°C:** Potatoes, tropical fruits

**Important:** **Potatoes 5-10°C** (not 0-5°C!)
- Below 5°C → Cold sweetening (starch → sugar)
- Sweet taste, dark frying color

**Chilling injury:** Tropical fruits damaged below 10-13°C
- Bananas: 13-15°C
- Mangoes: 10-13°C
- Symptoms: Discoloration, pitting, faster decay

### Relative Humidity

**Importance:**
- **Too low (<80%):** Wilting, weight loss
- **Too high (>95%):** Microbial growth, condensation
- **Optimal:** 90-95% for most produce

**Control methods:**
- Humidifiers
- Wet pads
- Perforated film packaging

### Design Parameters

**Cold storage room:**

**1. Insulation:** Polyurethane foam (50-100 mm)

**2. Refrigeration capacity:**
$$
Q = Q_{product} + Q_{infiltration} + Q_{equipment} + Q_{respiration}
$$

**3. Air circulation:** 0.5-1.5 m/s (uniform temperature)

**4. Defrosting:** Automatic (every 6-12 hours)

---

## 📈 Summary

### Critical Concepts
```
1. aw < 0.6 for microbial safety
2. aw = P/P₀ = ERH/100
3. Fast freezing → Small crystals → Better quality
4. Blanching before drying/freezing
5. MAP: Low O₂, High CO₂
6. Hurdle technology: Multiple barriers
7. Potato storage: 5-10°C (not colder)
```

### Must-Remember Values
```
Safe aw: < 0.60
Bacteria limit: aw > 0.90
Yeast limit: aw > 0.80
Mold limit: aw > 0.70
Frozen storage: -18°C
Fast freeze: -30 to -40°C
MAP O₂: 2-5%, CO₂: 3-10%
Potato: 5-10°C
UHT + aseptic: 6-9 months
```

### Key Formulas
```
aw = P/P₀ = ERH/100
ERH(%) = aw × 100
Mdb = Mwb/(100-Mwb) × 100
Mwb = Mdb/(100+Mdb) × 100
Q = m(c₁ΔT₁ + Lf + c₂ΔT₂)
```

---

*[Solutions](./Solutions.md) | [CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
