# 🌾 Grain Drying - GATE PYQ Solutions

> **14 Previous Year Questions with Detailed Solutions**

---

## 📚 Question Index

| Q# | Topic | Difficulty | Time | Year |
|----|-------|------------|------|------|
| 1 | MC conversion wb to db | ⭐ Easy | 2 min | 2024 |
| 2 | MC conversion db to wb | ⭐ Easy | 2 min | 2024 |
| 3 | Safe storage moisture | ⭐ Easy | 1 min | 2024 |
| 4 | Drying rate calculation | ⭐⭐ Medium | 3 min | 2023 |
| 5 | EMC concept | ⭐ Easy | 2 min | 2023 |
| 6 | Water removal | ⭐⭐ Medium | 3 min | 2023 |
| 7 | Dryer type selection | ⭐ Easy | 2 min | 2022 |
| 8 | Drying time | ⭐⭐⭐ Hard | 4 min | 2022 |
| 9 | Relative humidity | ⭐⭐ Medium | 3 min | 2022 |
| 10 | Final moisture | ⭐⭐ Medium | 3 min | 2021 |
| 11 | Heat requirement | ⭐⭐⭐ Hard | 4 min | 2021 |
| 12 | Thin layer drying | ⭐⭐ Medium | 3 min | 2021 |
| 13 | Psychrometry basics | ⭐⭐ Medium | 3 min | 2020 |
| 14 | MC determination method | ⭐ Easy | 2 min | 2020 |

**Total: 14 questions, ~40 minutes**

---

## ✅ Solutions

### Q1. Moisture Content wb to db (GATE 2024) ⭐

**Question:**  
Grain has moisture content of 20% (wb). The moisture content on dry basis (%) is:

(A) 16.7  
(B) 20.0  
(C) 25.0  
(D) 30.0

**Solution:**

Formula for wb to db conversion:
$$
M_{db} = \frac{M_{wb}}{100 - M_{wb}} \times 100
$$

Given: Mwb = 20%

$$
M_{db} = \frac{20}{100 - 20} \times 100 = \frac{20}{80} \times 100 = 25\%
$$

**Answer: (C) 25.0%**

**Key:** db is always higher than wb (same water, less base)

---

### Q2. Moisture Content db to wb (GATE 2024) ⭐

**Question:**  
Paddy has 25% moisture on dry basis. Express this on wet basis (%):

(A) 16.7  
(B) 20.0  
(C) 25.0  
(D) 31.25

**Solution:**

Formula for db to wb:
$$
M_{wb} = \frac{M_{db}}{100 + M_{db}} \times 100
$$

Given: Mdb = 25%

$$
M_{wb} = \frac{25}{100 + 25} \times 100 = \frac{25}{125} \times 100 = 20\%
$$

**Answer: (B) 20.0%**

**Note:** This is inverse of Q1 - verify the relationship!

---

### Q3. Safe Storage Moisture (GATE 2024) ⭐

**Question:**  
The safe storage moisture content for wheat (wb%) is:

(A) 8-10  
(B) 12-14  
(C) 16-18  
(D) 20-22

**Solution:**

**Safe storage MC (wb%) for major grains:**

| Grain | Safe MC (wb%) |
|-------|---------------|
| **Wheat** | **12-14%** ✓ |
| Paddy | 12-14% |
| Rice | 12-13% |
| Maize | 13-15% |
| Pulses | 10-12% |
| Oilseeds | 7-9% |

**Answer: (B) 12-14%**

**Memory:** "12-14 for wheat indeed!"

---

### Q4. Drying Rate (GATE 2023) ⭐⭐

**Question:**  
For thin-layer drying, if drying constant K = 0.5 hr⁻¹, current moisture = 18% db, equilibrium moisture = 10% db, the drying rate (% db per hour) is:

(A) 2.0  
(B) 3.0  
(C) 4.0  
(D) 5.0

**Solution:**

Drying rate equation:
$$
\frac{dM}{dt} = -K(M - M_e)
$$

Given:
- K = 0.5 hr⁻¹
- M = 18% db
- Me = 10% db

Calculate:
$$
\frac{dM}{dt} = -0.5 \times (18 - 10) = -0.5 \times 8 = -4.0\% \text{ db/hr}
$$

Magnitude: **4.0% db/hr**

**Answer: (C) 4.0**

**Note:** Negative sign indicates moisture decrease; question asks magnitude.

---

### Q5. EMC Concept (GATE 2023) ⭐

**Question:**  
Equilibrium Moisture Content (EMC) is the moisture at which:

(A) Grain starts drying  
(B) Drying rate is maximum  
(C) Grain neither gains nor loses moisture  
(D) All water is removed

**Solution:**

**EMC definition:**
- Moisture content where grain is in equilibrium with surrounding air
- No net moisture transfer between grain and air
- Depends on temperature and relative humidity
- Cannot dry below EMC using that air condition

