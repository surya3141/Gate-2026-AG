# 🌡️ Thermal Processing - GATE PYQ Solutions

> **12 Previous Year Questions with Detailed Solutions**

---

## ✅ Solutions

### Q1. D-value Definition (GATE 2024) ⭐

**Question:**  
D-value in thermal processing represents:

(A) Time to heat product to processing temperature  
(B) Time to reduce microbial population by 90%  
(C) Temperature to kill all microorganisms  
(D) Total processing time required

**Solution:**

**D-value (Decimal reduction time):**
- Time required at constant temperature to reduce microbial population by **90% (1 log cycle)**
- Also: Time to reduce population by factor of 10

**Example:**
- Initial count: 10⁶ CFU/ml
- After D-value time: 10⁵ CFU/ml (reduced by 90%)
- After 2D: 10⁴ CFU/ml
- After 6D: 1 CFU/ml (6-log reduction)

**Answer: (B) Time to reduce microbial population by 90%**

**Memory:** "D for Decimal reduction (90% or 1 log)"

---

### Q2. D-value Calculation (GATE 2024) ⭐⭐

**Question:**  
If D₁₂₁ = 0.5 minutes for *Cl. botulinum*, the time required for 12D reduction at 121°C is:

(A) 3 minutes  
(B) 6 minutes  
(C) 12 minutes  
(D) 24 minutes

**Solution:**

**nD reduction time:**
$$
t = n \times D
$$

Given:
- D₁₂₁ = 0.5 min
- n = 12 (12D process)

$$
t = 12 \times 0.5 = 6 \text{ minutes}
$$

**12D concept:**
- Standard for low-acid canned foods
- Initial load: 10¹² spores
- Final: 10⁰ = 1 spore (probability)
- "Commercial sterility"

**Answer: (B) 6 minutes**

---

### Q3. z-value Concept (GATE 2023) ⭐⭐

**Question:**  
The z-value is typically:

(A) 5°C  
(B) 10°C  
(C) 20°C  
(D) 50°C

**Solution:**

**z-value:** Temperature change required for 10-fold (1 log cycle) change in D-value

**Typical values:**
- **Bacterial spores:** z = **10°C** ✓ (most common)
- Vegetative bacteria: z = 4-7°C
- Enzymes: z = 20-50°C

**Example:**
If z = 10°C and D₁₂₁ = 0.5 min, then:
- D₁₁₁ = 5.0 min (10× higher at 10°C lower)
- D₁₃₁ = 0.05 min (10× lower at 10°C higher)

**Answer: (B) 10°C**

**Memory:** "z = 10 for bacterial spores, GATE's favorite one!"

---

### Q4. F-value Definition (GATE 2023) ⭐⭐

**Question:**  
F₀ value with reference temperature 121°C and z = 10°C represents:

(A) D-value at 121°C  
(B) Equivalent time at 121°C  
(C) Heating rate  
(D) Cooling rate

**Solution:**

**F-value (Lethality):**
- **Equivalent time at reference temperature** (Tref = 121°C for F₀)
- Integrates lethal effect over entire process
- Accounts for come-up time and cooling

**Formula:**
$$
F = \int_0^t 10^{(T-T_{ref})/z} dt
$$

**F₀ specifically:**
- Reference: 121°C
- z-value: 10°C
- For low-acid foods: F₀ = 3-5 min typical

**Answer: (B) Equivalent time at 121°C**

---

### Q5. F-value from D-value (GATE 2023) ⭐⭐⭐

**Question:**  
If D₁₂₁ = 0.5 min, initial count = 10⁸, final count = 10², the F-value is:

(A) 1 minute  
(B) 2 minutes  
(C) 3 minutes  
(D) 6 minutes

**Solution:**

**Relationship:**
$$
F = D \times (\log N_0 - \log N) = D \times n
$$

where n = number of log reductions

Given:
- D₁₂₁ = 0.5 min
- N₀ = 10⁸
- N = 10²

**Calculate n:**
$$
n = \log(10^8) - \log(10^2) = 8 - 2 = 6 \text{ log cycles}
$$

**F-value:**
$$
F = 0.5 \times 6 = 3 \text{ minutes}
$$

**Answer: (C) 3 minutes**

---

### Q6. HTST vs LTLT (GATE 2022) ⭐

**Question:**  
Compared to LTLT, HTST pasteurization:

(A) Takes longer time  
(B) Requires lower temperature  
(C) Better retains quality  
(D) Needs batch processing

**Solution:**

**Comparison:**

| Parameter | LTLT | HTST |
|-----------|------|------|
| Temperature | 63°C | 72°C |
| Time | 30 min | 15 sec |
| Process | Batch | Continuous |
| Quality | Good | **Better** ✓ |
| Throughput | Low | High |

**Why HTST better quality?**
- Shorter time at high temp → less nutrient loss
- Less flavor change
- Better color retention
- Equivalent microbial kill

**Answer: (C) Better retains quality**

---

### Q7. UHT Shelf Life (GATE 2022) ⭐

**Question:**  
UHT processed milk has shelf life at room temperature:

(A) 1-2 weeks  
(B) 3-4 weeks  
(C) 6-9 months  
(D) 1-2 years

**Solution:**

