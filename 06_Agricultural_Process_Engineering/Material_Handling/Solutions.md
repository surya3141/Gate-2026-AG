# 🚜 Material Handling - GATE PYQ Solutions

> **6 Previous Year Questions with Detailed Solutions**

---

## ✅ Solutions

### Q1. Belt Conveyor Capacity (GATE 2024) ⭐⭐

**Question:**  
A belt conveyor has cross-sectional area 0.02 m², belt speed 1.5 m/s, and material bulk density 800 kg/m³. The capacity (in tonnes/hour) is:

(A) 72  
(B) 86  
(C) 108  
(D) 144

**Solution:**

**Conveyor capacity formula:**
$$
Q = 3.6 \times A \times v \times \rho
$$

where:
- Q = Capacity (t/hr)
- A = Cross-sectional area (m²)
- v = Belt velocity (m/s)
- ρ = Bulk density (t/m³)

Given:
- A = 0.02 m²
- v = 1.5 m/s
- ρ = 800 kg/m³ = 0.8 t/m³

$$
Q = 3.6 \times 0.02 \times 1.5 \times 0.8
$$
$$
= 3.6 \times 0.024 = 0.0864 \times 1000 = 86.4 \text{ t/hr}
$$

**Answer: (B) 86 t/hr**

**Note:** Factor 3.6 converts m³/s to m³/hr

---

### Q2. Screw Conveyor (GATE 2023) ⭐⭐

**Question:**  
A screw conveyor has pitch 200 mm, diameter 150 mm, speed 60 rpm, and loading efficiency 40%. The capacity (in m³/hr) is approximately:

[Use: Q = (π/4) × D² × p × N × η × (1/1000)]

**Solution:**

**Screw conveyor capacity:**
$$
Q = \frac{\pi}{4} \times D^2 \times p \times N \times \eta \times \frac{60}{1000}
$$

Given:
- D = 150 mm = 0.15 m
- p = 200 mm = 0.2 m
- N = 60 rpm
- η = 0.40

$$
Q = \frac{3.14}{4} \times (0.15)^2 \times 0.2 \times 60 \times 0.40
$$
$$
= 0.785 \times 0.0225 \times 0.2 \times 60 \times 0.40
$$
$$
= 0.785 \times 0.108 = 0.0848 \text{ m}^3/\text{min} = 5.09 \text{ m}^3/\text{hr}
$$

**Answer: ~5 m³/hr**

---

### Q3. Bucket Elevator (GATE 2023) ⭐

**Question:**  
Bucket elevators are most suitable for:

(A) Horizontal transport  
(B) Inclined transport (< 45°)  
(C) Vertical transport  
(D) Any angle transport

**Solution:**

**Material handling equipment by orientation:**

| Equipment | Best Orientation | Typical Use |
|-----------|------------------|-------------|
| Belt conveyor | Horizontal, slight incline | General |
| Screw conveyor | Horizontal, slight incline | Enclosed |
| **Bucket elevator** | **Vertical** | **Lifting** ✓ |
| Pneumatic | Any angle | Long distance |
| Chain conveyor | Any angle | Heavy loads |

**Bucket elevator:**
- Buckets attached to belt/chain
- Lifts material vertically
- Efficient for height gain
- Common in grain elevators

**Answer: (C) Vertical transport**

---

### Q4. Pneumatic Conveying (GATE 2022) ⭐⭐

**Question:**  
In dilute phase pneumatic conveying, the typical air velocity (in m/s) is:

(A) 5-10  
(B) 15-30  
(C) 40-50  
(D) 60-80

**Solution:**

**Pneumatic conveying phases:**

| Phase | Solid:Air Ratio | Air Velocity (m/s) |
|-------|----------------|-------------------|
| **Dilute phase** | Low (<15) | **15-30** ✓ |
| Dense phase | High (>15) | 3-10 |

**Dilute phase characteristics:**
- High air velocity
- Particles suspended
- Lower material concentration
- Long distance capability

**Minimum velocity:** Must exceed saltation velocity (~12-15 m/s)

**Answer: (B) 15-30 m/s**

---

### Q5. Belt Conveyor Power (GATE 2021) ⭐⭐

**Question:**  
Power required for a belt conveyor carrying 100 t/hr material over 50 m horizontal distance with friction coefficient 0.03 is (in kW):

[Use: P = (Q × L × f × g)/3600, g = 10 m/s²]

**Solution:**

**Horizontal belt power:**
$$
P = \frac{Q \times L \times f \times g}{3600}
$$

Given:
- Q = 100 t/hr = 100,000 kg/hr
- L = 50 m
- f = 0.03
- g = 10 m/s²

$$
P = \frac{100000 \times 50 \times 0.03 \times 10}{3600}
$$
$$
= \frac{1,500,000}{3600} = 416.7 \text{ W} = 0.417 \text{ kW}
$$

**Answer: ~0.42 kW**

**Note:** For inclined conveyor, add component for lifting: ΔH × Q × g/3600

---

### Q6. Angle of Surcharge (GATE 2020) ⭐

**Question:**  
The angle of surcharge for a belt conveyor is typically:

(A) Equal to angle of repose  
(B) 5-10° less than angle of repose  
(C) 5-10° more than angle of repose  
(D) Half the angle of repose

**Solution:**

**Belt conveyor material profile:**

- **Angle of repose (θr):** Static pile angle
- **Angle of surcharge (θs):** Dynamic angle on moving belt

**Relationship:**
$$
\theta_s = \theta_r - (5° \text{ to } 10°)
$$

**Reason:** Material settles less on moving belt due to vibration and motion.

**Example:**
- Wheat: θr = 28°, θs ≈ 20°
- Paddy: θr = 32°, θs ≈ 24°

**Answer: (B) 5-10° less than angle of repose**

---

## 📊 Summary

### Critical Formulas

1. **Belt capacity:** Q = 3.6 × A × v × ρ (t/hr)
2. **Screw capacity:** Q = (π/4) × D² × p × N × η
3. **Belt power:** P = Q × L × f × g / 3600

### Equipment Selection

| Distance | Orientation | Best Choice |
|----------|-------------|-------------|
| Short | Horizontal | Screw conveyor |
| Long | Horizontal | Belt conveyor |
| Any | Vertical | Bucket elevator |
| Long | Any angle | Pneumatic |

### Must Remember

- **Dilute phase velocity:** 15-30 m/s
- **Angle of surcharge:** 5-10° less than repose
- **Belt conveyor:** Most common, versatile
- **Screw conveyor:** Enclosed, 40% efficiency
- **Bucket elevator:** Vertical lifting

---

*[CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
