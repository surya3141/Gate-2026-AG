# ⚙️ Power Transmission - Quick Reference CheatSheet

> Last-minute revision for GATE Agricultural Engineering

---

## 🔢 Critical Formulas

### Gear Ratio
$$
\boxed{i = \frac{T_{driven}}{T_{driving}} = \frac{N_{input}}{N_{output}}}
$$

**Effect:**
$$
N_{out} = \frac{N_{in}}{i}; \quad T_{out} = T_{in} \times i \times \eta
$$

---

### Compound Gear Train
$$
\boxed{i_{total} = i_1 \times i_2 \times i_3 \times ...}
$$

**Memory:** **Multiply** individual ratios

---

### PTO Power
$$
\boxed{P_{PTO} = 0.80 \text{ to } 0.85 \times P_{engine}}
$$

**Memory:** **"80-85% for PTO"**

---

### PTO Torque
$$
\boxed{T = \frac{P \times 9550}{N}}
$$

- P in kW
- N in rpm
- T in N·m

---

### Hydraulic Force
$$
\boxed{F = P \times A}
$$

**Piston area:**
$$
A = \frac{\pi D^2}{4}
$$

---

### Wheel Speed
$$
\boxed{V = \frac{\pi D N}{60000} \text{ km/h}}
$$

- D in mm
- N in rpm

**Or (D in meters):**
$$
V = \frac{\pi D N \times 60}{1000} \text{ km/h}
$$

---

## 🔄 Clutch - Quick Facts

### Types

| Type | Features | Use |
|------|----------|-----|
| **Single plate** | 1 disc, simple | Cars, light tractors |
| **Multi-plate** | Multiple discs | **Tractors (most common)** ⭐ |

---

### Multi-Plate Advantages
- ✓ Higher torque capacity
- ✓ Compact design
- ✓ Smooth engagement
- ✓ Longer life

**Friction surfaces:** n = 2(N-1), where N = number of plates

---

### Clutch Free Play
**Standard:** 20-30 mm at pedal

---

## ⚙️ Gearbox - Quick Facts

### Purpose
**Vary speed and torque** to match load

**Trade-off:**
- Low gear: Low speed, **High torque**
- High gear: High speed, **Low torque**

---

### Typical Tractor Gears
- **Forward:** 8-16 gears
- **Reverse:** 2-4 gears

---

### Speed Ranges

| Gear | Speed (km/h) | Application |
|------|--------------|-------------|
| **L1** | 2-4 | Heavy tillage (ploughing) |
| **L2** | 4-6 | Seeding, harrowing |
| **M1-M2** | 6-12 | Cultivation |
| **H1-H2** | 12-20 | Field transport |
| **Road** | 20-35 | Road transport |

---

### Gearbox Types
1. **Sliding mesh** (obsolete)
2. **Constant mesh** (common)
3. **Synchromesh** (modern, smooth)

---

## 🔀 Differential - Quick Facts

### Primary Function
**Allow wheels to rotate at different speeds** during turns

**Formula:**
$$
\boxed{N_{carrier} = \frac{N_{left} + N_{right}}{2}}
$$

---

### Final Drive Ratio
$$
i_{FD} = \frac{\text{Crown wheel teeth}}{\text{Pinion teeth}}
$$

**Typical:** **4:1 to 6:1** ⭐

**Example:**
- Crown wheel: 50 teeth
- Pinion: 10 teeth
- Ratio = 50/10 = **5:1**

---

### Differential Lock
**Purpose:** Improve traction on slippery soil

**When to use:**
- ✓ Stuck in mud/sand
- ✗ **NOT during turns** (dangerous!)

**Effect:** Both wheels rotate at same speed

---

## 🔗 Power Take-Off (PTO)

### Standard Speeds

| Type | Speed (rpm) | Shaft Dia | Common Use |
|------|-------------|-----------|-----------|
| **Type I** | **1000** | 35 mm, 6 splines | High power |
| **Type II** | **540** ⭐ | 35 mm, 6/21 splines | **Most common** |

