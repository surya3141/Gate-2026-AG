# ⚡ Plant Protection Equipment - Quick Reference

> Essential formulas, specifications, and memory tricks for GATE AG

---

## 🔑 Key Formulas

### 1. Application Rate

**General Formula:**
$$
\text{Application rate (L/ha)} = \frac{Q \times 600}{W \times S}
$$

Where:
- Q = Flow rate (L/min)
- W = Swath width (m)
- S = Speed (km/h)
- 600 = Conversion constant

**Memory Trick:** **"Q-600 over W-S"**

---

### 2. Calibration (Area Method)

$$
\text{Application rate (L/ha)} = \frac{\text{Volume used (L)}}{\text{Area (m}^2\text{)}} \times 10000
$$

**For 100 m² test area:**
$$
\text{Rate} = \text{Volume used} \times 100
$$

**Example:** Used 6 L in 100 m² → 6 × 100 = 600 L/ha

---

### 3. Nozzle Discharge

$$
Q = K\sqrt{P}
$$

Where:
- Q = Discharge (L/min)
- K = Nozzle constant
- P = Pressure (bar)

**Changing Pressure:**
$$
\frac{Q_2}{Q_1} = \sqrt{\frac{P_2}{P_1}}
$$

**Double pressure → 1.41× flow**

**Memory:** **"Q equals K root P"**

---

### 4. Boom Height

$$
h = \frac{W}{2 \tan(\theta/2)}
$$

Where:
- h = Height above target (cm)
- W = Nozzle spacing (cm)
- θ = Spray angle (degrees)

**For 110° nozzle, 50 cm spacing:**
$$
h = \frac{50}{2 \times 1.428} = 17.5 \text{ cm}
$$

**Practical:** Add 40-60 cm above canopy

---

### 5. Terminal Velocity (Droplet)

$$
V_t = \frac{d^2 (\rho_p - \rho_a) g}{18\mu}
$$

Where:
- d = Droplet diameter (m)
- ρ_p = Droplet density (kg/m³)
- ρ_a = Air density (kg/m³)
- μ = Air viscosity (Pa·s)

**Key:** V_t ∝ d² (velocity proportional to diameter squared)

---

### 6. Concentration

**From percentage:**
$$
\text{Chemical amount (L)} = \frac{\text{Required \%} \times \text{Total volume}}{100}
$$

**Example:** 2% in 500 L = (2 × 500)/100 = 10 L

**Dilution ratio:**
$$
\text{Concentration (\%)} = \frac{\text{Chemical}}{\text{Total solution}} \times 100
$$

---

### 7. Field Capacity

$$
\text{Field capacity (ha/h)} = \frac{W \times S}{10}
$$

Where:
- W = Swath width (m)
- S = Speed (km/h)

---

### 8. Dust Application Rate

$$
\text{Application rate (kg/ha)} = \frac{Q \times 10}{W \times S}
$$

Where:
- Q = Dust discharge (kg/h)
- W = Swath width (m)
- S = Speed (km/h)

---

## 📊 Nozzle Types Comparison

### Quick Selection Guide

| Chemical Type | Nozzle | Droplet Size | Why |
|---------------|--------|--------------|-----|
| **Insecticides** | Hollow cone | Fine (50-200 μm) | Penetration |
| **Fungicides** | Hollow/Solid cone | Medium (100-300 μm) | Coverage |
| **Herbicides** | Flat fan | Coarse (200-400 μm) | Less drift |
| **Fertilizers** | Solid cone | Medium-Coarse | Full coverage |

**Memory:** **"Insects need Fine Hollow, Herbs need Flat Coarse"**

---

### Nozzle Pattern Details

| Type | Pattern | Pressure | Drift Risk | Use |
|------|---------|----------|------------|-----|
| **Hollow cone** | Ring | 3-10 bar | High | Insect/Fungi |
| **Solid cone** | Full circle | 2-5 bar | Medium | Fertilizer |
| **Flat fan** | Ellipse | 2-4 bar | Low | Herbicide |
| **Deflector** | Wide flat | 1-3 bar | Very low | Low-drift |

---

## 🎨 Nozzle Color Coding (ISO)

| Color | Flow at 3 bar | Orifice | Code |
|-------|---------------|---------|------|
| **Orange** | 0.4 L/min | 1.0 mm | 01 |
| **Green** | 0.6 L/min | 1.5 mm | 015 |
| **Yellow** | 0.8 L/min | 2.0 mm | 02 |
| **Blue** | 1.2 L/min | 3.0 mm | 03 |
| **Red** | 1.6 L/min | 4.0 mm | 04 |
| **Brown** | 2.0 L/min | 5.0 mm | 05 |

