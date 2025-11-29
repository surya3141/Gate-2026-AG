# ⚙️ Size Reduction

> **Comprehensive Theory for GATE Agricultural Engineering 2026**

---

## 📚 Table of Contents

1. [Introduction](#introduction)
2. [Energy Laws](#energy-laws)
3. [Size Reduction Equipment](#size-reduction-equipment)
4. [Screening and Grading](#screening-and-grading)
5. [Design Considerations](#design-considerations)

---

## 🎯 Introduction

### Purpose of Size Reduction

**Why reduce size?**
- Increase surface area for reactions
- Improve mixing and blending
- Facilitate extraction
- Enhance digestibility (animal feed)
- Prepare for further processing
- Improve handling and packaging

**Applications:**
- Flour milling (wheat, rice, maize)
- Animal feed preparation
- Spice grinding
- Oil extraction (seed crushing)
- Biomass processing

---

## ⚡ Energy Laws

### 1. Kick's Law 🔥

**Statement:** Energy required for size reduction is proportional to the logarithm of the reduction ratio.

**Formula:**
$$
E = K_k \times \log\left(\frac{D_i}{D_f}\right)
$$

where:
- E = Specific energy (kJ/kg)
- Kk = Kick's constant
- Di = Initial particle size (mm)
- Df = Final particle size (mm)
- Di/Df = Reduction ratio (R)

**Best for:** **Coarse crushing** (Di > 50 mm)

**Physical basis:**
- Energy proportional to new crack length
- For coarse crushing, cracks through entire particle
- Crack length proportional to particle size

**Example:**
Di = 50 mm, Df = 10 mm, Kk = 10 kJ/kg

$$
E = 10 \times \log(50/10) = 10 \times \log(5) = 10 \times 0.699 = 6.99 \text{ kJ/kg}
$$

### 2. Rittinger's Law 🔥

**Statement:** Energy required is proportional to the new surface area created.

**Formula:**
$$
E = K_r \times \left(\frac{1}{D_f} - \frac{1}{D_i}\right)
$$

where:
- Kr = Rittinger's constant
- Units: kJ·mm/kg

**Best for:** **Fine grinding** (Df < 1 mm)

**Physical basis:**
- Energy creates new surface
- Surface area ∝ 1/D
- More important for fine particles (larger relative surface increase)

**Example:**
Di = 50 mm, Df = 10 mm, Kr = 100 kJ·mm/kg

$$
E = 100 \times (1/10 - 1/50) = 100 \times (0.1 - 0.02) = 100 \times 0.08 = 8 \text{ kJ/kg}
$$

**Comparison with Kick:**
For 50 → 10 mm:
- Kick: 6.99 kJ/kg
- Rittinger: 8 kJ/kg

For finer grinding (e.g., 10 → 1 mm):
- Kick: 10 × log(10) = 10 kJ/kg
- Rittinger: 100 × (1 - 0.1) = 90 kJ/kg (much higher!)

**Rule:** Rittinger > Bond > Kick for fine grinding

### 3. Bond's Law 🔥

**Statement:** Compromise between Kick and Rittinger - energy proportional to crack propagation.

**Formula:**
$$
E = E_i \times \left(\frac{1}{\sqrt{D_f}} - \frac{1}{\sqrt{D_i}}\right)
$$

or in Bond Work Index form:
$$
E = 10 \times E_i \times \left(\frac{1}{\sqrt{D_f}} - \frac{1}{\sqrt{D_i}}\right)
$$

where:
- Ei = Bond work index (kWh/tonne) for 80% passing 100 μm
- D in micrometers (μm)

**Best for:** **General purpose** (intermediate sizes)

**Physical basis:**
- Energy proportional to length of crack tip
- Crack length ∝ √D
- Good approximation for most industrial applications

**Bond Work Index (Ei) for common materials:**

| Material | Ei (kWh/t) |
|----------|------------|
| Wheat | 8.5 |
| Maize | 10.3 |
| Rice | 9.0 |
| Soybeans | 12.6 |
| Limestone | 11.6 |

**Example:**
Di = 10,000 μm (10 mm), Df = 1,000 μm (1 mm), Ei = 10 kWh/t

$$
E = 10 \times 10 \times \left(\frac{1}{\sqrt{1000}} - \frac{1}{\sqrt{10000}}\right)
$$
$$
= 100 \times (0.0316 - 0.010) = 100 \times 0.0216 = 2.16 \text{ kWh/t}
$$

### 4. Comparison of Laws

| Law | Formula | Best For | Advantage |
|-----|---------|----------|-----------|
| **Kick's** | E = Kk×log(Di/Df) | Coarse crushing (>50mm) | Simple |
| **Rittinger's** | E = Kr×(1/Df-1/Di) | Fine grinding (<1mm) | Surface basis |
| **Bond's** | E = Ei×(1/√Df-1/√Di) | General (1-50mm) | Most accurate |

**Which gives maximum energy?**
- For **fine grinding:** Rittinger > Bond > Kick
- For **coarse crushing:** Kick > Bond > Rittinger

**GATE tip:** Remember "RBK fine to coarse" (Rittinger-Bond-Kick in decreasing order for fine grinding)

---

## 🔨 Size Reduction Equipment

### 1. Jaw Crusher

**Description:**
- Primary crusher
- One fixed jaw, one moving jaw
- Crushing by compression

**Specifications:**
- Feed size: Up to 1500 mm
- Product size: 50-200 mm
- Reduction ratio: 3:1 to 9:1
- Capacity: 10-500 t/hr

**Mechanism:**
- Material enters from top
- Crushed between jaws
- Product falls from bottom

**Applications:**
- Primary crushing of rocks, ores
- Rarely for agricultural products
- Very hard materials

**Advantages:**
- Simple, robust
- High capacity
- Low maintenance

**Disadvantages:**
- Large space requirement
- Coarse product only
- High power consumption

### 2. Hammer Mill 🔥

**Description:**
- Impact-based crushing
- Rotating hammers/beaters
- Most versatile mill

**Components:**
- Rotor with hammers
- Breaker plate/screen
- Feed inlet (top)
- Discharge (bottom/side)

**Specifications:**
- Feed size: 50-100 mm
- Product size: 1-20 mm
- Reduction ratio: 10:1 to 40:1
- Speed: 1000-3000 rpm
- Screen openings: 1-20 mm

**Mechanism:**
- **Impact:** Hammers strike material at high speed
- **Attrition:** Particle-particle friction
- **Shear:** Between hammer and breaker plate

**Applications:**
- **Animal feed grinding** (most common)
- Grain processing
- Spices, herbs
- Biomass (straw, stover)
- General-purpose milling

**Screen selection:**
- Fine grind: 2-5 mm screen
- Medium: 6-10 mm
- Coarse: 12-20 mm

**Advantages:**
- Versatile (coarse to medium)
- High reduction ratio
- Simple operation
- Adjustable fineness (change screen)
- Relatively low cost

**Disadvantages:**
- High power consumption
- Hammer wear
- Heat generation
- Dust production
- Over-grinding risk

**Power calculation:**
$$
P = K \times Q \times R
$$
where K depends on material (1-3 kW·hr/t)

### 3. Roller Mill

**Description:**
- Two or more rollers rotating toward each other
- Crushing by compression and shear

**Types:**

**a) Smooth rollers:**
- For fine grinding
- Flour milling

**b) Corrugated rollers:**
- For coarse breaking
- Flaking

**c) Differential speed:**
- Different roller speeds
- Shearing action

**Specifications:**
- Feed size: 10-50 mm
- Product size: 0.5-5 mm
- Reduction ratio: 4:1 to 8:1
- Roller diameter: 200-600 mm
- Speed: 300-800 rpm

**Applications:**
- **Wheat flour milling** (primary use)
- Rice milling
- Flaking (cereals)
- Oil seed crushing

**Advantages:**
- Controlled particle size
- Less dust
- Lower energy than hammer mill
- Uniform product
- Less heat generation

**Disadvantages:**
- Lower reduction ratio
- Not for hard materials
- Higher cost
- Roller wear
- Requires consistent feed

**Roll gap calculation:**
- Minimum gap = 1.05 to 1.10 × feed particle size
- For sticky materials: wider gap needed

### 4. Ball Mill

**Description:**
- Rotating cylinder with grinding balls
- Grinding by attrition and impact

**Components:**
- Cylindrical shell (horizontal)
- Grinding media (steel/ceramic balls)
- Feed: one end or center
- Discharge: other end or through screen

**Specifications:**
- Feed size: <25 mm
- Product size: <0.1 mm (very fine)
- Reduction ratio: >50:1
- Diameter: 0.5-5 m
- Length: 0.5-10 m
- Speed: 65-80% of critical speed

**Critical speed:**
$$
N_c = \frac{42.3}{\sqrt{D}}
$$
where D = diameter (m), Nc = critical speed (rpm)

At critical speed, balls centrifuge (don't cascade)
Operate at 70-80% of Nc

**Mechanism:**
- **Attrition:** Grinding between balls and shell
- **Impact:** Balls cascading down

**Applications:**
- Very fine grinding
- Cement, minerals
- Paints, pigments
- Chocolate refining

**Ball filling:**
- 30-50% of mill volume
- Higher filling → more grinding, more power

**Advantages:**
- Very fine product possible
- Closed circuit operation
- Wet or dry grinding
- Continuous operation

**Disadvantages:**
- High power consumption
- Large space
- Slow (long residence time)
- Expensive
- Ball wear

### 5. Attrition Mill

**Description:**
- Two discs (one stationary, one rotating)
- Grinding between disc surfaces

**Specifications:**
- Feed size: <10 mm
- Product size: 0.05-1 mm
- Speed: 1000-5000 rpm

**Mechanism:**
- Material fed at center
- Moves outward by centrifugal force
- Ground between disc surfaces
- Fine control by disc gap

**Applications:**
- Spices, herbs
- Fine grinding
- Pastes, purees

**Advantages:**
- Very fine grinding
- Controlled fineness
- Compact
- Suitable for wet grinding

**Disadvantages:**
- Limited capacity
- High wear
- Heat generation
- Not for hard materials

### 6. Comparison Table

| Mill Type | Feed Size | Product Size | Reduction Ratio | Best For | Power |
|-----------|-----------|--------------|-----------------|----------|-------|
| Jaw Crusher | Very large | Coarse | 3-9:1 | Primary | High |
| **Hammer Mill** | Medium | Medium | 10-40:1 | **General purpose** | High |
| **Roller Mill** | Small-Medium | Fine | 4-8:1 | **Flour** | Medium |
| Ball Mill | Small | Very fine | >50:1 | Ultra-fine | Very high |
| Attrition Mill | Small | Very fine | High | Spices, paste | Medium |

---

## 📏 Screening and Grading

### 1. Screen Terminology

**Mesh number:** Number of openings per linear inch

Formula:
$$
\text{Opening size (mm)} = \frac{25.4}{\text{Mesh number}} - \text{Wire diameter}
$$

Simplified (assuming wire ≈ opening):
$$
\text{Opening (mm)} \approx \frac{25.4}{2 \times \text{Mesh}}
$$

**Common mesh sizes:**

| Mesh | Opening (mm) | Typical Use |
|------|--------------|-------------|
| 4 | 4.75 | Coarse screen |
| 8 | 2.36 | Coarse |
| 16 | 1.18 | Medium |
| 30 | 0.60 | Medium |
| 50 | 0.30 | Fine |
| 100 | 0.15 | Very fine |
| 200 | 0.075 | Ultra-fine |

**Memory:** Higher mesh = Finer screen

### 2. Screen Efficiency

**Definition:**
$$
\eta = \frac{\text{Undersize in underflow}}{\text{Undersize in feed}} \times 100
$$

**Detailed formula:**
$$
\eta = \frac{a(b-f)}{f(a-f)} \times 100
$$

where:
- a = % undersize in overflow (reject)
- b = % undersize in underflow (product)
- f = % undersize in feed

**Typical efficiencies:**
- Commercial screens: 80-95%
- Laboratory screens: >95%

**Example:**
Feed: 70% undersize, Underflow: 95% undersize, Overflow: 10% undersize

$$
\eta = \frac{10(95-70)}{70(10-70)} \times 100 = \frac{10 \times 25}{70 \times (-60)} \times 100
$$

Actually use simpler:
$$
\eta \approx \frac{95}{70} \times 100 = 135\%?
$$

(Formula needs actual mass fractions, not percentages directly)

**Practical definition:** % of undersize recovered

### 3. Screen Types

**a) Flat screens:**
- Reciprocating/vibrating
- Most common

**b) Rotary screens:**
- Trommel screens
- Cylindrical, rotating
- For large volumes

**c) Centrifugal screens:**
- High-speed rotation
- Very fine separation