**Memory:** **"540 standard"**

---

### PTO Power
**Efficiency:** 80-85% of engine power

**Example:**
- 50 HP engine
- PTO power = 40-42.5 HP

---

### PTO Types (By Engagement)

**1. Transmission PTO:**
- Stops when clutch pressed
- Older tractors

**2. Independent/Live PTO:** ⭐
- Separate clutch
- **Continues when tractor clutch pressed**
- **Modern standard**

---

### PTO Torque Calculation
$$
T = \frac{P \times 9550}{N}
$$

**Quick example:**
- P = 30 kW, N = 540 rpm
- T = (30 × 9550) / 540 = **530 N·m**

---

## 🔧 Hydraulic System

### Components

| Component | Typical Value |
|-----------|---------------|
| **Pump** | Gear/piston type |
| **Pressure** | **140-180 bar** ⭐ |
| **Flow rate** | 20-40 L/min |
| **Oil capacity** | 30-60 L |
| **Cylinder stroke** | 400-600 mm |

---

### Hydraulic Force
$$
F = P \times A
$$

**Quick calculation (100 mm piston, 150 bar):**
- Area = π × 0.1² / 4 = 0.00785 m²
- P = 150 × 10⁵ Pa = 15 MPa
- F = 15 × 10⁶ × 0.00785 = **117.8 kN**

---

### Lift Capacity (Typical)

| Tractor Size | Lift Capacity |
|--------------|---------------|
| **Small** | 800-1200 kg |
| **Medium** | **1500-2500 kg** ⭐ |
| **Large** | >3000 kg |

**Measured at:** 610 mm behind hitch points

---

### Control Types
1. **Position control** - Constant depth (ploughing)
2. **Draft control** - Constant load
3. **Float** - Follow ground (scrapers)

---

## 🔺 Three-Point Hitch

### Categories

| Category | Tractor HP | Pin Diameter | Typical Use |
|----------|------------|--------------|-------------|
| **Cat 0** | <20 | Small | Garden tractors |
| **Cat I** | **20-45** | **22-25 mm** | **Small tractors** ⭐ |
| **Cat II** | 40-100 | 28-32 mm | Medium tractors |
| **Cat III** | >80 | 37-45 mm | Large tractors |

**Memory:** Higher category = Bigger tractor = Larger pins

---

### Components
1. **Two lower links** - Lift implement
2. **One top link** - Control pitch
3. **Check chains** - Prevent side sway

---

### Advantages
- ✓ Quick attach/detach
- ✓ Universal/standardized
- ✓ Hydraulic lift
- ✓ Weight transfer (better traction)

---

## 🚜 Drawbar

### Types
1. **Fixed drawbar** - Rigid
2. **Swinging drawbar** - Can pivot (more common)

**Standard height:** 400-500 mm from ground

---

## 📊 Power Flow Summary

### Engine to Wheels (Losses)

```
Engine Power (100%)
  ↓ -2% (Clutch)
  ↓ -5% (Gearbox)
  ↓ -3% (Differential)
  ↓ -3% (Final drive)
= ~87% at wheels
  ↓ -12% (Slip + rolling)
= Drawbar Power (55-75%)
```

---

### Engine to PTO (Losses)

```
Engine Power (100%)
  ↓ -15 to -20% (PTO gears)
= PTO Power (80-85%)
```

**Key:** **PTO more efficient than drawbar** ⭐

---

## 🧮 Quick Calculation Tricks

### Gear Ratio (Fast)

**Given:** 20T driving → 60T driven

$$
i = \frac{60}{20} = 3:1
$$

**Output speed:** Input / 3  
**Output torque:** Input × 3 (approx, ignore small losses)

---

### Compound Gears (Fast)

**Stage 1:** 2:1, **Stage 2:** 3:1

$$
Total = 2 \times 3 = 6:1
$$

---

### PTO Power (Fast)

**50 HP engine:**

$$
PTO ≈ 50 \times 0.82 = 41 \text{ HP (use 82% average)}
$$

---

### Hydraulic Force (Fast)

