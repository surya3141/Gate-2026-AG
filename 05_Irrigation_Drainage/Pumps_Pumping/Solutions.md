# ⚙️ Pumps & Pumping - GATE PYQ Solutions

> **10 Previous Year Questions with Detailed Solutions**

---

## 📚 Question Index

| Q# | Topic | Difficulty | Time | Year |
|----|-------|------------|------|------|
| 1 | Total head | ⭐⭐ Medium | 3 min | 2024 |
| 2 | Pump power | ⭐⭐ Medium | 3 min | 2024 |
| 3 | Specific speed | ⭐⭐ Medium | 4 min | 2023 |
| 4 | Pump efficiency | ⭐ Easy | 2 min | 2023 |
| 5 | NPSH | ⭐⭐⭐ Hard | 4 min | 2022 |
| 6 | Pump selection | ⭐ Easy | 2 min | 2022 |
| 7 | Friction head loss | ⭐⭐ Medium | 3 min | 2021 |
| 8 | Brake power | ⭐⭐ Medium | 3 min | 2021 |
| 9 | Water power | ⭐ Easy | 2 min | 2020 |
| 10 | Affinity laws | ⭐⭐ Medium | 3 min | 2020 |

**Total: 10 questions, ~30 minutes**

---

## ✅ Solutions

### Q1. Total Dynamic Head (GATE 2024) ⭐⭐

**Question:**  
Water is to be pumped from a well with water level 8 m below ground to a tank 25 m above ground. If friction losses are 3 m, the total dynamic head (in m) is:

(A) 30  
(B) 33  
(C) 36  
(D) 41

**Solution:**

**Total Dynamic Head (TDH):**
$$
H = H_s + H_d + H_f
$$

Given:
- Static suction head (Hs) = 8 m (below ground)
- Static delivery head (Hd) = 25 m (above ground)
- Friction head (Hf) = 3 m

Calculate:
$$
TDH = 8 + 25 + 3 = 36 \text{ m}
$$

**Answer: (C) 36 m**

**Concept:** TDH = Total lift + All losses

---

### Q2. Pump Power (GATE 2024) ⭐⭐

**Question:**  
A pump delivers 30 L/s water against a head of 20 m with overall efficiency of 70%. The input power required (in kW) is approximately:

(A) 8.4  
(B) 10.0  
(C) 12.0  
(D) 14.2

**Solution:**

**Water power:**
$$
WP = \frac{\gamma \times Q \times H}{1000}
$$

where γ = 9.81 kN/m³

$$
WP = \frac{9.81 \times 0.030 \times 20}{1} = 5.886 \text{ kW}
$$

**Brake power (input):**
$$
BP = \frac{WP}{\eta} = \frac{5.886}{0.70} = 8.41 \text{ kW}
$$

**Answer: (A) 8.4 kW**

**Formula:** BP = (γQH)/(1000η) with γ=9.81, Q in m³/s, H in m

---

### Q3. Specific Speed (GATE 2023) ⭐⭐

**Question:**  
A centrifugal pump runs at 1450 rpm, delivers 50 L/s against 30 m head. The specific speed (dimensionless) is approximately:

(A) 15  
(B) 25  
(C) 35  
(D) 45

**Solution:**

**Specific speed formula:**
$$
N_s = \frac{N \times \sqrt{Q}}{H^{0.75}}
$$

Given:
- N = 1450 rpm
- Q = 50 L/s = 0.050 m³/s
- H = 30 m

Calculate:
$$
N_s = \frac{1450 \times \sqrt{0.050}}{30^{0.75}}
$$
$$
= \frac{1450 \times 0.2236}{13.39}
$$
$$
= \frac{324.2}{13.39} = 24.2
$$

**Answer: (B) 25**

**Interpretation:**
- Ns < 20: Centrifugal (radial flow)
- Ns = 20-40: Mixed flow
- Ns = 40-80: Axial flow

---

### Q4. Pump Efficiency (GATE 2023) ⭐

**Question:**  
If water power is 5 kW and brake power is 7 kW, the overall pump efficiency (%) is:

(A) 58  
(B) 67  
(C) 71  
(D) 83

**Solution:**

**Overall efficiency:**
$$
\eta = \frac{WP}{BP} \times 100
$$

Given:
- WP = 5 kW
- BP = 7 kW

Calculate:
$$
\eta = \frac{5}{7} \times 100 = 71.4\%
$$

**Answer: (C) 71%**

**Typical pump efficiencies:**
- Small pumps: 50-65%
- Medium: 65-75%
- Large: 75-85%

---

### Q5. NPSH (GATE 2022) ⭐⭐⭐

**Question:**  
A centrifugal pump is installed 3 m above water source. Atmospheric pressure = 10.3 m water, vapor pressure = 0.3 m water, friction loss in suction = 0.5 m. The NPSH available (in m) is:

(A) 6.5  
(B) 7.0  
(C) 7.5  
(D) 8.0

**Solution:**

**NPSH Available:**
$$
NPSH_a = H_{atm} - H_s - H_{vp} - H_{fs}
$$

Given:
- Hatm = 10.3 m (atmospheric)
- Hs = 3.0 m (static suction)
- Hvp = 0.3 m (vapor pressure)
- Hfs = 0.5 m (friction in suction)

Calculate:
$$
NPSH_a = 10.3 - 3.0 - 0.3 - 0.5
$$
$$
= 6.5 \text{ m}
$$

**Answer: (A) 6.5 m**