**Memory:** **"Orange Gives Yellow Blue Red Brown"** (O-G-Y-B-R-B)

---

## 💧 Droplet Size Classification

| Category | Size (μm) | Drift | Coverage | Application |
|----------|-----------|-------|----------|-------------|
| **Mist** | 10-50 | Extreme | Poor | ULV only |
| **Fine** | 50-100 | High | Excellent | Insecticides |
| **Medium** | 100-200 | Medium | Good | Fungicides |
| **Coarse** | 200-400 | Low | Fair | Herbicides |
| **Very Coarse** | >400 | Very low | Poor | Soil application |

**Memory:** **"Smaller = More drift"**

---

### Terminal Velocity by Size

| Droplet Size | Terminal Velocity | Time from 2m | Drift in 10 km/h wind |
|--------------|-------------------|--------------|----------------------|
| **50 μm** | 0.08 m/s | 25 s | 69 m |
| **100 μm** | 0.3 m/s | 6.5 s | 18 m |
| **200 μm** | 1.2 m/s | 1.7 s | 5 m |
| **400 μm** | 4.8 m/s | 0.4 s | 1 m |

**Key:** Droplets <100 μm = High drift risk

---

## ⚙️ Pump Types Comparison

| Pump Type | Pressure | Self-priming | Flow | Best For |
|-----------|----------|--------------|------|----------|
| **Piston** | 10-30 bar | Yes | Medium | Power sprayers |
| **Diaphragm** | 5-15 bar | Yes | Low-Medium | Knapsack |
| **Centrifugal** | 2-8 bar | No | High | Boom sprayers |
| **Roller** | 5-10 bar | Yes | Medium-High | Boom |

**Memory for GATE:**
- **High pressure → Piston**
- **High volume → Centrifugal**
- **Knapsack → Diaphragm**

---

## 📏 Standard Specifications

### Knapsack Sprayer (Manual)

| Parameter | Specification |
|-----------|---------------|
| **Capacity** | 10-20 L |
| **Pressure** | 2-4 bar |
| **Discharge** | 0.5-1.5 L/min |
| **Swath** | 1-2 m |
| **Coverage** | 0.2-0.4 ha/h |
| **Weight (full)** | 15-25 kg |

---

### Power Sprayer (Motorized)

| Parameter | Specification |
|-----------|---------------|
| **Capacity** | 50-500 L |
| **Engine** | 2-10 HP |
| **Pressure** | 8-30 bar |
| **Discharge** | 2-10 L/min |
| **Coverage** | 1-3 ha/h |
| **Hose length** | 30-100 m |

---

### Boom Sprayer

| Parameter | Specification |
|-----------|---------------|
| **Capacity** | 200-1000 L |
| **Boom width** | 6-24 m |
| **Nozzle spacing** | 50 cm (typical) |
| **Pressure** | 2-5 bar |
| **Coverage** | 2-8 ha/h |
| **Application** | 200-500 L/ha |

---

### Duster (Motorized)

| Parameter | Specification |
|-----------|---------------|
| **Capacity** | 5-15 kg |
| **Engine** | 1-2 HP |
| **Discharge** | 5-20 kg/h |
| **Application** | 10-20 kg/ha |
| **Coverage** | 0.5-1 ha/h |

---

## 🎯 Application Volume Classification

| Category | Volume (L/ha) | Equipment | Typical Use |
|----------|---------------|-----------|-------------|
| **High Volume** | >500 | Boom sprayer | Herbicides |
| **Medium Volume** | 50-500 | Knapsack/Power | Most pesticides |
| **Low Volume** | 5-50 | Power sprayer | Insecticides |
| **Ultra-Low (ULV)** | <5 | Aerial | Large areas |

**Memory:** **"More volume = Less concentration"**

---

## 🧮 Quick Calculation Templates

### Template 1: Application Rate (Boom)

**Given:** Q = 24 L/min, W = 6 m, S = 6 km/h

**Solution:**
$$
\text{Rate} = \frac{24 \times 600}{6 \times 6} = \frac{14400}{36} = 400 \text{ L/ha}
$$

---

### Template 2: Calibration (Area)

**Given:** Used 8 L in 100 m²