**UHT (Ultra High Temperature):**
- 135-150°C for 2-4 seconds
- **Commercial sterility** (not absolute)
- Aseptic packaging

**Shelf life:**
- **6-9 months** at room temperature (unopened)
- No refrigeration needed
- Once opened: 3-5 days in fridge

**Comparison:**
- Pasteurized milk: 7-14 days (refrigerated)
- **UHT milk: 6-9 months** (room temp) ✓

**Answer: (C) 6-9 months**

---

### Q8. Retort Processing (GATE 2021) ⭐⭐

**Question:**  
In retort processing of canned foods, the coldest point (slow heating zone) is typically:

(A) At the can wall  
(B) At the geometric center  
(C) At the top  
(D) At the bottom

**Solution:**

**Heat penetration in cans:**

**For conduction heating (thick products):**
- Heat enters from can wall
- Slowest at **geometric center** ✓
- Examples: Purees, pastes, thick sauces

**For convection heating (liquid products):**
- Convection currents
- Coldest slightly below center
- Examples: Soups, broths

**GATE context:** Usually asks about conduction (most common)

**Answer: (B) At the geometric center**

**Critical:** Temperature probe must be at coldest point for process validation!

---

### Q9. Low-acid vs High-acid (GATE 2021) ⭐

**Question:**  
Low-acid foods are those with pH:

(A) < 3.7  
(B) < 4.5  
(C) > 4.5  
(D) > 7.0

**Solution:**

**FDA classification:**

| Category | pH | Concern | Example |
|----------|-------|---------|---------|
| **High-acid** | **< 4.5** | Molds, yeasts | Fruits, pickles |
| **Low-acid** | **> 4.5** | ***Cl. botulinum*** | Vegetables, meat, milk |

**Why pH 4.5 critical?**
- ***Clostridium botulinum* cannot grow below pH 4.5**
- Low-acid foods need sterilization (121°C, 12D)
- High-acid foods need only pasteurization (~100°C)

**Answer: (C) > 4.5**

**Memory:** "Above 4.5, botulinum survives!"

---

### Q10. Come-up Time (GATE 2020) ⭐⭐

**Question:**  
Come-up time in thermal processing contributes to:

(A) Zero lethality  
(B) Additional lethality  
(C) Negative lethality  
(D) No effect on process

**Solution:**

**Come-up time:** Time for retort to reach processing temperature from start

**Lethality contribution:**
- Temperature rising during come-up
- 100°C → 121°C (example)
- Microorganisms being killed throughout
- **Contributes to total F-value** ✓

**F-value calculation includes:**
1. Come-up time (heating)
2. Hold time (at set temperature)
3. Cooling time

**Answer: (B) Additional lethality**

**Practical:** Come-up lethality can be 10-30% of total F₀

---

### Q11. Aseptic Processing (GATE 2020) ⭐

**Question:**  
In aseptic processing, the product and package are:

(A) Sterilized together  
(B) Sterilized separately  
(C) Not sterilized  
(D) Only product is sterilized

**Solution:**

**Aseptic processing:**

1. **Product sterilized separately** (UHT, 135-150°C/2-4s)
2. **Package sterilized separately** (H₂O₂, UV, heat)
3. **Filling in sterile environment**
4. **Sealing maintains sterility**

**Advantages:**
- Better quality (short heat time for product)
- Flexible packaging (Tetra Pak, pouches)
- Room temperature storage

**Answer: (B) Sterilized separately**

---

### Q12. Thermal Death Time (GATE 2020) ⭐⭐

**Question:**  
If D₁₂₁ = 0.4 min and z = 10°C, the D-value at 111°C is:

(A) 0.4 min  
(B) 0.04 min  
(C) 4 min  
(D) 40 min

**Solution:**

**D-value temperature relationship:**
$$
\log\left(\frac{D_1}{D_2}\right) = \frac{T_2 - T_1}{z}
$$

Given:
- D₁₂₁ = 0.4 min (at T₁ = 121°C)
- z = 10°C
- Find D₁₁₁ (at T₂ = 111°C)

$$
\log\left(\frac{D_{121}}{D_{111}}\right) = \frac{111 - 121}{10} = \frac{-10}{10} = -1
$$

$$
\frac{D_{121}}{D_{111}} = 10^{-1} = 0.1
$$

$$
D_{111} = \frac{D_{121}}{0.1} = \frac{0.4}{0.1} = 4 \text{ min}
$$

**Answer: (C) 4 minutes**

**Check:** Lower temp → Higher D-value (takes longer) ✓

---

## 📊 Summary

### Key Formulas
1. **D-value:** 90% reduction time
2. **nD process:** t = n × D
3. **F-value:** F = D × (log N₀ - log N)
4. **D-T relationship:** log(D₁/D₂) = (T₂-T₁)/z
5. **z-value:** 10°C for spores

### Must Remember
- **D₁₂₁ for Cl. botulinum:** 0.2-0.5 min
- **12D process:** Commercial sterility
- **F₀:** 3-5 min for low-acid foods
- **z-value:** 10°C (bacterial spores)
- **pH 4.5:** Low-acid vs high-acid boundary
- **UHT:** 6-9 months shelf life

---

*[CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
