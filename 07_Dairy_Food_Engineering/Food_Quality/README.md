# 🔬 Food Quality & Safety

> **Comprehensive Theory for GATE 2026**

---

## 📚 Table of Contents
1. [pH & Acidity](#ph-acidity)
2. [Moisture Determination](#moisture-determination)
3. [Proximate Analysis](#proximate-analysis)
4. [Food Microbiology](#food-microbiology)
5. [HACCP](#haccp)
6. [Food Standards](#food-standards)
7. [Sensory Evaluation](#sensory-evaluation)
8. [Adulteration Detection](#adulteration-detection)

---

## 🎨 pH & Acidity

### pH Scale 🔥

**Definition:** Negative logarithm of hydrogen ion concentration

$$
pH = -\log[H^+]
$$

**Scale:** 0 to 14
- **< 7:** Acidic
- **= 7:** Neutral
- **> 7:** Basic (alkaline)

### pH of Common Foods

| Food | pH | Classification |
|------|-----|----------------|
| Lemon juice | 2.0-2.5 | Very acidic |
| Vinegar | 2.4-3.4 | Very acidic |
| Orange juice | 3.5-4.0 | Acidic |
| Tomato | 4.0-4.5 | Acidic |
| **Banana** | **4.5-5.2** | **pH boundary** |
| **Fresh milk** | **6.6-6.8** | **Slightly acidic** 🔥 |
| Egg white | 7.6-8.0 | Slightly alkaline |
| Baking soda solution | 8.3 | Alkaline |

**Critical pH values:**
- **pH 4.5:** Divides low-acid (>4.5) from high-acid (<4.5) foods
  - ***C. botulinum* won't grow below pH 4.5**
  - Low-acid need 121°C sterilization
  - High-acid need 100°C pasteurization only

### Titratable Acidity 🔥

**Definition:** Total acid content determined by titration with standard alkali

**Formula:**
$$
\text{Acidity (\%)} = \frac{V \times N \times E}{W} \times 100
$$

where:
- V = Volume of NaOH used (ml)
- N = Normality of NaOH
- E = Equivalent weight of acid (g)
- W = Sample weight (g)

**Equivalent weights:**
- **Lactic acid:** 0.090 g (or 90 mg) → Use **0.009** in formula
- Citric acid: 0.064 g
- Acetic acid: 0.060 g

**Milk acidity (as % lactic acid):**
$$
\text{Acidity (\%)} = \frac{V \times N \times 0.009}{W} \times 100
$$

**Example:**
- Sample: 10 g milk
- NaOH used: 5 ml of 0.1 N
- Acidity = (5 × 0.1 × 0.009 / 10) × 100 = **0.045%** = **0.45 g/L**

**Fresh milk:** 0.14-0.16% lactic acid
**Sour milk:** > 0.18% lactic acid

### pH vs Titratable Acidity

**Important difference:**
- **pH:** Intensity (concentration of free H⁺)
- **Titratable Acidity:** Capacity (total acid that can be neutralized)

**Example:**
- 0.1 M HCl: pH 1, low TA
- Lemon juice: pH 2.5, high TA (citric acid)
- Both acidic, but lemon has more total acid

---

## 💧 Moisture Determination

### Standard Method: Oven Drying 🔥

**Procedure:**
1. **Weigh** empty aluminum dish + lid → W₁
2. **Add sample** → W₂ (typically 5-10 g)
3. **Dry** in oven at **103-105°C**
4. **Cool** in desiccator (prevent moisture uptake)
5. **Weigh** → W₃
6. **Repeat** until constant weight (difference < 0.5 mg)

**Calculation (wet basis):**
$$
M_{wb} (\%) = \frac{W_2 - W_3}{W_2 - W_1} \times 100
$$

**Calculation (dry basis):**
$$
M_{db} (\%) = \frac{W_2 - W_3}{W_3 - W_1} \times 100
$$

**Time:** 2-4 hours (depends on moisture level)

**Limitations:**
- Volatile compounds lost (not just water)
- Maillard browning (overestimation)
- Not suitable for high-sugar foods

### Alternative Methods

**1. Karl Fischer Method:**
- **Chemical titration** (specific to water)
- Very accurate (±0.01%)
- Use: Oils, fats, chocolate
- Fast (minutes)
- Expensive reagent

**2. Vacuum Oven:**
- Lower temperature (60-70°C), vacuum
- Less decomposition
- Use: Heat-sensitive materials

**3. Microwave Drying:**
- Very fast (5-10 minutes)
- Not standard, but screening
- Calibration needed

**4. NIR (Near-Infrared) Spectroscopy:**
- Non-destructive, instant
- Requires calibration for each product
- Use: Online monitoring (grain, feed)

**5. Moisture Meter (Capacitance/Resistance):**
- Electrical properties change with moisture
- Quick, portable
- Use: Grains (calibrated)

---

## 📊 Proximate Analysis 🔥

**Definition:** Standard analysis for basic composition

**Six components:**

### 1. Moisture

**Method:** Oven drying 105°C (described above)

**Importance:**
- Spoilage risk
- Processing parameters
- Legal standards (e.g., milk powder <5%)

### 2. Protein

**Method:** Kjeldahl nitrogen determination

**Principle:** Total N → Protein

**Steps:**
1. **Digestion:** Sample + H₂SO₄ + catalyst → NH₄⁺
2. **Distillation:** NH₄⁺ + NaOH → NH₃ (distill into boric acid)
3. **Titration:** Titrate with HCl

**Calculation:**
$$
N (\%) = \frac{(V_{sample} - V_{blank}) \times N_{HCl} \times 14.007}{W_{sample}} \times 100
$$

$$
\text{Protein (\%)} = N (\%) \times \text{Factor}
$$

**Conversion factors:** 🔥
- **General:** 6.25 (assumes 16% N in protein)
- **Milk:** **6.38** (casein-rich)
- **Wheat:** 5.70 (gluten)
- **Rice:** 5.95

**Why different?**
- Different proteins have different amino acid compositions
- Different % nitrogen
- Milk proteins: ~15.7% N → 100/15.7 = 6.38

**Example (milk):**
- N% = 0.53%
- Protein = 0.53 × 6.38 = **3.38%**

### 3. Fat

**Method:** Soxhlet extraction

**Principle:** Solvent extraction of lipids

**Solvents:** Petroleum ether, hexane, diethyl ether

**Steps:**
1. **Dry sample** (if high moisture)
2. **Extract** with solvent (6-8 hours)
3. **Evaporate solvent**
4. **Weigh** extracted fat

**Calculation:**
$$
\text{Fat (\%)} = \frac{W_{fat}}{W_{sample}} \times 100
$$

**Alternative methods:**
- **Gerber (milk):** Sulfuric acid + centrifuge
- **Babcock (milk):** Similar to Gerber
- **Rose-Gottlieb (milk):** Solvent extraction (reference)

### 4. Ash

**Method:** Muffle furnace incineration

**Principle:** Burn organic matter, residue = minerals

**Procedure:**
1. **Weigh** sample in crucible
2. **Char** on hot plate (smoke removal)
3. **Ash** in muffle furnace at **550°C** (4-6 hours)
4. **Cool** in desiccator
5. **Weigh** ash residue

**Calculation:**
$$
\text{Ash (\%)} = \frac{W_{ash}}{W_{sample}} \times 100
$$

**Typical values:**
- Cereals: 1-3%
- Milk: 0.7%
- Vegetables: 1-2%

**Composition:** Ca, P, K, Na, Mg, Fe, Zn, etc.

### 5. Crude Fiber

**Method:** Sequential acid-alkali digestion

**Principle:** Removes soluble components, leaves cellulose + lignin

**Steps:**
1. **Acid digestion:** 1.25% H₂SO₄, boil 30 min
2. **Filter, wash**
3. **Alkali digestion:** 1.25% NaOH, boil 30 min
4. **Filter, wash, dry**
5. **Ash** at 550°C
6. **Weigh** (weight loss = fiber)

**Calculation:**
$$
\text{Crude Fiber (\%)} = \frac{W_{before ash} - W_{ash}}{W_{sample}} \times 100
$$

**Typical values:**
- Refined flour: 0.5-1%
- Whole wheat: 10-12%
- Rice bran: 20-25%

**Note:** "Crude fiber" ≠ "Dietary fiber"
- Crude fiber: Indigestible cellulose + lignin (underestimates)
- Dietary fiber: All non-digestible polysaccharides (more accurate)

### 6. Carbohydrate (by difference)

**Calculation:**
$$
\text{Carbohydrate (\%)} = 100 - (\text{Moisture} + \text{Protein} + \text{Fat} + \text{Ash} + \text{Fiber})
$$

**Not measured directly** (includes errors from all other analyses)

### Summary Table

| Component | Method | Typical Time |
|-----------|--------|--------------|
| **Moisture** | Oven 105°C | 2-4 hours |
| **Protein** | Kjeldahl | 4-6 hours |
| **Fat** | Soxhlet | 6-8 hours |
| **Ash** | Muffle 550°C | 4-6 hours |
| **Fiber** | Acid-alkali | 3-4 hours |
| **Carbohydrate** | By difference | - |

---

## 🦠 Food Microbiology

### Spoilage Microorganisms

**1. Bacteria:**
- *Pseudomonas* (meat, dairy, vegetables)
- *Bacillus* (spore-formers, canned foods)
- *Lactobacillus* (dairy souring)

**2. Yeasts:**
- *Saccharomyces* (fruits, juices)
- Fermentation → alcohol + CO₂

**3. Molds:**
- *Aspergillus* (grains, nuts)
- *Penicillium* (cheese, bread)
- Some produce mycotoxins (aflatoxin)

### Pathogenic Microorganisms

**1. *Clostridium botulinum*:**
- **Anaerobic spore-former**
- **Produces deadly botulinum toxin**
- **Growth pH > 4.5** (low-acid foods)
- **Target for canning:** 12D reduction (121°C)

**2. *Salmonella*:**
- Poultry, eggs, meat
- Gastroenteritis
- D₇₀ = 0.5-1 min

**3. *Staphylococcus aureus*:**
- Toxin-producer (heat-stable enterotoxin)
- Cooked foods, dairy
- Prevention: < 7°C or > 60°C

**4. *Listeria monocytogenes*:**
- Grows at refrigeration temperatures
- Ready-to-eat foods, soft cheese
- Risk: Pregnant women

**5. *E. coli* O157:H7:**
- Produces Shiga toxin
- Ground beef, raw produce
- **Juice pasteurization: 5-log reduction**

### Microbial Counts

**Total Plate Count (TPC):**
- Pour plate method
- Incubate 35°C, 48 hours
- CFU/g or CFU/ml

**Standards:**
- Fresh milk: < 100,000 CFU/ml
- Pasteurized milk: < 30,000 CFU/ml
- Dried foods: < 10,000 CFU/g

---

## ✅ HACCP 🔥

**HACCP:** Hazard Analysis and Critical Control Points

**Definition:** Systematic preventive approach to food safety

### Seven Principles

**1. Conduct Hazard Analysis**
- Identify biological, chemical, physical hazards
- Assess severity and likelihood

**2. Determine Critical Control Points (CCPs)** 🔥
- **CCP:** Step where control can prevent/eliminate hazard
- **Decision tree:** Is control essential for safety?

**Examples of CCPs:**
- **Pasteurization** (milk): Pathogen kill
- **Metal detection** (finished product): Foreign object
- **Refrigeration** (cold storage): Pathogen growth
- **pH control** (canning): *C. botulinum*

**3. Establish Critical Limits**
- **Measurable parameter** at CCP
- Examples:
  - Pasteurization: **72°C for 15 seconds**
  - Refrigeration: **≤ 4°C**
  - pH: **< 4.5** (high-acid canned foods)
  - Metal detection: **≤ 2 mm ferrous**

**4. Establish Monitoring Procedures**
- Continuous or batch monitoring
- Who, what, when, how
- **Examples:**
  - Temperature recording charts
  - pH meters every batch
  - Metal detector check every 30 min

**5. Establish Corrective Actions**
- What to do if critical limit violated
- **Examples:**
  - Reprocess if under-pasteurized
  - Retest if pH out of range
  - Hold product if metal detected

**6. Establish Verification Procedures**
- Confirm HACCP system working
- **Examples:**
  - Calibrate equipment (thermometers, pH meters)
  - Microbial testing (finished product)
  - Review records monthly
  - Audit HACCP plan annually

**7. Establish Record-Keeping and Documentation**
- **Records:**
  - HACCP plan
  - Hazard analysis
  - CCP monitoring charts
  - Corrective actions log
  - Verification records
- **Retention:** Typically 2 years

### Prerequisite Programs

Before HACCP:
1. **GMP** (Good Manufacturing Practices)
2. **Sanitation** (cleaning, pest control)
3. **Training** (personnel hygiene)
4. **Supplier control**
5. **Traceability**

---

## 📜 Food Standards (India)

### BIS (Bureau of Indian Standards)

**IS Codes:** Indian Standards

**Examples:**
- **IS 1155:** Butter (min 80% fat)
- **IS 1479:** Ghee
- **IS 2802:** Paneer
- **IS 13078:** Pasteurized milk

### FSSAI (Food Safety and Standards Authority of India)

**Regulates:** Food safety and standards in India

**FSS Act 2006:** Primary legislation

**Standards:**
- Milk: Fat 3.5%, SNF 8.5% (full cream)
- Toned milk: Fat 3%, SNF 8.5%
- Double-toned: Fat 1.5%, SNF 9%
- Skimmed: Fat 0.5%, SNF 8.5%

**Food additives:** Permitted lists (INS numbers)

**Labeling:** Mandatory declarations
- Ingredients list
- Nutritional information
- Allergen declaration
- Manufacturing date, expiry
- FSSAI license number

---

## 👅 Sensory Evaluation 🔥

### Methods

**1. 9-Point Hedonic Scale** (Preference/Acceptance)
```
9 - Like extremely
8 - Like very much
7 - Like moderately
6 - Like slightly
5 - Neither like nor dislike
4 - Dislike slightly
3 - Dislike moderately
2 - Dislike very much
1 - Dislike extremely
```

**Use:** Consumer acceptance studies

**2. Triangle Test** (Difference Testing)
- Present 3 samples (2 identical, 1 different)
- Identify the odd sample
- **Purpose:** Detect if difference exists

**3. Duo-Trio Test** (Difference Testing)
- Reference sample + 2 test samples (1 matches reference)
- Match to reference
- **Purpose:** Quality control

**4. Ranking Test**
- Rank samples in order of preference/intensity
- **Purpose:** Product comparison

**5. Rating Scales**
- Intensity scales (e.g., sweetness 1-10)
- **Purpose:** Quantify attribute

### Sensory Attributes

**Appearance:** Color, size, shape, defects

**Texture:** Hardness, chewiness, crispness, smoothness

**Flavor:**
- **Taste:** Sweet, sour, salty, bitter, umami
- **Aroma:** Nose perception (volatile compounds)

**Mouthfeel:** Astringency, creaminess

---

## 🔍 Adulteration Detection (Milk) 🔥

### Common Adulterants

**1. Water**
- **Detection:** Lactometer (density), Freezing point depression
- Fresh milk density: 1.028-1.032 kg/L
- Freezing point: -0.525 to -0.550°C
- **Effect:** Lower density, higher freezing point

**2. Formalin** (Preservative - illegal)
- **Test:** Rosolic acid (Hehner test)
- **Procedure:** Milk + Rosolic acid + HCl
- **Positive:** Red/violet ring at interface
- **Why used:** Preserves milk (bactericidal)

**3. Urea** (Increases SNF reading)
- **Test:** Urease test
- **Procedure:** Milk + urease enzyme
- **Positive:** Pink color (ammonia formation)

**4. Starch** (Increases viscosity)
- **Test:** Iodine test
- **Procedure:** Milk + iodine solution
- **Positive:** Blue color

**5. Neutralizers** (Sodium carbonate/bicarbonate - masks sourness)
- **Test:** Rosolic acid, COB (Colour of Bromothymol Blue)
- **Positive:** Pink color (rosolic acid)

**6. Sugar** (Increases sweetness, SNF)
- **Test:** Resorcinol test
- **Positive:** Red color on heating

---

## 📈 Summary

### Critical Values
```
Milk pH: 6.6-6.8
Fresh milk acidity: 0.14-0.16% LA
pH boundary: 4.5 (low-acid vs high-acid)
Kjeldahl factors: General 6.25, Milk 6.38
Moisture method: 105°C oven drying
Ash temperature: 550°C muffle
```

### Must-Remember Concepts
```
1. pH 4.5 divides low/high-acid foods
2. Acidity expressed as % lactic acid (milk)
3. Kjeldahl: N% × 6.38 (milk protein)
4. Proximate: M-P-F-F-A-C (6 components)
5. HACCP: CCP = Critical Control Point
6. 9-point hedonic = Preference test
7. Formalin test = Rosolic acid
```

---

*[Solutions](./Solutions.md) | [CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