**Answer: (C) Grain neither gains nor loses moisture**

**Concept:** EMC is the lowest MC achievable with given air conditions.

---

### Q6. Water Removal Calculation (GATE 2023) ⭐⭐

**Question:**  
1000 kg of grain at 20% wb MC is dried to 14% wb. The water removed (in kg) is:

(A) 60  
(B) 69  
(C) 71  
(D) 75

**Solution:**

**Method 1: Using dry matter balance**

Initial: 1000 kg at 20% wb
- Water = 1000 × 0.20 = 200 kg
- Dry matter = 1000 - 200 = 800 kg

Final: X kg at 14% wb
- Dry matter remains same = 800 kg
- If 14% is water, then 86% is dry matter
- X × 0.86 = 800
- X = 930.2 kg

Water removed = 1000 - 930.2 = **69.8 kg**

**Answer: (B) 69 kg**

**Formula approach:**
$$
W_{removed} = W_i - W_f = \frac{M_i(M_{i,wb} - M_{f,wb})}{100 - M_{f,wb}}
$$

---

### Q7. Dryer Type Selection (GATE 2022) ⭐

**Question:**  
For large-scale paddy drying, which dryer is most commonly used?

(A) Tray dryer  
(B) LSU dryer  
(C) Fluidized bed dryer  
(D) Vacuum dryer

**Solution:**

**Dryer types by application:**

| Dryer Type | Best For | Capacity |
|------------|----------|----------|
| Tray | Herbs, small batches | Very small |
| **LSU (Louisiana State University)** | **Paddy, large scale** | **Large** ✓ |
| Fluidized bed | Seeds, continuous | Medium-Large |
| Vacuum | Heat-sensitive | Small |
| Rotary | Grains, continuous | Large |

**LSU dryer:**
- Column type
- Continuous flow
- Ideal for paddy
- Widely used in Asia

**Answer: (B) LSU dryer**

---

### Q8. Drying Time Calculation (GATE 2022) ⭐⭐⭐

**Question:**  
Grain drying follows Newton's law: ln[(M-Me)/(M₀-Me)] = -Kt. If K = 0.3 hr⁻¹, initial MC = 25% db, equilibrium MC = 12% db, final MC = 15% db, the drying time (in hours) is:

(A) 3.5  
(B) 4.3  
(C) 5.2  
(D) 6.1

**Solution:**

Newton's drying equation:
$$
\ln\left[\frac{M - M_e}{M_0 - M_e}\right] = -Kt
$$

Given:
- K = 0.3 hr⁻¹
- M₀ = 25% db
- Me = 12% db
- M = 15% db

Rearrange for t:
$$
t = -\frac{1}{K} \times \ln\left[\frac{M - M_e}{M_0 - M_e}\right]
$$

Calculate:
$$
t = -\frac{1}{0.3} \times \ln\left[\frac{15 - 12}{25 - 12}\right]
$$
$$
= -\frac{1}{0.3} \times \ln\left[\frac{3}{13}\right]
$$
$$
= -\frac{1}{0.3} \times \ln[0.231]
$$
$$
= -\frac{1}{0.3} \times (-1.466)
$$
$$
= \frac{1.466}{0.3} = 4.89 \text{ hours}
$$

**Answer: (C) 5.2 hours** (closest)

**Key:** Time increases logarithmically as final MC approaches EMC.

---

### Q9. Relative Humidity (GATE 2022) ⭐⭐

**Question:**  
At 30°C, saturation vapor pressure is 4.24 kPa. If actual vapor pressure is 2.12 kPa, the relative humidity (%) is:

(A) 40  
(B) 50  
(C) 60  
(D) 75

**Solution:**

Relative humidity formula:
$$
RH = \frac{P_{actual}}{P_{sat}} \times 100
$$

Given:
- Pactual = 2.12 kPa
- Psat = 4.24 kPa

Calculate:
$$
RH = \frac{2.12}{4.24} \times 100 = 0.50 \times 100 = 50\%
$$

**Answer: (B) 50%**

**Note:** RH = 50% means air holds half the moisture it could at that temperature.

---

### Q10. Final Moisture After Mixing (GATE 2021) ⭐⭐

**Question:**  
500 kg grain at 18% wb is mixed with 500 kg grain at 14% wb. The final moisture content (wb%) of the mixture is:

(A) 14  
(B) 15  
(C) 16  
(D) 17

**Solution:**

**Water balance method:**

Grain 1:
- Mass = 500 kg
- MC = 18% wb
- Water = 500 × 0.18 = 90 kg

Grain 2:
- Mass = 500 kg
- MC = 14% wb
- Water = 500 × 0.14 = 70 kg

Total:
- Total mass = 500 + 500 = 1000 kg
- Total water = 90 + 70 = 160 kg
- Final MC = (160/1000) × 100 = **16% wb**