**Solution:**
$$
\text{Rate} = \frac{8}{100} \times 10000 = 800 \text{ L/ha}
$$

**Quick:** Volume × 100 = Rate

---

### Template 3: Nozzle Discharge

**Given:** K = 0.8, P = 9 bar

**Solution:**
$$
Q = 0.8 \times \sqrt{9} = 0.8 \times 3 = 2.4 \text{ L/min}
$$

---

### Template 4: Concentration

**Given:** Need 2% in 500 L

**Solution:**
$$
\text{Chemical} = \frac{2 \times 500}{100} = 10 \text{ L}
$$

Water = 500 - 10 = 490 L

---

### Template 5: Boom Height

**Given:** 110° nozzle, 50 cm spacing

**Solution:**
$$
h = \frac{50}{2 \times \tan(55°)} = \frac{50}{2.856} = 17.5 \text{ cm}
$$

Practical: Add 40 cm for canopy → Total 57.5 cm

---

## 🌬️ Drift Management

### Wind Speed Guidelines

| Wind Speed | Condition | Recommendation |
|------------|-----------|----------------|
| **<5 km/h** | Calm | Ideal for spraying |
| **5-10 km/h** | Light breeze | Acceptable |
| **10-15 km/h** | Moderate | Caution, use coarse |
| **>15 km/h** | Strong | Avoid spraying |

**Memory:** **"Below 10 is Fine, Above 15 is No"**

---

### Drift Reduction Priority

**Most effective to least:**

1. **Use larger droplets** (Change nozzle/reduce pressure)
2. **Lower boom height** (40-50 cm above canopy)
3. **Add drift-control agent** (Increases droplet size)
4. **Choose calm conditions** (Spray early morning/evening)

**Memory:** **"Big Drops Low Boom"**

---

## 🛡️ Safety - Pesticide Toxicity

### WHO Classification

| Class | Color | Toxicity | Label |
|-------|-------|----------|-------|
| **Ia** | Red (skull) | Extremely toxic | DANGER |
| **Ib** | Red | Highly toxic | DANGER |
| **II** | Yellow | Moderately toxic | WARNING |
| **III** | Blue | Slightly toxic | CAUTION |
| **U** | Green | Unlikely hazard | CAUTION |

**Memory:** **"Red Dead, Yellow Yell, Blue Okay, Green Go"**

---

### Essential PPE

**For all pesticides:**
1. ✓ Protective clothing (coveralls)
2. ✓ Chemical-resistant gloves
3. ✓ Boots (rubber)
4. ✓ Goggles/face shield
5. ✓ Respirator (for Class I & II)
6. ✓ Hat

**Memory:** **"C-G-B-G-R-H = Cover, Gloves, Boots, Goggles, Respirator, Hat"**

---

## 🔧 Sprayer Components

### Knapsack Components

| Component | Function |
|-----------|----------|
| **Tank** | Stores liquid (10-20 L) |
| **Pump** | Creates pressure (2-4 bar) |
| **Pressure chamber** | Smooths pressure |
| **Delivery hose** | Connects to lance |
| **Lance** | Directs spray |
| **Nozzle** | Atomizes liquid |
| **Cut-off valve** | On/off control |
| **Straps** | Carrying |

**Memory for function questions:**
- **Pressure chamber = Smooth pressure** (NOT storage!)
- **Nozzle = Atomization** (NOT pressure chamber!)

---

## 📊 Comparison Tables

### Sprayer Types

| Type | Capacity | Pressure | Coverage | Cost | Labor |
|------|----------|----------|----------|------|-------|
| **Manual knapsack** | 10-20 L | 2-4 bar | 0.3 ha/h | Low | High |
| **Motorized knapsack** | 10-20 L | 8-15 bar | 0.5 ha/h | Medium | Medium |
| **Power sprayer** | 50-500 L | 8-30 bar | 1-3 ha/h | High | Low |
| **Boom sprayer** | 200-1000 L | 2-5 bar | 3-8 ha/h | Very high | Very low |

---

### Spraying vs Dusting

| Aspect | Spraying | Dusting |
|--------|----------|---------|
| **Form** | Liquid | Powder |
| **Coverage** | Excellent | Fair |
| **Drift** | Lower | Higher |
| **Water** | Needed | Not needed |
| **Uniformity** | Good | Poor |
| **Safety** | Better | Worse (inhalation) |
| **Trend** | Increasing | Declining |