### 4. Factors Affecting Screening

**Efficiency increases with:**
- Lower feed rate
- Smaller particle size
- Lower moisture content
- Larger screen area
- Higher vibration frequency

**Efficiency decreases with:**
- Overloading
- Wet/sticky material
- Near-size particles (close to opening)
- Screen blinding (plugging)

---

## 🔧 Design Considerations

### 1. Reduction Ratio

**Definition:**
$$
R = \frac{D_i}{D_f} = \frac{\text{Feed size}}{\text{Product size}}
$$

**Typical ratios:**

| Equipment | Reduction Ratio |
|-----------|-----------------|
| Jaw crusher | 3-9:1 |
| Roller mill | 4-8:1 |
| Hammer mill | 10-40:1 |
| Ball mill | >50:1 |

**Multi-stage crushing:**
If overall R = 100:1 needed:
- Stage 1 (Jaw): 10:1 (100mm → 10mm)
- Stage 2 (Hammer): 10:1 (10mm → 1mm)

### 2. Capacity Calculations

**Hammer mill capacity:**
$$
Q = K \times P
$$
where Q = capacity (t/hr), P = power (kW), K = 0.3-1.0 (depends on material)

**Roller mill capacity:**
$$
Q = L \times D \times N \times k
$$
where:
- L = roller length (m)
- D = roller diameter (m)
- N = speed (rpm)
- k = constant (0.5-2.0 kg/(m²·rpm))

### 3. Power Requirements

**General estimation:**
$$
P = K \times Q \times R
$$
where:
- P = Power (kW)
- Q = Capacity (t/hr)
- R = Reduction ratio
- K = constant (0.5-3.0 kW·hr/t)

**K values:**
- Soft grains (wheat): 0.5-1.0
- Hard grains (maize): 1.0-2.0
- Very hard (minerals): 2.0-5.0

---

## 📊 Study Strategy

### Week 1: Energy Laws
- Memorize three laws
- Practice calculations
- Understand when each applies
- Reduction ratio problems

### Week 2: Equipment
- Hammer mill (focus)
- Roller mill (flour)
- Comparison table
- Applications

### Week 3: Screening + PYQs
- Mesh calculations
- Screen efficiency
- All 10 PYQs
- Speed practice

---

*[Solutions](./Solutions.md) | [CheatSheet](./CheatSheet.md) | [Section Home](../README.md)*
