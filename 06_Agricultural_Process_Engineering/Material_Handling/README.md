# 🚜 Material Handling

> **Comprehensive Theory for GATE Agricultural Engineering 2026**

---

## 📚 Table of Contents

1. [Introduction](#introduction)
2. [Belt Conveyors](#belt-conveyors)
3. [Screw Conveyors](#screw-conveyors)
4. [Bucket Elevators](#bucket-elevators)
5. [Pneumatic Conveying](#pneumatic-conveying)
6. [Other Systems](#other-systems)

---

## 🎯 Introduction

### Purpose of Material Handling

**Why needed?**
- Move materials between process units
- Load/unload storage
- Feed processing equipment
- Continuous production lines
- Reduce manual labor

**Key considerations:**
- Material type (grain, powder, bulk)
- Distance (short/long, horizontal/vertical)
- Capacity required
- Cost (capital + operating)
- Space available

---

## 🔄 Belt Conveyors

### 1. Description

**Most common material handling equipment**

**Components:**
- Endless belt (rubber, fabric, steel cord reinforced)
- Drive pulley (head, motorized)
- Tail pulley (belt return)
- Idler rollers (support belt)
- Frame/structure

**Belt cross-section:**
- Flat belt
- Troughed belt (most common for bulk materials)
  - 20° trough angle (shallow)
  - 35° trough angle (standard)
  - 45° trough angle (steep)

### 2. Capacity Calculation 🔥

**General formula:**
$$
Q = 3.6 \times A \times v \times \rho
$$

where:
- Q = Capacity (tonnes/hour)
- A = Cross-sectional area of material (m²)
- v = Belt velocity (m/s)
- ρ = Bulk density (tonnes/m³)
- 3.6 = Conversion factor (m³/s to m³/hr ÷ 1000)

**Derivation:**
- Volume flow rate = A × v (m³/s)
- Mass flow rate = A × v × ρ (t/s)
- Convert to t/hr: × 3600 s/hr = 3600 A v ρ
- But ρ usually in kg/m³, so divide by 1000
- Factor: 3600/1000 = **3.6**

**Cross-sectional area (troughed belt):**

For 35° trough, three-roll idler:
$$
A = b^2 \times (0.40 \cos\theta - 0.025)
$$

Simplified for 35° trough:
$$
A \approx 0.30 \times b^2
$$

where b = belt width (m)

**Example:**

Belt width = 0.6 m, velocity = 2 m/s, wheat (ρ = 0.75 t/m³)

A = 0.30 × 0.6² = 0.30 × 0.36 = 0.108 m²

Q = 3.6 × 0.108 × 2 × 0.75 = **0.583 t/hr = 583 kg/hr**

**For given A directly:**

A = 0.02 m², v = 1.5 m/s, ρ = 800 kg/m³ = 0.8 t/m³

Q = 3.6 × 0.02 × 1.5 × 0.8 = 3.6 × 0.024 = **0.0864 t/hr = 86.4 t/hr**

(Note: This assumes area already given)

### 3. Belt Velocity

**Typical velocities:**

| Material | Velocity (m/s) |
|----------|----------------|
| Fine powder | 0.8-1.5 |
| Grain (wheat, rice) | 1.5-2.5 |
| Coarse grain (maize) | 2.0-3.5 |
| Lumpy material | 2.5-4.0 |

**Higher velocity:**
- ✅ Higher capacity
- ❌ More spillage, dust
- ❌ Higher power

**Design choice:** Balance capacity vs. stability

### 4. Angle of Surcharge 🔥

**Definition:** Angle of material surface on moving belt

**Relationship:**
$$
\theta_{surcharge} = \theta_{repose} - (5° \text{ to } 10°)
$$

**Why less than repose angle?**
- Belt vibration
- Acceleration effects
- Dynamic vs. static pile

**Example:**
- Wheat: θr = 28°, θs ≈ **20°**
- Paddy: θr = 32°, θs ≈ **24°**

**Use in design:** Determines max load profile (troughed section area)

### 5. Power Calculation

**For horizontal belt:**
$$
P = \frac{Q \times L \times f \times g}{3600}
$$

where:
- P = Power (kW)
- Q = Capacity (t/hr)
- L = Length (m)
- f = Friction coefficient (0.02-0.04)
- g = 9.81 m/s²

**For inclined belt (add lifting power):**
$$
P = P_{horizontal} + P_{lift}
$$

$$
P_{lift} = \frac{Q \times \Delta H \times g}{3600}
$$

where ΔH = vertical lift (m)

**Total power:**
$$
P_{motor} = \frac{P}{\eta}
$$

where η = drive efficiency (0.85-0.95)

**Example:** 100 t/hr, L = 50 m, f = 0.03, horizontal

P = (100,000 × 50 × 0.03 × 9.81) / 3600 = 408.75 W ≈ **0.41 kW**

### 6. Belt Width Selection

**Rule of thumb:**
$$
b \geq 2.5 \times d_{max}
$$

where dmax = maximum particle size

**Standard widths:** 300, 400, 500, 600, 750, 900, 1200 mm

**Selection based on capacity:**
- 100-500 t/hr: 600-750 mm
- 500-1000 t/hr: 900-1200 mm
- >1000 t/hr: 1200-1500 mm

### 7. Advantages and Disadvantages

**Advantages:**
- High capacity (up to 10,000 t/hr)
- Long distance (up to several km)
- Continuous operation
- Low maintenance
- Economical for large volumes
- Versatile (various materials)

**Disadvantages:**
- Fixed route
- Not suitable for vertical lift (max 15-20° incline)
- Space requirement
- Spillage/dust issues
- Belt wear

---

## 🌀 Screw Conveyors

### 1. Description

**Rotating helical screw in trough**

**Components:**
- Helical screw (flighting)
- Shaft (center)
- Trough (U-shaped housing)
- Drive motor (one end)
- Bearings
- Inlet/outlet

**Types by pitch:**
- **Standard pitch:** Pitch = Diameter (most common)
- **Short pitch:** P < D (higher torque)
- **Long pitch:** P > D (faster discharge)

### 2. Capacity Calculation 🔥

**Formula:**
$$
Q = \frac{\pi}{4} \times D^2 \times p \times N \times \eta
$$

where:
- Q = Capacity (m³/min or m³/hr)
- D = Screw diameter (m)
- p = Pitch (m)
- N = Rotational speed (rpm)
- η = Loading efficiency (0.15-0.45, typically **0.30-0.40**)

**For mass flow:**
$$
Q_{mass} = Q_{volume} \times \rho \times 60 \text{ (if in m³/min)}
$$

**Loading efficiency (η):**

| Material | η | Reason |
|----------|---|--------|
| Free-flowing (grain) | 0.40-0.45 | Easy movement |
| Average | 0.30-0.35 | Standard |
| Sticky/sluggish | 0.15-0.25 | Poor flow |

**Never 100%!** Some space needed for material to tumble and advance.

**Example:**

D = 150 mm = 0.15 m, p = 200 mm = 0.2 m, N = 60 rpm, η = 0.40

$$
Q = \frac{3.14}{4} \times (0.15)^2 \times 0.2 \times 60 \times 0.40
$$
$$
= 0.785 \times 0.0225 \times 0.2 \times 60 \times 0.40
$$
$$
= 0.0848 \text{ m}^3/\text{min} = 5.09 \text{ m}^3/\text{hr}
$$

If wheat (ρ = 750 kg/m³):
Qmass = 5.09 × 0.75 = **3.82 t/hr**

### 3. Speed Selection

**Typical speeds:**

| Diameter (mm) | Max Speed (rpm) | Material |
|---------------|-----------------|----------|
| 100-150 | 100-120 | Heavy/abrasive |
| 150-250 | 80-100 | Average |
| 250-400 | 60-80 | Light grain |
| >400 | 40-60 | Very light |

**Higher speed:**
- ✅ Higher capacity
- ❌ More wear
- ❌ Material degradation
- ❌ Higher power

### 4. Power Calculation

**Empty screw power:**
$$
P_0 = K_0 \times L \times N
$$

**Loaded screw power:**
$$
P = P_0 + K_1 \times Q \times L
$$

where K0, K1 are constants depending on diameter

**Simplified:**
$$
P \approx 0.01 \times Q \times L
$$

where P (kW), Q (t/hr), L (m)

### 5. Applications

**Best for:**
- Short distances (< 30 m)
- Horizontal or slight incline (< 20°)
- Enclosed transport (dust control)
- Mixing during transport
- Feeding equipment (controlled rate)

**Common uses:**
- Grain elevator feed
- Mill feeding
- Silo discharge
- Mixing/blending

### 6. Advantages and Disadvantages

**Advantages:**
- Enclosed (dust-free, sanitary)
- Simple, compact
- Can mix while conveying
- Multiple inlets/outlets possible
- No spillage
- Low cost

**Disadvantages:**
- Short distance only
- High power consumption
- Material degradation (breaking kernels)
- High wear on screw and trough
- Not for sticky materials
- Limited to ~40° incline

---

## 🪣 Bucket Elevators

### 1. Description

**Vertical lifting equipment**

**Components:**
- Buckets (steel, plastic)
- Belt or chain (endless loop)
- Head pulley/sprocket (top, driven)
- Boot pulley/sprocket (bottom)
- Casing (encloses buckets)
- Loading (boot section)
- Discharge (head section)

**Types by speed:**

**a) Centrifugal discharge:**
- High speed (100-150 m/min)
- Spaced buckets
- Discharge by centrifugal force
- For free-flowing materials

**b) Positive (continuous) discharge:**
- Low speed (30-60 m/min)
- Buckets close together (continuous)
- Discharge by bucket tipping
- For sticky/sluggish materials

### 2. Capacity

**Formula:**
$$
Q = \frac{V_b \times N_b \times \rho \times 60}{1000}
$$

where:
- Q = Capacity (t/hr)
- Vb = Bucket volume (liters)
- Nb = Number of buckets per meter
- ρ = Bulk density (kg/m³)
- 60 = minutes per hour

**Bucket spacing:**
- Centrifugal: 2-4 buckets/m
- Continuous: 6-10 buckets/m

**Example:**

Bucket volume = 2 liters, spacing = 3 buckets/m, speed = 60 m/min, wheat (ρ = 750 kg/m³)

Buckets per minute = 3 × 60 = 180

Q = (2 × 180 × 750) / 1000 = 270 kg/min = **16.2 t/hr**

### 3. Power Calculation

**Lifting power:**
$$
P = \frac{Q \times H \times g}{3600 \times \eta}
$$

where:
- Q = Capacity (t/hr)
- H = Lift height (m)
- η = Efficiency (0.6-0.8)

**Example:** 20 t/hr, H = 15 m, η = 0.70

P = (20,000 × 15 × 9.81) / (3600 × 0.70) = **1.17 kW**

Add 20-30% for drive and friction → **1.4-1.5 kW**

### 4. Applications

**Best for:**
- **Vertical transport** (primary use)
- Heights 5-50 m (sometimes >100 m)
- Free-flowing to moderately sticky
- Grain elevators (hence the name!)

**Typical installations:**
- Ship unloading
- Grain elevator facilities
- Feed mills
- Flour mills

### 5. Advantages and Disadvantages

**Advantages:**
- Excellent for vertical lift
- High capacity in small footprint
- Enclosed (no spillage)
- Continuous operation
- Energy efficient for vertical transport
- Suitable for high lifts

**Disadvantages:**
- Vertical only (no horizontal)
- Fragile materials may break
- Maintenance (buckets, chains)
- Not for very sticky materials
- Boot loading critical

---

## 💨 Pneumatic Conveying

### 1. Description

**Material transported suspended in air stream**

**Types:**

**a) Dilute phase (lean phase):**
- Low solid:air ratio (< 15)
- High air velocity (15-30 m/s)
- Material fully suspended
- Long distance capability

**b) Dense phase (rich phase):**
- High solid:air ratio (> 15)
- Low air velocity (3-10 m/s)
- Material partially suspended (slugs)
- Short distance, less degradation

**Pressure systems:**
- **Positive pressure (push):** Fan/blower at inlet, push material
- **Negative pressure (pull):** Fan at outlet, suck material
- **Combination:** Both push and pull

### 2. Air Velocity 🔥

**Minimum velocity (saltation velocity):**
- Just sufficient to keep particles suspended
- If below this → settling, blockage

**For grains:**
- **Dilute phase:** 15-30 m/s
- **Dense phase:** 3-10 m/s

**Factors affecting:**
- Particle size (larger → higher velocity)
- Particle density (heavier → higher velocity)
- Moisture content (wet → higher velocity)

### 3. Air Requirements

**Solid loading ratio:**
$$
\mu = \frac{\text{Mass flow rate of solid}}{\text{Mass flow rate of air}}
$$

**Dilute phase:** μ = 1 to 15
**Dense phase:** μ = 15 to 50

**Airflow calculation:**
$$
Q_{air} = \frac{Q_{solid}}{\mu}
$$

**Pressure drop:**
- Depends on distance, bends, solid loading
- 5-50 kPa typical for dilute phase

### 4. Applications

**Best for:**
- Long distance (100-1000 m)
- Multiple pick-up or delivery points
- Flexible routing (pipes can bend)
- Clean, enclosed system
- Vertical, horizontal, inclined (any angle)

**Common uses:**
- Flour mill pneumatic systems
- Grain ship unloading
- Silo filling
- Dust collection with transport

### 5. Advantages and Disadvantages

**Advantages:**
- Flexible routing (any direction)
- Multiple inlets/outlets
- No moving parts in pipe (low maintenance)
- Completely enclosed (dust-free)
- Can transport to/from storage easily

**Disadvantages:**
- **High power consumption** (moving air + material)
- Material degradation (high velocity impacts)
- Moisture sensitive
- Abrasive wear on pipes (bends especially)
- Complex design

---

## 🔗 Other Systems

### 1. Chain Conveyors

**Drag chain conveyor:**
- Chain drags material through trough
- Fully enclosed
- Horizontal or steep incline
- Heavy-duty

**Applications:** Heavy materials, abrasive materials

### 2. Vibratory Conveyors

**Vibrating trough:** Material "jumps" forward

**Applications:** Controlled feeding, short distance

### 3. Rollers and Skate Wheel

**For packages/bags:** Not for bulk grain

---

## 📊 Comparison Table

| Conveyor Type | Best Orientation | Distance | Capacity | Power | Degradation | Cost |
|---------------|------------------|----------|----------|-------|-------------|------|
| **Belt** | Horizontal, slight incline | Long | Very High | Low | Low | Medium |
| **Screw** | Horizontal, slight incline | Short | Medium | High | Medium | Low |
| **Bucket Elevator** | **Vertical** | Medium | High | Medium | Low | Medium |
| **Pneumatic** | Any angle | Long | Medium | Very High | High | High |

**Selection guide:**

| Need | Choose |
|------|--------|
| Horizontal, long, high capacity | **Belt** |
| Horizontal, short, enclosed | **Screw** |
| **Vertical lifting** | **Bucket elevator** |
| Flexible routing, multiple points | **Pneumatic** |

---

## 📚 Study Strategy

### Week 1: Belt Conveyors
- Capacity formula (Q = 3.6Avρ)
- Power calculations
- Angle of surcharge concept
- Practice numerical problems

### Week 2: Screw and Bucket
- Screw capacity (with efficiency)
- Bucket elevator for vertical
- Speed and power
- Applications clear

### Week 3: Pneumatic + PYQs
- Velocity ranges (15-30 m/s dilute)
- All 6 PYQs solved
- Equipment selection practice

---

*[Solutions](./Solutions.md) | [CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