**Memory:** **"Spray is Superior"**

---

## 💡 Problem-Solving Strategy

### For Application Rate:
1. Identify: Q (L/min), W (m), S (km/h)
2. Apply: Rate = Q×600/(W×S)
3. Check units carefully

### For Calibration:
1. Volume used ÷ Area (m²)
2. Multiply by 10,000
3. Or: Volume × 100 (for 100 m² area)

### For Nozzle Discharge:
1. Use Q = K√P
2. If K unknown, use ratio: Q₂/Q₁ = √(P₂/P₁)

### For Concentration:
1. Chemical = (% × Total)/100
2. Water = Total - Chemical

### For Drift Analysis:
1. Smaller droplet → Higher drift
2. Check wind speed
3. Terminal velocity ∝ d²

---

## ⚠️ Common Mistakes to Avoid

### ❌ Don't:
- Confuse Q (flow rate) with application rate
- Forget to convert cm to m
- Mix up nozzle types (hollow cone for herbicide)
- Use wrong formula constant (600 not 60)
- Ignore pressure when calculating discharge
- Forget unit conversions (km/h to m/s)

### ✅ Do:
- Check all units match formula
- Remember: Q = K√P (not linear!)
- Know droplet size ranges
- Match nozzle to chemical type
- Consider drift in all calculations

---

## 🔢 Important Constants

| Constant | Value | Unit |
|----------|-------|------|
| **π** | 3.14159 | - |
| **g** | 9.81 or 10 | m/s² |
| **Water density** | 1000 | kg/m³ |
| **Air density** | 1.2 | kg/m³ |
| **Air viscosity** | 1.8×10⁻⁵ | Pa·s |
| **1 hectare** | 10,000 | m² |
| **Conversion (rate)** | 600 | Formula constant |

---

## 📝 Pre-Exam Checklist

### Must Remember:
- [ ] Application rate: Q×600/(W×S)
- [ ] Nozzle discharge: Q = K√P
- [ ] Calibration: Volume/Area × 10000
- [ ] Hollow cone = Insecticides, Flat fan = Herbicides
- [ ] Piston pump = High pressure
- [ ] Droplet size: Smaller = More drift
- [ ] Pressure chamber = Smooth pressure
- [ ] Boom height: h = W/(2tan(θ/2))

### Quick Facts:
- Knapsack: 2-4 bar, 10-20 L
- Power sprayer: 8-30 bar
- Boom sprayer: 2-5 bar, 200-1000 L
- Acceptable drift: <100 μm high risk
- Wind: <10 km/h okay, >15 avoid
- WHO Class II = Yellow = Moderately toxic

---

## 🎯 Exam Strategy

### Time Management:
- **1 mark:** 1-2 minutes (concept/selection)
- **2 marks:** 3-4 minutes (calculation)
- Component ID: 30-60 seconds

### High Weightage Topics:
1. Nozzle types and selection (★★★)
2. Application rate calculation (★★★)
3. Calibration methods (★★★)
4. Pump types (★★)
5. Drift factors (★★)
6. Safety/PPE (★)

### Quick Win Topics:
- Nozzle color coding (easy 1 mark)
- Pump type for application (1 mark)
- Component functions (1 mark)
- WHO toxicity classification (1 mark)

---

## 🧠 Memory Hooks

### Nozzle Selection:
**"Hollow for Hunting (insects), Flat for Fields (weeds)"**

### Application Rate:
**"Q-six-hundred over Width-Speed"**

### Drift Priority:
**"Big Droplets Beat Everything"**

### Pressure Chamber:
**"Smooth Pressure, Not Storage"**

### PPE for Class II:
**"Cover-Gloves-Boots-Goggles-Respirator-Hat"**

### Boom Height:
**"Width over 2-tan-half"**

---

## 🔗 Related Topics

- [Detailed Theory](./README.md)
- [PYQ Solutions](./Solutions.md)
- [Farm Machinery Overview](../README.md)
- [Harvesting Equipment](../Harvesting_Threshing/)

---

**Quick Reference Version 1.0**  
**Last Updated:** November 2025  
**Topics Covered:** Sprayers, Nozzles, Pumps, Dusters, Calibration, Safety  
**For:** GATE Agricultural Engineering

---

*Print this for last-minute revision!*  
*Master these formulas and specifications for guaranteed marks in plant protection questions.*

🌿 **Spray Wisely, Farm Safely!** 💚
