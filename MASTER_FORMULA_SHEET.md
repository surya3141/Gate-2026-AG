# 📐 GATE AG 2026 - Master Formula Sheet

> **Complete Formula Reference - All Sections - Print Ready**

---

## 📋 Table of Contents
1. [Engineering Mathematics](#engineering-mathematics)
2. [Farm Machinery](#farm-machinery)
3. [Farm Power](#farm-power)
4. [Soil & Water Conservation](#soil-water-conservation)
5. [Irrigation & Drainage](#irrigation-drainage)
6. [Agricultural Process Engineering](#agricultural-process-engineering)
7. [Dairy & Food Engineering](#dairy-food-engineering)
8. [General Aptitude](#general-aptitude)

---

# 1️⃣ Engineering Mathematics

## Calculus

**Derivatives:**
$$
\frac{d}{dx}(x^n) = nx^{n-1}
$$
$$
\frac{d}{dx}(e^x) = e^x, \quad \frac{d}{dx}(\ln x) = \frac{1}{x}
$$
$$
\frac{d}{dx}(\sin x) = \cos x, \quad \frac{d}{dx}(\cos x) = -\sin x
$$

**Integration:**
$$
\int x^n dx = \frac{x^{n+1}}{n+1} + C
$$
$$
\int e^x dx = e^x + C, \quad \int \frac{1}{x} dx = \ln|x| + C
$$

**Definite Integration:**
$$
\int_a^b f(x)dx = F(b) - F(a)
$$

**Maxima/Minima:**
- First derivative = 0 for critical points
- Second derivative: f''(x) > 0 → minimum, f''(x) < 0 → maximum

## Differential Equations

**First Order Linear:**
$$
\frac{dy}{dx} + P(x)y = Q(x)
$$
$$
\text{IF} = e^{\int P(x)dx}, \quad y \cdot \text{IF} = \int Q(x) \cdot \text{IF} \, dx
$$

**Second Order Linear:**
$$
\frac{d^2y}{dx^2} + p\frac{dy}{dx} + qy = 0
$$
Auxiliary equation: $m^2 + pm + q = 0$

## Linear Algebra

**Matrix Operations:**
$$
\det(A) = ad - bc \quad \text{for } \begin{bmatrix} a & b \\ c & d \end{bmatrix}
$$
$$
A^{-1} = \frac{1}{\det(A)} \text{adj}(A)
$$

**Eigenvalues:**
$$
\det(A - \lambda I) = 0
$$

## Probability & Statistics

**Probability:**
$$
P(A \cup B) = P(A) + P(B) - P(A \cap B)
$$
$$
P(A|B) = \frac{P(A \cap B)}{P(B)}
$$

**Mean & Variance:**
$$
\mu = \frac{\sum x_i}{n}, \quad \sigma^2 = \frac{\sum (x_i - \mu)^2}{n}
$$

**Standard Deviation:**
$$
\sigma = \sqrt{\frac{\sum (x_i - \mu)^2}{n}}
$$

---

# 2️⃣ Farm Machinery

## Tillage

**Draft Force:**
$$
D = f \times W \times d \times w \times v
$$
- f = specific draft (N/cm²)
- W = weight on tool
- d = depth, w = width, v = speed

**Specific Draft:**
$$
\text{Specific draft} = \frac{\text{Total draft}}{\text{Cross-sectional area}}
$$

**Power Required:**
$$
P = \frac{D \times v}{1000} \text{ kW}
$$

## Seed Drill

**Seed Rate:**
$$
Q = \frac{A \times L \times N \times \pi D}{8}
$$
- A = seed rate (kg/ha)
- L = length of plot
- N = no. of furrow openers
- D = drive wheel diameter

**Seed Spacing:**
$$
s = \frac{60 \times v}{n}
$$
- v = forward speed (m/s)
- n = seed drops per minute

## Sprayer

**Discharge Rate:**
$$
Q = 600 \times s \times w \times a
$$
- s = speed (km/h)
- w = swath width (m)
- a = application rate (L/ha)

**Nozzle Flow:**
$$
Q = K \sqrt{P}
$$
- K = nozzle constant
- P = pressure

## Harvesting

**Threshing Efficiency:**
$$
\eta_t = \frac{\text{Grain output}}{\text{Grain input}} \times 100
$$

**Cleaning Efficiency:**
$$
\eta_c = \frac{\text{Clean grain}}{\text{Total grain output}} \times 100
$$

**Field Capacity:**
$$
\text{TFC} = \frac{w \times s}{10}, \quad \text{EFC} = \text{TFC} \times \text{FE}
$$
- TFC in ha/h, w = width (m), s = speed (km/h)

**Field Efficiency:**
$$
\text{FE} = \frac{\text{EFC}}{\text{TFC}} \times 100
$$

---

# 3️⃣ Farm Power

## Engine Performance

**Brake Power:**
$$
BP = \frac{2\pi NT}{60,000} \text{ kW}
$$
- N = RPM, T = torque (Nm)

**Indicated Power:**
$$
IP = \frac{P_{mean} \times L \times A \times N \times n}{60,000}
$$

**Mechanical Efficiency:**
$$
\eta_m = \frac{BP}{IP} \times 100
$$

**Thermal Efficiency:**
$$
\eta_{th} = \frac{\text{Work output}}{\text{Heat input}} \times 100 = \frac{BP}{m_f \times CV} \times 100
$$

**Brake Specific Fuel Consumption:**
$$
BSFC = \frac{m_f}{BP} \text{ kg/kWh}
$$

## Traction

**Tractive Efficiency:**
$$
\eta_t = \frac{\text{Drawbar power}}{\text{Axle power}} \times 100
$$

**Slip:**
$$
s = \frac{v_t - v_a}{v_t} \times 100
$$
- vₜ = theoretical speed, vₐ = actual speed

**Weight Transfer:**
$$
W_f = W \times \frac{b - h\mu}{L}
$$
$$
W_r = W \times \frac{a + h\mu}{L}
$$

**Rolling Resistance:**
$$
R_r = C_r \times W
$$
- Cᵣ = coefficient (0.04-0.08 for firm soil)

---

# 4️⃣ Soil & Water Conservation

## Soil Erosion

**Universal Soil Loss Equation (USLE):**
$$
A = R \times K \times LS \times C \times P
$$
- A = soil loss (t/ha/yr)
- R = rainfall erosivity
- K = soil erodibility
- LS = slope length-steepness
- C = crop management
- P = conservation practice

**Revised USLE (RUSLE):**
Same formula, updated factor values

## Water Erosion

**Runoff:**
$$
Q = \frac{(P - I_a)^2}{P - I_a + S}
$$
- P = rainfall, Iₐ = initial abstraction, S = potential retention

**Rational Method:**
$$
Q = \frac{C \times i \times A}{360}
$$
- Q = runoff (m³/s), C = coefficient, i = intensity (mm/h), A = area (ha)

## Contour Bunding

**Vertical Interval:**
$$
VI = \frac{XY}{100}
$$
- X = constant (0.3-0.6), Y = % slope

**Horizontal Interval:**
$$
HI = \frac{VI}{\text{Slope (fraction)}}
$$

## Terracing

**Channel Spacing:**
$$
S = \frac{XY + Z}{100}
$$
- Z = constant for rainfall zone

---

# 5️⃣ Irrigation & Drainage

## Irrigation Water Requirement

**Consumptive Use (ETc):**
$$
ET_c = K_c \times ET_0
$$
- Kc = crop coefficient, ET₀ = reference ET

**Net Irrigation Requirement:**
$$
NIR = ET_c - P_e
$$
- Pₑ = effective rainfall

**Gross Irrigation Requirement:**
$$
GIR = \frac{NIR}{\eta_{app}}
$$

**Irrigation Efficiency:**
$$
\eta = \frac{\text{Water stored in root zone}}{\text{Water applied}} \times 100
$$

## Canal Design

**Manning's Equation:**
$$
V = \frac{1}{n} R^{2/3} S^{1/2}
$$
- n = Manning's roughness, R = hydraulic radius, S = slope

**Discharge:**
$$
Q = A \times V
$$

**Hydraulic Radius:**
$$
R = \frac{A}{P}
$$
- A = area, P = wetted perimeter

**Lacey's Regime:**
$$
V = 0.55 \times m \times R^{1/2}
$$
$$
P = 4.75 \sqrt{Q}
$$

## Sprinkler Irrigation

**Discharge:**
$$
q = \frac{A \times d}{T \times S_l \times S_s}
$$
- A = area, d = depth, T = time, Sl × Ss = spacing

**Application Rate:**
$$
i = \frac{q}{S_l \times S_s} \text{ mm/h}
$$

## Drip Irrigation

**Emitter Discharge:**
$$
q = K \times H^x
$$
- K = constant, H = pressure head, x = exponent (0.5 for turbulent)

**Irrigation Time:**
$$
T = \frac{A \times d \times S_p \times S_l}{q \times n \times 60}
$$
- n = no. of emitters per plant

---

# 6️⃣ Agricultural Process Engineering

## Grain Drying

**Moisture Content (wet basis):**
$$
M_{wb} = \frac{W_{water}}{W_{wet}} \times 100
$$

**Moisture Content (dry basis):**
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

**Drying Rate:**
$$
\frac{dM}{dt} = -K(M - M_e)
$$
- K = drying constant, Mₑ = equilibrium MC

**Heat Required:**
$$
Q = m \times L
$$
- m = water evaporated (kg), L = latent heat (~2450 kJ/kg)

## Size Reduction

**Kick's Law (Coarse grinding):**
$$
E = K_k \times \log \frac{D_i}{D_f}
$$

**Rittinger's Law (Fine grinding):**
$$
E = K_r \times \left(\frac{1}{D_f} - \frac{1}{D_i}\right)
$$

**Bond's Law (General):**
$$
E = E_i \times \left(\frac{1}{\sqrt{D_f}} - \frac{1}{\sqrt{D_i}}\right)
$$

**Reduction Ratio:**
$$
RR = \frac{D_i}{D_f}
$$

## Storage Engineering

**Janssen's Equation (Pressure):**
$$
P_v = \frac{\gamma R}{k\mu} \left[1 - \exp\left(-\frac{k\mu h}{R}\right)\right]
$$
$$
P_h = k \times P_v
$$
- γ = bulk density, R = hydraulic radius, k = lateral pressure ratio, μ = friction coefficient

**Bulk Density:**
- Paddy: 550-600 kg/m³
- Wheat: 750-800 kg/m³
- Maize: 700-750 kg/m³

**Aeration Rate:**
$$
Q = 0.01 - 0.02 \text{ m}^3/(\text{min·t})
$$

## Material Handling

**Belt Conveyor Capacity:**
$$
Q = 3.6 \times A \times v \times \rho \times \eta
$$
- Factor 3.6 critical for unit conversion

**Screw Conveyor Capacity:**
$$
Q = \frac{\pi}{4} \times D^2 \times p \times N \times \eta
$$
- η = 0.30-0.40

**Pneumatic Conveying:**
- Dilute phase: 15-30 m/s
- Dense phase: 3-8 m/s

---

# 7️⃣ Dairy & Food Engineering

## Milk Processing

**Milk Composition:**
$$
\text{Total Solids (TS)} = \text{Fat} + \text{SNF}
$$
$$
\text{SNF} = \text{TS} - \text{Fat}
$$

**Standard Values:**
- Fat: 3.5%, SNF: 8.5%, TS: 12%
- Density: 1.028-1.032 kg/L at 15°C
- pH: 6.6-6.8

**Stokes' Law (Cream Separation):**
$$
v = \frac{2gr^2(\rho_m - \rho_f)}{9\mu}
$$
- v ∝ g (velocity proportional to acceleration)

**Centrifugal Force:**
$$
F \propto N^2
$$
- Double speed → 4× force

**Pearson's Square (Standardization):**
```
      Higher (H)        Target-Lower
          ╲           ╱
           ╲         ╱
            Target
           ╱         ╲
          ╱           ╲
      Lower (L)      Higher-Target
```

## Thermal Processing

**D-value (90% reduction time):**
$$
t = n \times D
$$
- n = log reductions

**F-value (Process lethality):**
$$
F = D \times (\log N_0 - \log N) = D \times n
$$

**z-value (Temperature coefficient):**
$$
\log \left(\frac{D_1}{D_2}\right) = \frac{T_2 - T_1}{z}
$$
- z = 10°C for bacterial spores

**Lethal Rate:**
$$
L = 10^{\frac{T-121}{z}}
$$

**Pasteurization Standards:**
- LTLT: 63°C × 30 min
- HTST: 72°C × 15 sec
- UHT: 135-150°C × 2-4 sec

## Food Preservation

**Water Activity:**
$$
a_w = \frac{P}{P_0} = \frac{ERH}{100}
$$
- Safe storage: aw < 0.6

**Moisture Content Conversions:** (Same as drying)

**Freezing Heat:**
$$
Q = m \times (c_1 \Delta T_1 + L_f + c_2 \Delta T_2)
$$
- Lf ≈ 335 kJ/kg for water

## Food Quality

**pH:**
$$
pH = -\log[H^+]
$$

**Titratable Acidity (Milk):**
$$
\text{Acidity (\%)} = \frac{V \times N \times 0.009}{W} \times 100
$$
- 0.009 = equivalent of lactic acid

**Kjeldahl Protein:**
$$
\text{Protein (\%)} = N(\%) \times \text{Factor}
$$
- Milk: Factor = 6.38
- General: Factor = 6.25

---

# 8️⃣ General Aptitude

## Quantitative Formulas

**Percentage:**
$$
\text{Net change} = -\frac{x^2}{100} \text{ (for x% up then x% down)}
$$

**Time-Work:**
$$
\frac{1}{A} + \frac{1}{B} = \frac{1}{T}
$$

**Speed-Distance:**
$$
\text{Average speed (equal distance)} = \frac{2xy}{x+y}
$$

**Simple Interest:**
$$
SI = \frac{P \times R \times T}{100}
$$
- If doubles in T years: R = 100/T

**Compound Interest:**
$$
A = P\left(1 + \frac{R}{100}\right)^T
$$

**Profit-Loss:**
$$
\text{Profit\%} = \frac{\text{Profit}}{CP} \times 100
$$

**Geometry:**
- Triangle: $A = \frac{1}{2} bh$ or $A = \sqrt{s(s-a)(s-b)(s-c)}$
- Circle: $A = \pi r^2$, $C = 2\pi r$
- Sphere: $V = \frac{4}{3}\pi r^3$

**Series:**
- AP: $S_n = \frac{n}{2}[2a + (n-1)d]$
- GP: $S_n = \frac{a(r^n - 1)}{r - 1}$

**Number System:**
$$
\text{LCM} \times \text{HCF} = \text{Product of numbers}
$$

## Verbal Essentials

**Grammar Rules:**
- Each/Every/Either/Neither → Singular verb
- The number IS / A number ARE
- By [future time] → will have V3 (future perfect)

**Common Prepositions:**
- Addicted TO, Good AT, Interested IN, Different FROM

---

## 🎯 Critical Values Quick Reference

| Section | Key Values |
|---------|------------|
| **Drying** | Safe MC: 12-14%, EMC concept |
| **Storage** | Wheat 750-800 kg/m³, Aeration 0.01-0.02 |
| **Milk** | Fat 3.5%, SNF 8.5%, pH 6.6-6.8, HTST 72°C/15s |
| **Thermal** | D₁₂₁ = 0.2-0.5 min, z = 10°C, F₀ = 3-5 min |
| **Preservation** | aw < 0.6 safe, Fast freeze -30°C |
| **Irrigation** | Kc varies 0.3-1.2, η 60-90% |

---

**📌 Print this sheet and carry to exam center for last-minute revision!**

*Total Formulas: 100+ | All Sections Covered | GATE AG 2026*