**Answer: (C) 16%**

**Quick formula:** For equal masses, MC_final = (MC₁ + MC₂)/2 = (18+14)/2 = 16%

---

### Q11. Heat Requirement for Drying (GATE 2021) ⭐⭐⭐

**Question:**  
To evaporate 100 kg water from grain, with latent heat of vaporization = 2400 kJ/kg, the heat required (in MJ) is:

(A) 180  
(B) 200  
(C) 240  
(D) 280

**Solution:**

Heat for evaporation:
$$
Q = m \times L
$$

Given:
- m = 100 kg water
- L = 2400 kJ/kg

Calculate:
$$
Q = 100 \times 2400 = 240,000 \text{ kJ} = 240 \text{ MJ}
$$

**Answer: (C) 240 MJ**

**Note:** This is sensible heat only; actual drying requires additional sensible heat to warm grain and air.

---

### Q12. Thin Layer Drying Constant (GATE 2021) ⭐⭐

**Question:**  
In thin-layer drying equation MR = exp(-Kt), if after 2 hours MR = 0.6, the drying constant K (hr⁻¹) is approximately:

(A) 0.15  
(B) 0.21  
(C) 0.26  
(D) 0.35

**Solution:**

Given equation:
$$
MR = e^{-Kt}
$$

where MR = Moisture Ratio = (M-Me)/(M₀-Me)

Given:
- MR = 0.6
- t = 2 hours

Take natural log:
$$
\ln(MR) = -Kt
$$
$$
\ln(0.6) = -K \times 2
$$
$$
-0.511 = -2K
$$
$$
K = \frac{0.511}{2} = 0.255 \text{ hr}^{-1}
$$

**Answer: (C) 0.26 hr⁻¹**

**Check:** e^(-0.26×2) = e^(-0.52) = 0.595 ≈ 0.6 ✓

---

### Q13. Psychrometry - Dry Bulb vs Wet Bulb (GATE 2020) ⭐⭐

**Question:**  
In a psychrometric chart, when relative humidity is 100%, the relationship between dry bulb temperature (DBT) and wet bulb temperature (WBT) is:

(A) DBT > WBT  
(B) DBT < WBT  
(C) DBT = WBT  
(D) No fixed relationship

**Solution:**

**Psychrometry concepts:**

- **Dry bulb temperature (DBT):** Actual air temperature
- **Wet bulb temperature (WBT):** Temperature with evaporative cooling
- **Depression:** DBT - WBT

**At different RH:**
- RH = 0% (dry air): Maximum depression, DBT >> WBT
- RH = 50%: Moderate depression, DBT > WBT
- **RH = 100% (saturated):** No evaporation possible, **DBT = WBT** ✓

**Answer: (C) DBT = WBT**

**Rule:** Higher RH → smaller depression → WBT closer to DBT

---

### Q14. MC Determination Method (GATE 2020) ⭐

**Question:**  
The standard method for determining moisture content of grains is:

(A) Karl Fischer method  
(B) Oven drying method  
(C) Infrared method  
(D) Microwave method

**Solution:**

**Moisture determination methods:**

| Method | Accuracy | Speed | Standard? |
|--------|----------|-------|-----------|
| **Oven drying (105°C)** | **High** | Slow (4-24 hr) | **Yes** ✓ |
| Karl Fischer | Very high | Moderate | For oils |
| Moisture meter | Moderate | Fast | Field use |
| Infrared | Moderate | Fast | Quick test |
| Microwave | Moderate | Very fast | Quick test |

**Standard method:** Oven drying at 103-105°C until constant weight

**For grains:**
- Wheat, rice: 130°C, 4 hours (high temp method)
- General: 103°C, 24 hours (low temp method)

**Answer: (B) Oven drying method**

---

## 📊 Topic-wise Summary

| Topic | Questions | Key Formulas |
|-------|-----------|--------------|
| **MC conversion** | 3 (Q1, Q2, Q3) | Mdb = Mwb/(100-Mwb)×100 |
| **Drying rate** | 4 (Q4, Q8, Q12) | dM/dt = -K(M-Me) |
| **Water removal** | 2 (Q6, Q10) | Mass balance |
| **Heat/energy** | 1 (Q11) | Q = mL |
| **Concepts** | 4 (Q5, Q7, Q9, Q13, Q14) | EMC, RH, methods |

---

## 💡 Success Tips

### Must Memorize

1. **MC conversion:** Mdb = Mwb/(100-Mwb)×100
2. **Safe storage:** Wheat/Paddy 12-14% wb
3. **Drying rate:** dM/dt = -K(M-Me)
4. **RH:** Pactual/Psat × 100
5. **At 100% RH:** DBT = WBT

---

*[CheatSheet](./CheatSheet.md) | [Back to Section](../README.md)*