**100 mm piston, 150 bar:**

$$
Area ≈ 0.008 \text{ m}^2
$$
$$
F ≈ 150 \times 0.8 = 120 \text{ kN (rough)}
$$

---

### Wheel Speed (Rough)

**D = 1 m, N = 60 rpm:**

$$
V ≈ 3 \times 1 \times 60 \times 60/1000 ≈ 11 \text{ km/h}
$$

(Using π ≈ 3 for mental math)

---

## 📋 Standard Values (MEMORIZE!)

### PTO
- **Standard speed:** **540 rpm** (most common)
- **Alternative:** 1000 rpm
- **Power efficiency:** **80-85%**

---

### Hydraulic
- **Pressure:** **140-180 bar**
- **Medium tractor lift:** **1500-2500 kg**

---

### Differential
- **Final drive ratio:** **4:1 to 6:1**

---

### Hitch
- **Small tractor (20-45 HP):** **Category I**
- **Medium (40-100 HP):** Category II

---

### Gears
- **Forward gears:** 8-16
- **Reverse gears:** 2-4
- **Typical efficiency:** 95% per gear pair

---

## ⚠️ Common Exam Mistakes

### Mistake 1: Gear Ratio Direction
❌ Driving / Driven  
✅ **Driven / Driving**

---

### Mistake 2: Compound Gears
❌ Adding ratios (2:1 + 3:1 = 5:1)  
✅ **Multiplying** (2 × 3 = 6:1)

---

