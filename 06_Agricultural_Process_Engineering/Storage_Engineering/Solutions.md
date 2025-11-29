# 🏪 Storage Engineering - GATE PYQ Solutions

> **8 Previous Year Questions with Detailed Solutions**

---

## ✅ Solutions

### Q1. Janssen's Equation - Vertical Pressure (GATE 2024) ⭐⭐⭐

**Question:**  
In a cylindrical bin with radius 2 m, grain bulk density 800 kg/m³, lateral pressure ratio k = 0.4, wall friction μ = 0.3, depth 10 m. Vertical pressure at bottom using Janssen's equation (in kPa) is approximately:

[Use: Pv = (γR/kμ)[1 - exp(-kμh/R)], g = 10 m/s²]

**Solution:**

**Janssen's equation:**
$$
P_v = \frac{\gamma R}{k\mu} \times \left[1 - e^{-k\mu h/R}\right]
$$

Given:
- R = 2 m (radius)
- ρ = 800 kg/m³
- γ = ρg = 800 × 10 = 8000 N/m³ = 8 kN/m³
- k = 0.4
- μ = 0.3
- h = 10 m

Calculate term by term:

$$
\frac{kμh}{R} = \frac{0.4 \times 0.3 \times 10}{2} = \frac{1.2}{2} = 0.6
$$

$$
e^{-0.6} = 0.549
$$

$$
1 - e^{-0.6} = 1 - 0.549 = 0.451
$$

$$
\frac{\gamma R}{k\mu} = \frac{8 \times 2}{0.4 \times 0.3} = \frac{16}{0.12} = 133.3 \text{ kN/m}^2
$$

$$
P_v = 133.3 \times 0.451 = 60.1 \text{ kN/m}^2 = 60.1 \text{ kPa}
$$

**Answer: ~60 kPa**

**Key:** At large depths, Pv approaches γR/(kμ) asymptotically.

---

### Q2. Lateral Pressure (GATE 2024) ⭐⭐

**Question:**  
If vertical pressure in a bin is 50 kPa and lateral pressure ratio k = 0.4, the lateral pressure (in kPa) is:

(A) 12.5  
(B) 20.0  
(C) 30.0  
(D) 40.0

**Solution:**

**Lateral pressure formula:**
$$
P_h = k \times P_v
$$

Given:
- Pv = 50 kPa
- k = 0.4

$$
P_h = 0.4 \times 50 = 20 \text{ kPa}
$$

**Answer: (B) 20.0 kPa**

**Note:** k typically ranges 0.3-0.6 for grains.

---

### Q3. Bulk Density (GATE 2023) ⭐

**Question:**  
The typical bulk density of wheat (in kg/m³) is:

(A) 550-600  
(B) 750-800  
(C) 900-950  
(D) 1000-1050

**Solution:**

**Bulk densities (kg/m³):**

| Grain | Bulk Density |
|-------|--------------|
| Paddy | 550-600 |
| **Wheat** | **750-800** ✓ |
| Maize | 700-750 |
| Rice (milled) | 800-850 |
| Pulses | 750-850 |

**Answer: (B) 750-800 kg/m³**

---

### Q4. Angle of Repose (GATE 2023) ⭐

**Question:**  
The angle of repose for paddy is approximately:

(A) 15-20°  
(B) 25-30°  
(C) 30-35°  
(D) 40-45°

**Solution:**

**Angle of repose (°):**

| Material | Angle |
|----------|-------|
| Wheat | 25-30 |
| **Paddy** | **30-35** ✓ |
| Maize | 25-30 |
| Rice | 30-35 |
| Pulses | 30-35 |

**Answer: (C) 30-35°**

**Note:** Higher angle = less flowability

---

### Q5. Aeration Rate (GATE 2022) ⭐⭐

**Question:**  
Recommended aeration rate for grain storage (in m³/min per tonne) is:

(A) 0.01-0.02  
(B) 0.1-0.2  
(C) 1-2  
(D) 10-20

**Solution:**

**Aeration guidelines:**

| Purpose | Rate (m³/min/tonne) |
|---------|---------------------|
| **Cooling/maintenance** | **0.01-0.02** ✓ |
| Drying (supplement) | 0.1-0.5 |
| Emergency cooling | 0.05-0.1 |

**Standard aeration:** 0.01-0.02 m³/min/t = 10-20 m³/hr/t

**Answer: (A) 0.01-0.02 m³/min/tonne**

---

### Q6. Storage Loss (GATE 2022) ⭐

**Question:**  
Major cause of grain storage loss in India is:

(A) Mechanical damage  
(B) Insects and pests  
(C) Rodents  
(D) Birds

**Solution:**

**Storage loss causes (India):**

| Cause | Loss % | Priority |
|-------|--------|----------|
| **Insects/pests** | **5-10%** | **Highest** ✓ |
| Rodents | 2-5% | High |
| Moisture/mold | 3-5% | High |
| Birds | 1-2% | Medium |
| Mechanical | <1% | Low |

**Major pests:** Rice weevil, red flour beetle, khapra beetle

**Answer: (B) Insects and pests**

---

### Q7. CAP/CAS Storage (GATE 2021) ⭐⭐

**Question:**  
In controlled atmosphere storage, which gas composition is typically used?

(A) High O₂, Low CO₂  
(B) High O₂, High CO₂  
(C) Low O₂, High CO₂  
(D) Low O₂, Low CO₂

**Solution:**

**Controlled Atmosphere Storage (CAS):**

**Modified atmosphere:**
- **O₂: Reduced to 2-5%** (from 21% normal)
- **CO₂: Increased to 10-20%** (from 0.03% normal)
- **N₂: Balance**

**Purpose:**
- Inhibit respiration
- Control insects
- Reduce spoilage

**Answer: (C) Low O₂, High CO₂**

**Benefits:** Extended shelf life, reduced pesticide use

---

### Q8. Hopper Flow (GATE 2020) ⭐

**Question:**  
In a mass flow hopper, material flows in:

(A) Central core only  
(B) Along walls only  
(C) Entire cross-section  
(D) Random pattern

**Solution:**

**Hopper flow patterns:**

**1. Mass flow:**
- **Entire material moves uniformly**
- First-in-first-out (FIFO)
- Steep hopper angle (>50°)
- Smooth walls
- Best for quality control

**2. Funnel flow:**
- Central channel flows first
- Material remains at walls
- Less steep angle
- Irregular discharge

**Answer: (C) Entire cross-section**

**Design:** Mass flow preferred for grains to prevent segregation.

---

## 📊 Summary

### Critical Formulas

1. **Janssen's:** Pv = (γR/kμ)[1 - exp(-kμh/R)]
2. **Lateral:** Ph = k × Pv
3. **Typical k:** 0.3-0.6

### Must Remember Values

- **Bulk density:** Wheat 750-800, Paddy 550-600 kg/m³
- **Angle of repose:** Wheat 25-30°, Paddy 30-35°
- **Aeration rate:** 0.01-0.02 m³/min/tonne
- **CAS:** Low O₂ (2-5%), High CO₂ (10-20%)
- **Safe storage MC:** 12-14% wb

---

*[CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