**Safety:** NPSHa should be > NPSHr (required) to avoid cavitation.

---

### Q6. Pump Selection (GATE 2022) ⭐

**Question:**  
For deep tube wells (>100 m), the most suitable pump type is:

(A) Centrifugal  
(B) Submersible  
(C) Reciprocating  
(D) Jet pump

**Solution:**

**Pump selection by depth:**

| Depth | Best Pump | Reason |
|-------|-----------|--------|
| <7 m | Centrifugal | Surface installation |
| 7-15 m | Jet pump | Venturi effect |
| 15-100 m | Turbine | Multi-stage |
| **>100 m** | **Submersible** | **Motor underwater** ✓ |

**Deep tube wells:** Submersible pumps
- Motor and pump together underwater
- No suction lift limitation
- Can pump from great depths

**Answer: (B) Submersible**

---

### Q7. Friction Head Loss (GATE 2021) ⭐⭐

**Question:**  
For a pipe length 200 m, diameter 150 mm, velocity 2 m/s, friction factor f = 0.02, the friction head loss (in m) using Darcy-Weisbach equation is:

[Use: hf = (fLV²)/(2gD)]

(A) 2.72  
(B) 3.26  
(C) 4.08  
(D) 5.44

**Solution:**

**Darcy-Weisbach equation:**
$$
h_f = \frac{f \times L \times V^2}{2 \times g \times D}
$$

Given:
- f = 0.02
- L = 200 m
- V = 2 m/s
- D = 0.15 m
- g = 9.81 m/s²

Calculate:
$$
h_f = \frac{0.02 \times 200 \times 2^2}{2 \times 9.81 \times 0.15}
$$
$$
= \frac{0.02 \times 200 \times 4}{2.943}
$$
$$
= \frac{16}{2.943} = 5.44 \text{ m}
$$

**Answer: (D) 5.44 m**

**Note:** Friction losses increase with length and velocity², decrease with diameter.

---

### Q8. Brake Power vs Water Power (GATE 2021) ⭐⭐

**Question:**  
A pump lifts 20 L/s water through 15 m height. If pump efficiency is 65%, the brake power (in kW) is:

(A) 2.21  
(B) 2.94  
(C) 3.52  
(D) 4.52

**Solution:**

**Water power:**
$$
WP = \frac{\gamma \times Q \times H}{1000}
$$

$$
= \frac{9.81 \times 0.020 \times 15}{1} = 2.943 \text{ kW}
$$

**Brake power:**
$$
BP = \frac{WP}{\eta} = \frac{2.943}{0.65} = 4.53 \text{ kW}
$$

**Answer: (D) 4.52 kW**

**Remember:** BP > WP (losses occur, efficiency < 100%)

---

### Q9. Water Power (GATE 2020) ⭐

**Question:**  
The unit of water power in SI system is:

(A) Watt  
(B) Joule  
(C) Newton  
(D) Pascal

**Solution:**

**Water power = Rate of energy transfer**

$$
Power = \frac{Energy}{Time} = \frac{Joule}{Second} = Watt
$$

**Dimensional analysis:**
$$
WP = \gamma \times Q \times H
$$
$$
= \frac{Force}{Volume} \times \frac{Volume}{Time} \times Length
$$
$$
= \frac{Force \times Length}{Time} = \frac{Energy}{Time} = Power
$$

**SI unit of power: Watt (W) or kiloWatt (kW)**

**Answer: (A) Watt**

**Common units:**
- 1 kW = 1000 W
- 1 HP (horsepower) = 0.746 kW = 746 W

---

### Q10. Affinity Laws (GATE 2020) ⭐⭐

**Question:**  
A pump delivers 40 L/s at 1450 rpm. If speed is increased to 1750 rpm, the new discharge (in L/s) according to affinity laws is approximately:

(A) 44  
(B) 48  
(C) 52  
(D) 56

**Solution:**

**Affinity Law for discharge:**
$$
\frac{Q_2}{Q_1} = \frac{N_2}{N_1}
$$

Given:
- Q₁ = 40 L/s
- N₁ = 1450 rpm
- N₂ = 1750 rpm

Calculate:
$$
Q_2 = Q_1 \times \frac{N_2}{N_1}
$$
$$
= 40 \times \frac{1750}{1450}
$$
$$
= 40 \times 1.207 = 48.3 \text{ L/s}
$$

**Answer: (B) 48 L/s**

**Affinity Laws:**
- Q ∝ N (discharge proportional to speed)
- H ∝ N² (head proportional to speed²)
- P ∝ N³ (power proportional to speed³)

---

## 📊 Topic-wise Summary

| Topic | Questions | Key Formulas |
|-------|-----------|--------------|
| **Head calculations** | 3 (Q1, Q5, Q7) | TDH = Hs+Hd+Hf, NPSHa |
| **Power** | 4 (Q2, Q4, Q8, Q9) | BP = γQH/(1000η) |
| **Specific speed** | 1 (Q3) | Ns = N√Q/H^0.75 |
| **Pump selection** | 1 (Q6) | By depth/application |
| **Affinity laws** | 1 (Q10) | Q∝N, H∝N², P∝N³ |

---

## 💡 Success Tips

### Must Remember

1. **Total head:** TDH = Static lift + Friction
2. **Power:** BP = γQH/(1000η), γ=9.81
3. **Efficiency:** η = WP/BP
4. **Specific speed:** Ns = N√Q/H^0.75
5. **Affinity:** Q∝N, H∝N², P∝N³

---

*[Theory](./README.md) | [CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