### Mistake 3: PTO Efficiency
❌ Using 60-75% (that's drawbar)  
✅ **80-85% for PTO**

---

### Mistake 4: Hydraulic Pressure
❌ Using bar directly in force calculation  
✅ **Convert to Pa:** 1 bar = 10⁵ Pa

---

### Mistake 5: Wheel Speed Formula
❌ V = πDN (missing /60000)  
✅ **V = πDN/60000** (D in mm)

---

### Mistake 6: Differential Function
❌ "Increases torque" as primary function  
✅ **"Allows different wheel speeds"** is primary

---

## 🎓 Memory Techniques

### "540 Standard"
**PTO:** 540 rpm is most common

---

### "80-85 PTO"
**PTO efficiency:** 80-85% of engine

---

### "5 to 1 Diff"
**Differential ratio:** Typically around 5:1

---

### "Cat I = 20-45"
**Hitch Category I:** 20-45 HP tractors

---

### "150 bar Hydraulic"
**Typical pressure:** Around 150 bar (140-180 range)

---

### "Multiply Compound"
**Compound gears:** Multiply individual ratios

---

## 🔥 High-Yield Topics

**Must Know (Frequent in GATE):**
1. ✓ Gear ratio calculations ⭐⭐⭐
2. ✓ PTO power (80-85%) ⭐⭐⭐
3. ✓ PTO standard speed (540 rpm) ⭐⭐
4. ✓ Hydraulic force calculation ⭐⭐
5. ✓ Differential function ⭐⭐
6. ✓ Hitch categories ⭐⭐

**Moderate Priority:**
- Compound gear trains
- Wheel speed calculation
- Clutch types
- Final drive ratio

**Lower Priority:**
- Detailed component descriptions
- Maintenance schedules
- Historical development

---

## 💡 Last-Minute Tips

**If short on time, FOCUS ON:**
1. ✓ Gear ratio formula (i = driven/driving)
2. ✓ Compound gear multiplication
3. ✓ PTO: 540 rpm, 80-85% power
4. ✓ Hydraulic: F = P × A
5. ✓ Differential: allows different speeds
6. ✓ Hitch: Cat I = 20-45 HP

**Can skip:**
- Gearbox construction details
- Clutch material specifications
- Hydraulic valve types

---

## 🎯 Final Formula Card

**Top 6 - Commit to Memory:**

$$
\boxed{i = \frac{T_{driven}}{T_{driving}} = \frac{N_{in}}{N_{out}}}
$$

$$
\boxed{i_{total} = i_1 \times i_2 \times i_3 ...}
$$

$$
\boxed{P_{PTO} = 0.80 \text{ to } 0.85 \times P_{engine}}
$$

$$
\boxed{T = \frac{P \times 9550}{N}}
$$

$$
\boxed{F = P \times A}
$$

$$
\boxed{V = \frac{\pi D N}{60000} \text{ km/h}}
$$

---

## 📱 Quick Reference Card

**Write on exam rough sheet:**

```
Gear: i = driven/driving
Compound: i_total = i1 × i2 × i3
PTO: 540 rpm, 80-85% power
T = P×9550/N
Hydraulic: F = P×A, 150 bar typical
Diff ratio: 4:1 to 6:1
Cat I: 20-45 HP
Wheel speed: V = πDN/60000
```

---

## 🔗 Power Transmission Path

**Remember the sequence:**

```
Engine
  ↓
Clutch (disconnect)
  ↓
Gearbox (speed/torque variation)
  ↓
Propeller shaft
  ↓
Differential (allows turn)
  ↓
Final drive (further reduction)
  ↓
Wheels

Side branch:
Gearbox → PTO (80-85% power, 540 rpm)
Gearbox → Hydraulic pump → 3-point hitch
```

---

## 📊 Comparison Tables

### PTO vs Drawbar

| Parameter | PTO | Drawbar |
|-----------|-----|---------|
| **Efficiency** | 80-85% | 60-75% |
| **Purpose** | Operate machines | Pull implements |
| **Standard** | 540/1000 rpm | Variable speed |
| **Losses** | Gears only | Gears + slip + rolling |

**Memory:** **"PTO wins efficiency"**

---

### Clutch Types

| Feature | Single Plate | Multi-Plate |
|---------|--------------|-------------|
| **Discs** | 1 | Multiple |
| **Torque capacity** | Lower | Higher |
| **Size** | Larger | Compact |
| **Use** | Cars | **Tractors** ⭐ |

---

### Hitch Categories (Summary)

| Cat | HP Range | Quick ID |
|-----|----------|----------|
| **I** | 20-45 | Small tractors |
| **II** | 40-100 | Medium |
| **III** | >80 | Large |

---

## 📋 Pre-Exam Checklist

**24 Hours Before:**
- [ ] **Gear ratio:** i = driven/driving
- [ ] **Compound:** Multiply ratios
- [ ] **PTO:** 540 rpm, 80-85% power
- [ ] **Torque:** T = P×9550/N
- [ ] **Hydraulic:** F = P×A, 150 bar
- [ ] **Differential:** Allows different speeds
- [ ] **Cat I:** 20-45 HP
- [ ] **Final drive:** 4:1 to 6:1

---

**1 Hour Before:**
- [ ] Solve 2-3 gear ratio problems
- [ ] Calculate PTO power (50 HP → ~42 HP)
- [ ] Hydraulic force (100mm, 150bar → 118kN)
- [ ] Review hitch categories
- [ ] Remember: PTO > Drawbar efficiency

---

## 📝 Expected Question Patterns

**1-Mark (1-2 questions):**
- PTO standard speed (540 rpm)
- Differential function
- Hitch category for given HP
- Clutch type (multi-plate)

**2-Mark (2-3 questions):**
- Gear ratio calculation
- Compound gear train
- PTO power/torque
- Hydraulic force
- Wheel speed

---

## 💡 Final Tips

**Time Management:**
- Easy (1 mark): 2 minutes
- Medium (2 marks): 3-4 minutes
- Hard multi-part: 5-6 minutes

**Strategy:**
- Solve gear ratios quickly
- Know standard values (540, 80-85%, 150 bar)
- Don't get stuck on multi-step problems

---

**Last Updated:** November 2025  
**Exam Ready!** ✓

---

## 🔗 Navigation

- [Detailed Theory](./README.md)
- [PYQ Solutions](./Solutions.md)
- [Back to Farm Power](../README.md)

---

*Quick, focused, exam-oriented! All the best! 🎯*

⚙️ **Transmit Your Knowledge to Success!** 🏆
