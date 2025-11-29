# 🏪 Storage Engineering

> **Comprehensive Theory for GATE Agricultural Engineering 2026**

---

## 📚 Table of Contents

1. [Introduction](#introduction)
2. [Grain Properties](#grain-properties)
3. [Storage Structures](#storage-structures)
4. [Pressure in Storage](#pressure-in-storage)
5. [Aeration and Preservation](#aeration-and-preservation)

---

## 🎯 Introduction

### Importance of Storage

**Why store grains?**
- Bridge production and consumption
- Stabilize market prices
- Ensure year-round supply
- Buffer against crop failure
- Maintain strategic reserves

**India's storage capacity:** ~100 million tonnes (FCI + state + private)

**Storage losses:**
- Insects and pests: 5-10%
- Rodents: 2-5%
- Moisture/mold: 3-5%
- Total: **10-20% of production**

---

## 🌾 Grain Properties

### 1. Bulk Density 🔥

**Definition:** Mass per unit volume of bulk grain (including voids)

| Grain | Bulk Density (kg/m³) | Memory Aid |
|-------|---------------------|------------|
| **Paddy** | **550-600** | Lightest (with husk) |
| **Maize** | **700-750** | Medium |
| **Wheat** | **750-800** | Heavier |
| **Rice (milled)** | **800-850** | Heaviest (no husk) |
| Pulses | 750-850 | Similar to wheat |
| Soybeans | 700-750 | Similar to maize |

**Factors affecting:**
- Moisture content (↑ MC → ↑ density)
- Grain size (larger → lower density)
- Shape (spherical → higher density)
- Packing (compression → higher density)

**Uses:**
- Calculate storage capacity
- Determine bin loads
- Design handling equipment

**Example:** Cylindrical bin D = 4 m, H = 6 m, wheat (ρ = 780 kg/m³)

Volume = π/4 × D² × H = 0.785 × 16 × 6 = 75.4 m³

Mass = 75.4 × 780 = **58,812 kg ≈ 59 tonnes**

### 2. Angle of Repose 🔥

**Definition:** Angle of natural pile slope when poured freely

| Material | Angle (°) | Flowability |
|----------|-----------|-------------|
| **Wheat** | **25-30** | Good |
| **Paddy** | **30-35** | Fair |
| **Maize** | **25-30** | Good |
| **Rice** | **30-35** | Fair |
| Pulses | 30-35 | Fair |
| Oilseeds | 28-33 | Fair |

**Factors affecting:**
- Moisture content (↑ MC → ↑ angle, poor flow)
- Particle shape (round → lower angle)
- Surface roughness (smooth → lower angle)
- Particle size (uniform → lower angle)

**Applications:**
- **Hopper design:** Side wall angle > (angle of repose + 10-15°) for mass flow
- **Pile storage:** Calculate pile volume
- **Conveyor design:** Angle of surcharge

**Pile volume calculation:**
$$
V = \frac{1}{3} \pi r^2 h = \frac{1}{3} \pi r^3 \tan\theta
$$

where θ = angle of repose

### 3. Other Properties

**Porosity:**
- Void fraction in bulk grain
- Typically 35-45%
- Affects airflow resistance

**Coefficient of friction:**
- Grain-grain: 0.3-0.5
- Grain-steel: 0.25-0.40
- Grain-concrete: 0.35-0.50

**Lateral pressure ratio (k):**
- Ratio of horizontal to vertical pressure
- Typically 0.3-0.6 for grains
- Used in Janssen's equation

---

## 🏗️ Storage Structures

### 1. Classification

**By material:**
- Steel bins
- Reinforced concrete silos
- Masonry structures
- Fabric/bag storage
- Underground pits (traditional)

**By operation:**
- Temporary storage (< 6 months)
- Long-term storage (> 6 months)
- Buffer storage (commercial)

**By location:**
- Indoor warehouses
- Outdoor bins/silos
- Underground storage

### 2. Bins vs Silos

| Feature | Bin | Silo |
|---------|-----|------|
| **Height/Diameter** | **< 2** | **> 2** |
| Shape | Cylindrical/rectangular | Tall cylindrical |
| Capacity | 50-500 tonnes | 100-10,000 tonnes |
| Discharge | Gravity | Gravity/mechanical |
| Cost | Lower | Higher |
| Best for | Farms, small-scale | Commercial, bulk |

**Bin:** H/D < 2 (squat structure)
**Silo:** H/D > 2 (tall structure)

### 3. Warehouse Design

**CAP (Cover and Plinth) warehouses:**
- Capacity: 1,000-10,000 tonnes
- Grain in bags on raised platform
- Covered storage
- Natural ventilation

**Design parameters:**
- Stack height: 4-6 m (15-20 bags)
- Clearance: 45-60 cm from walls
- Aisle width: 1.0-1.5 m
- Plinth height: 15-30 cm

**Advantages:**
- Flexibility (any grain)
- Easy inspection
- Simple construction

**Disadvantages:**
- Labor intensive
- Lower space utilization
- Bag cost

### 4. Bin/Silo Design Considerations

**Shape:**
- **Circular:** Most efficient (area/perimeter), common
- **Square:** Easier construction, less efficient
- **Rectangular:** For modular units

**Hopper:**
- **Mass flow:** Entire contents move, FIFO, steep walls (>50°)
- **Funnel flow:** Central core moves first, flat bottom

**Roof:**
- Conical (most common)
- Dome (stronger, costlier)
- Flat (for silos with covers)

**Floor:**
- Conical (gravity discharge)
- Flat (mechanical sweep)
- Hopper bottom (steep discharge)

---

## ⚖️ Pressure in Storage

### 1. Janssen's Equation 🔥

**Problem:** In deep storage, why doesn't pressure increase linearly with depth?

**Answer:** Wall friction supports part of the grain weight

**Janssen's equation for vertical pressure:**
$$
P_v = \frac{\gamma R}{k\mu} \times \left[1 - e^{-\frac{k\mu h}{R}}\right]
$$

where:
- Pv = Vertical pressure at depth h (kPa)
- γ = Bulk weight = ρg (kN/m³)
- R = Hydraulic radius = A/P (m)
  - For cylinder: R = D/4
  - For square: R = Side/4
- k = Lateral pressure ratio (0.3-0.6)
- μ = Coefficient of friction (wall-grain)
- h = Depth below surface (m)

**Lateral (horizontal) pressure:**
$$
P_h = k \times P_v
$$

**At large depth (h → ∞):**
$$
P_{v,max} = \frac{\gamma R}{k\mu}
$$

Pressure approaches asymptotic limit!

**Physical meaning:**
- Initially, pressure ≈ γh (hydrostatic)
- As depth increases, wall friction increases
- At large depth, wall friction balances weight
- Pressure plateaus at γR/(kμ)

**Example:**

Cylindrical bin: D = 4 m, h = 10 m
- Wheat: ρ = 780 kg/m³, γ = 7.8 kN/m³
- k = 0.4, μ = 0.3

R = D/4 = 4/4 = 1 m

$$
\frac{k\mu h}{R} = \frac{0.4 \times 0.3 \times 10}{1} = 1.2
$$

$$
e^{-1.2} = 0.301, \quad 1 - e^{-1.2} = 0.699
$$

$$
\frac{\gamma R}{k\mu} = \frac{7.8 \times 1}{0.4 \times 0.3} = \frac{7.8}{0.12} = 65 \text{ kN/m}^2 = 65 \text{ kPa}
$$

$$
P_v = 65 \times 0.699 = 45.4 \text{ kPa}
$$

$$
P_h = 0.4 \times 45.4 = 18.2 \text{ kPa}
$$

**Compare with hydrostatic:** P = γh = 7.8 × 10 = 78 kPa (higher!)

**Wall load (for design):**
- Vertical shear stress: τv = Pv × μ
- Hoop stress in wall: σ = Ph × R / t (t = wall thickness)

### 2. Typical Parameter Values

| Grain | k | μ (steel) | μ (concrete) |
|-------|---|-----------|--------------|
| Wheat | 0.40-0.50 | 0.25-0.35 | 0.35-0.45 |
| Paddy | 0.50-0.60 | 0.30-0.40 | 0.40-0.50 |
| Maize | 0.40-0.50 | 0.25-0.35 | 0.35-0.45 |
| Rice | 0.40-0.50 | 0.25-0.35 | 0.35-0.45 |

**For design:** Use upper bound values (conservative)

---

## 🌬️ Aeration and Preservation

### 1. Purpose of Aeration

**Why aerate?**
- Cool grain (prevent hot spots)
- Reduce moisture migration
- Control insect activity
- Prevent spoilage
- Maintain quality

**Not for drying!** (airflow too low)

### 2. Aeration Rate 🔥

**Recommended rates:**

| Purpose | Rate (m³/min per tonne) | Rate (m³/hr per tonne) |
|---------|------------------------|------------------------|
| **Maintenance** | **0.01-0.02** | **0.6-1.2** |
| Cooling | 0.02-0.05 | 1.2-3.0 |
| Emergency | 0.05-0.10 | 3.0-6.0 |

**Most common for GATE:** 0.01-0.02 m³/(min·t)

**Design airflow:**
$$
Q = m \times q
$$

where:
- Q = Total airflow (m³/min)
- m = Grain mass (tonnes)
- q = Specific airflow (m³/(min·t))

**Example:** 100 tonnes wheat, q = 0.015 m³/(min·t)

Q = 100 × 0.015 = **1.5 m³/min**

### 3. Aeration System Design

**Components:**
- **Fan:** Centrifugal or axial
- **Ducts:** Perforated, buried in grain
- **Controls:** Manual or automatic (temperature-based)

**Fan sizing:**
$$
P = \frac{Q \times \Delta P}{\eta \times 60}
$$

where:
- P = Power (kW)
- Q = Airflow (m³/min)
- ΔP = Static pressure (Pa)
- η = Fan efficiency (0.5-0.7)

**Pressure drop:** Depends on depth, grain type, airflow rate
- Typical: 500-2000 Pa for 3-5 m depth

**Duct spacing:**
- Lateral ducts: 1.5-2.5 m apart
- Main duct: Center of bin

### 4. Controlled Atmosphere Storage (CAS) 🔥

**Principle:** Modify gas composition to inhibit respiration and insects

**Modified atmosphere:**
- **O₂: Reduced to 2-5%** (from 21% normal)
- **CO₂: Increased to 10-20%** (from 0.03% normal)
- **N₂: Balance** (inert filler)

**Methods:**
1. **N₂ flushing:** Displace air with N₂
2. **CO₂ injection:** Add CO₂ directly
3. **Sealed storage:** Natural respiration reduces O₂

**Benefits:**
- Kills insects (larvae, eggs)
- Prevents mold growth
- Maintains quality (color, nutrition)
- Reduces need for fumigation
- Extended shelf life (2-3x normal)

**Limitations:**
- High initial cost
- Requires sealed structure
- Monitoring needed
- Not suitable for high-moisture grain

**Applications:**
- Export quality grains
- Seed storage
- High-value products (spices)

### 5. Storage Pest Management

**Major pests:**

| Pest | Grain | Temperature Range |
|------|-------|-------------------|
| **Rice weevil** | Whole grains | 15-34°C |
| **Red flour beetle** | Flour, damaged grain | 20-37°C |
| **Lesser grain borer** | All cereals | 25-35°C |
| **Khapra beetle** | All grains | 25-40°C (dry) |

**Integrated Pest Management (IPM):**

1. **Preventive:**
   - Clean storage before filling
   - Proper drying (MC < 14%)
   - Seal cracks, prevent entry
   - FIFO rotation

2. **Physical:**
   - Aeration (cooling)
   - Heating (>50°C kills insects)
   - Freezing (<-15°C)

3. **Chemical:**
   - Fumigation (Phosphine, Methyl bromide)
   - Contact insecticides (Malathion, Deltamethrin)
   - Inert dusts (Diatomaceous earth)

4. **Biological:**
   - Natural enemies (parasitoids)
   - Less common in grain storage

**Fumigation:**
- **Phosphine (PH₃):** Most common, 1-3 g/m³, 5-7 days exposure
- **Methyl bromide:** Being phased out (ozone depletion)
- Requires gas-tight structure

---

## 📊 Study Strategy

### Week 1: Properties + Pressure
- Bulk density values
- Angle of repose
- Janssen's equation (focus!)
- Practice pressure calculations

### Week 2: Structures + Aeration
- Bin vs silo
- Aeration rates (critical!)
- CAS concept
- Pest management basics

### Week 3: PYQs + Revision
- All 8 solved
- Janssen calculation practice
- Quick recall: densities, angles, rates

---

*[Solutions](./Solutions.md) | [CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
