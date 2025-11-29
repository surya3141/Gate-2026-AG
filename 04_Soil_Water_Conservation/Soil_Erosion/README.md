# 🌱 Soil Erosion & Conservation

> Comprehensive theory for GATE Agricultural Engineering

---

## 📑 Table of Contents

1. [Introduction to Soil Erosion](#introduction-to-soil-erosion)
2. [Types of Erosion](#types-of-erosion)
3. [Water Erosion](#water-erosion)
4. [Wind Erosion](#wind-erosion)
5. [Soil Loss Estimation](#soil-loss-estimation)
6. [Erosion Control Measures](#erosion-control-measures)
7. [Conservation Practices](#conservation-practices)

---

## 🎯 Introduction to Soil Erosion

### Definition

**Soil erosion:** Detachment and transportation of soil particles by water, wind, or gravity.

**Natural process** but **accelerated by human activities**

---

### Impact of Erosion

**Agricultural:**
- Loss of topsoil (fertile layer)
- Reduced crop productivity (30-90%)
- Loss of nutrients and organic matter

**Environmental:**
- Siltation of water bodies
- Water pollution (sediment, chemicals)
- Habitat destruction

**Economic:**
- Reduced farm income
- Increased fertilizer costs
- Reservoir capacity loss

---

### Permissible Soil Loss

**Definition:** Maximum erosion rate that allows sustained crop productivity

**Values:**

| Land Use | Permissible Loss (t/ha/yr) |
|----------|----------------------------|
| **Agricultural land** | **4.5-11.2** ⭐ |
| **Forest land** | **2.5** |
| **Pasture** | 2.5-11.2 |
| **Marginal land** | <2.5 |

**Memory:** **"Agriculture ≈ 5-10 t/ha/yr"** (midrange)

---

## 🌊 Types of Erosion

### 1. Water Erosion

**Most important** - Causes 60-70% of soil loss in India

**Forms:**
- Splash erosion
- Sheet erosion
- Rill erosion
- Gully erosion
- Stream bank erosion

---

### 2. Wind Erosion

**Important in arid/semi-arid regions**

**Forms:**
- Suspension (fine particles)
- Saltation (medium particles)
- Surface creep (coarse particles)

---

### 3. Gravity Erosion

**Less common:**
- Landslides
- Slumping
- Mass wasting

---

## 💧 Water Erosion (Detailed)

### 1. Splash Erosion

**Mechanism:**
- Raindrop impact on soil
- Detaches particles
- Splashes up to 60 cm high
- Can move 150 cm laterally

**Kinetic energy:**
$$
KE = \frac{1}{2} m v^2
$$

Terminal velocity of raindrop: 5-9 m/s (depends on size)

---

### 2. Sheet Erosion

**Definition:** Uniform removal of thin soil layer

**Characteristics:**
- Difficult to detect initially
- Occurs on gentle slopes
- Most destructive form
- Removes topsoil uniformly

**Indicators:**
- Exposed subsoil
- Roots visible
- Crop color variation

---

### 3. Rill Erosion

**Definition:** Small channels (<30 cm deep) formed by concentrated flow

**Characteristics:**
- Can be obliterated by tillage
- Finger-like patterns
- Precursor to gully

**Formation:** When runoff velocity exceeds erosion resistance

---

### 4. Gully Erosion

**Definition:** Large channels (>30 cm deep) that cannot be crossed by farm machinery

**Characteristics:**
- **Permanent features**
- V-shaped or U-shaped
- Continuous headward cutting
- Most visible form

**Classification by depth:**
- Small: 1-3 m
- Medium: 3-7 m
- Large: >7 m

---

### 5. Stream Bank Erosion

**Mechanism:**
- Lateral cutting by stream
- Undercutting of banks
- Slumping of soil

---

## 🌬️ Wind Erosion

### Mechanism

**Three modes of particle movement:**

**1. Suspension:**
- Particles <0.1 mm (clay, silt)
- Lifted high into air
- Transported long distances (100s of km)
- Creates dust storms

**2. Saltation:**
- Particles 0.1-0.5 mm (fine sand)
- **Most important** - 50-75% of movement
- Bouncing motion (hop, skip, jump)
- Height: 30 cm to 2 m

**3. Surface Creep:**
- Particles 0.5-1.0 mm (coarse sand)
- Roll/slide along surface
- Pushed by saltating particles
- 5-25% of movement

---

### Factors Affecting Wind Erosion

**1. Wind Velocity:**
- Threshold velocity: 5-6 m/s at 30 cm height
- Erosion ∝ (Velocity)³

**2. Soil Properties:**
- Texture (sandy soils most susceptible)
- Moisture (dry soil erodes more)
- Organic matter (increases cohesion)

**3. Surface Roughness:**
- Vegetation cover
- Crop residue
- Clods and ridges

**4. Field Length:**
- Longer field = more erosion
- Fetch distance

---

### Wind Erosion Equation

**Simple form:**
$$
E = f(I, K, C, L, V)
$$

Where:
- E = Soil loss
- I = Soil erodibility index
- K = Ridge roughness factor
- C = Climatic factor
- L = Field length
- V = Vegetation cover

---

## 📐 Soil Loss Estimation

### Universal Soil Loss Equation (USLE)

**Most important equation for GATE!**

$$
\boxed{A = R \times K \times LS \times C \times P}
$$

Where:
- **A** = Average annual soil loss (t/ha/yr)
- **R** = Rainfall erosivity factor
- **K** = Soil erodibility factor
- **LS** = Topographic factor (slope length × steepness)
- **C** = Crop management factor
- **P** = Conservation practice factor

---

### R Factor (Rainfall Erosivity)

**Definition:** Erosive power of rainfall

**Formula:**
$$
R = \sum \frac{KE \times I_{30}}{100}
$$

Where:
- KE = Kinetic energy of storm (MJ/ha)
- I₃₀ = Maximum 30-min rainfall intensity (mm/h)

**Units:** MJ·mm/(ha·h·yr)

**Typical values (India):**
- Low erosivity: <200
- **Medium:** 200-400 ⭐
- High: 400-800
- Very high: >800

**Regional variation:**
- North India: 200-400
- South India: 400-800
- Western Ghats: >1000

---

### K Factor (Soil Erodibility)

**Definition:** Soil's susceptibility to erosion

**Influenced by:**
- Texture (clay, silt, sand %)
- Organic matter
- Structure
- Permeability

**Units:** t·ha·h/(ha·MJ·mm)

**Typical values:**

| Soil Texture | K Value |
|--------------|---------|
| **Sand** | 0.05-0.10 |
| **Sandy loam** | 0.15-0.25 |
| **Loam** | **0.25-0.40** ⭐ |
| **Silt loam** | 0.40-0.50 (most erodible) |
| **Clay loam** | 0.20-0.35 |
| **Clay** | 0.10-0.25 |

**Memory:** **Silt loam most erodible** (K highest)

---

**Nomograph method:** Uses % sand, silt, OM, structure, permeability

**Quick estimate:**
$$
K ≈ 0.3 \text{ (average for many soils)}
$$

---

### LS Factor (Topographic)

**Two components:**

**L (Slope length):**
- Distance from top to toe of slope
- Or to point where deposition begins

**S (Slope steepness):**
- Gradient of slope (%)

---

**Combined LS factor:**
$$
LS = \left(\frac{\lambda}{22.13}\right)^m \times (65.41 \sin^2\theta + 4.56 \sin\theta + 0.065)
$$

Where:
- λ = Slope length (m)
- θ = Slope angle
- m = Exponent (0.2-0.5, typically 0.5)

**Simplified (for slope %):**
$$
LS = \left(\frac{\lambda}{22}\right)^{0.5} \times \left(\frac{S(\%)}{9}\right)^{1.3}
$$

---

**Quick values:**

| Slope % | Slope Length (m) | LS Factor |
|---------|------------------|-----------|
| 2% | 50 | 0.4 |
| 5% | 50 | 1.0 |
| 10% | 50 | 2.5 |
| 5% | 100 | 1.4 |
| 10% | 100 | 3.5 |

**Memory:** Steep + Long = High LS

---

### C Factor (Crop Management)

**Definition:** Ratio of soil loss from cropped land to bare fallow

**Range:** 0 to 1.0

**Values:**

| Land Use/Crop | C Factor |
|---------------|----------|
| **Bare fallow** | **1.0** (reference) |
| Row crops (poor) | 0.7-0.9 |
| Row crops (good) | 0.4-0.7 |
| **Small grains** | **0.2-0.5** |
| **Dense grass** | **0.01-0.05** ⭐ |
| **Forest** | **0.001-0.01** (best) |

**Memory:** Lower C = Better protection

---

**Factors affecting C:**
- Crop type and stage
- Canopy cover
- Residue on surface
- Tillage practice

---

### P Factor (Conservation Practice)

**Definition:** Ratio of soil loss with practice to up-and-down slope farming

**Range:** 0 to 1.0 (1.0 = no practice)

**Values:**

| Practice | Slope (%) | P Factor |
|----------|-----------|----------|
| **Up-down slope** | Any | **1.0** |
| **Contour farming** | 2-7 | 0.5-0.6 |
| | 7-12 | 0.6-0.7 |
| | 12-18 | 0.7-0.8 |
| | 18-24 | 0.8-0.9 |
| **Strip cropping** | 2-7 | 0.25-0.30 |
| | 7-12 | 0.30-0.40 |
| **Terracing** | Any | **0.10-0.30** |

**Memory:** Terracing best (lowest P), Contour moderate

---

### RUSLE (Revised USLE)

**Improved version** with better estimation

**Same basic form:**
$$
A = R \times K \times LS \times C \times P
$$

**Improvements:**
- Better R factor (erosivity)
- More accurate LS (includes rill/interrill)
- Refined C factor (sub-factors)
- Time-varying factors

**For GATE:** USLE form sufficient, know concept of RUSLE

---

## 🛡️ Erosion Control Measures

### Classification

**1. Agronomic Measures** (Biological)
**2. Mechanical Measures** (Structural)
**3. Management Practices**

---

## 🌾 Agronomic Measures

### 1. Contour Farming

**Definition:** Tillage and planting along contours (equal elevation lines)

**Mechanism:**
- Ridges/furrows act as mini-barriers
- Slow runoff velocity
- Increase infiltration
- Reduce soil loss by 50%

**Suitable:** Slopes 2-8%, uniform

**Limitations:**
- Requires surveying
- Breaks at field boundaries
- Not for irregular terrain

---

### 2. Strip Cropping

**Definition:** Growing alternate strips of different crops along contours

**Types:**

**Contour strip cropping:**
- Strips follow contours
- Dense crop (grass) alternates with regular crop
- Erosion reduction: 50-75%

**Field strip cropping:**
- Straight strips (not contour)
- Easier to implement

**Buffer strip cropping:**
- Permanent grass strips
- Between cropped areas

**Typical strip width:** 15-30 m

---

### 3. Cover Cropping

**Definition:** Growing protective crops during off-season

**Benefits:**
- Protects soil from raindrop impact
- Improves soil structure (organic matter)
- Reduces runoff velocity

**Examples:**
- Legumes (cowpea, green gram)
- Grasses (rye, oats)

---

### 4. Mulching

**Definition:** Covering soil with organic/inorganic material

**Types:**
- Straw/crop residue
- Plastic film
- Gravel

**Effects:**
- Prevents splash erosion
- Reduces evaporation
- Moderates soil temperature

**Application rate:** 4-6 t/ha (straw)

---

### 5. Crop Rotation

**Definition:** Sequential cropping of different crops

**Benefits:**
- Varies root depth
- Different residues
- Breaks pest cycles
- Maintains fertility

**Example:**
Wheat → Legume → Maize → Fallow

---

### 6. Afforestation

**Definition:** Planting trees on degraded land

**Effects:**
- Canopy intercepts rainfall
- Root binding
- Litter protects surface
- Reduces wind velocity

**Best for:** Steep slopes, wastelands

---

## 🏗️ Mechanical Measures

### 1. Terracing

**Definition:** Construction of ridges across slope to intercept runoff

**Most effective mechanical measure**

---

#### Types of Terraces

**A. Bench Terraces:**
- **Most effective** (90% reduction)
- Level or slightly sloped platforms
- Step-like appearance
- Steep slopes (>15%)

**Construction:**
- Cut-and-fill
- Width: 3-15 m
- Vertical interval: 1.5-3 m

**Best for:** Hills, orchards, tea/coffee

---

**B. Broad-Base Terraces:**
- Wide, flat ridges
- Can be farmed over
- Gentle slopes (2-8%)
- Channel between ridges

**Dimensions:**
- Width: 5-15 m
- Height: 0.3-0.6 m
- Channel: 0.3-0.5 m deep

---

**C. Graded Terraces:**
- Have longitudinal slope (0.1-0.5%)
- Water flows to outlet
- Suitable: 3-8% slope
- Common in USA

---

**D. Level Terraces:**
- No slope, retain all water
- For water conservation
- Arid/semi-arid regions

---

#### Terrace Spacing

**Vertical interval (VI):**
$$
VI = \frac{XS + Y}{100}
$$

Where:
- S = Land slope (%)
- X, Y = Constants (depend on rainfall, soil)

**Typical:**
- X = 0.3-0.6
- Y = 0.6-1.5

**Example:** S = 10%, X = 0.4, Y = 1.0
$$
VI = \frac{0.4 \times 10 + 1.0}{100} = 0.05 \text{ (inconsistent units!)}
$$

**Correct formula:**
$$
VI (m) = 0.3S + 1.0 \text{ (simplified)}
$$

For 10% slope: VI = 0.3×10 + 1 = 4 m

---

### 2. Bunding

**Definition:** Constructing earthen embankments along contours

**Types:**

**Contour bunds:**
- Follow contours
- Height: 0.5-1.0 m
- Vertical interval: 1-3 m (depends on slope)

**Graded bunds:**
- Slight slope (0.1-0.3%)
- Dispose excess water

**Stone bunds:**
- In rocky areas
- Permeable structure

---

### 3. Gully Control Structures

**For active gullies:**

**Temporary structures:**
- Brush dams
- Loose rock dams
- Woven wire dams

**Permanent structures:**
- Masonry check dams
- Concrete drop structures
- Chutes/flumes

**Vegetation:**
- Grasses at periphery
- Trees on banks
- Stabilize gully

---

### 4. Waterways

**Grassed waterways:**
- Natural drainage paths
- Planted with grass
- Carry runoff safely
- Prevent gully formation

**Design:**
- Width: 3-10 m
- Grade: 0.5-4%
- Side slopes: 4:1 to 6:1

---

## 🎯 Key Points for GATE

**High Priority:**
- ✓ USLE equation and all factors (R, K, LS, C, P)
- ✓ Permissible soil loss values
- ✓ Types of water erosion
- ✓ C and P factor values
- ✓ Terrace types and spacing

**Moderate Priority:**
- Wind erosion mechanisms
- Agronomic vs mechanical measures
- Contour farming, strip cropping
- Gully classification

**Formulas:**
- A = R × K × LS × C × P (must know!)
- LS factor calculation
- Terrace spacing

---

## 📊 Comparison Tables

### Water vs Wind Erosion

| Feature | Water Erosion | Wind Erosion |
|---------|---------------|--------------|
| **Agent** | Rainfall, runoff | Wind |
| **Dominant in** | Humid, sub-humid | Arid, semi-arid |
| **Visibility** | Usually visible | Visible (dust) |
| **Control** | Terracing, bunding | Windbreaks, cover |
| **India impact** | 60-70% soil loss | 30-40% |

---

### Erosion Types by Severity

| Type | Severity | Control Difficulty |
|------|----------|-------------------|
| **Splash** | Low | Easy |
| **Sheet** | High (subtle) | Moderate |
| **Rill** | Moderate | Moderate |
| **Gully** | Very high | Difficult |
| **Stream bank** | High | Difficult |

---

## 🔗 Related Topics

- [Water Harvesting Structures](../Water_Harvesting/README.md)
- [Land Drainage](../Land_Drainage/README.md)
- [Watershed Management](../Watershed_Management/README.md)
- [Solutions - PYQs](./Solutions.md)
- [Quick Reference](./CheatSheet.md)

---

**Last Updated:** November 2025  
**Next:** Practice with PYQ Solutions!

---

*Understanding soil erosion is key to conservation!*

🌱 **Conserve Soil, Save Future!** 🌍
