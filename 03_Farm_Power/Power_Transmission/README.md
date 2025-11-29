# ⚙️ Power Transmission in Tractors

> Comprehensive theory for GATE Agricultural Engineering

---

## 📑 Table of Contents

1. [Introduction](#introduction)
2. [Clutch](#clutch)
3. [Transmission/Gearbox](#transmission-gearbox)
4. [Differential](#differential)
5. [Final Drive](#final-drive)
6. [Power Take-Off (PTO)](#power-take-off-pto)
7. [Hydraulic System](#hydraulic-system)
8. [Three-Point Hitch](#three-point-hitch)

---

## 🎯 Introduction

### Power Transmission System

**Definition:** Mechanism to transmit engine power to drive wheels and implement

**Path:**
```
Engine → Clutch → Gearbox → Differential → Final Drive → Wheels
              ↓
            PTO (for implements)
```

---

### Functions

1. **Transfer power** from engine to wheels
2. **Vary speed** and torque (gearbox)
3. **Disconnect** power (clutch)
4. **Change direction** (reverse gear)
5. **Distribute power** to wheels (differential)
6. **Operate implements** (PTO, hydraulics)

---

## 🔄 Clutch

### Purpose

**Engage/disengage** power between engine and gearbox

**When used:**
- Starting from rest
- Changing gears
- Stopping without turning off engine

---

### Types of Clutch

**1. Single Plate Clutch:**
- One friction disc
- Used in cars, light tractors
- Simpler design

**2. Multi-Plate Clutch:**
- **Multiple friction discs**
- **Most common in tractors**
- Higher torque capacity
- Compact design
- Smooth engagement

---

### Multi-Plate Clutch Components

**Main Parts:**

**1. Driving Member:**
- Connected to engine flywheel
- Outer plates (steel)
- Rotates with engine

**2. Driven Member:**
- Connected to gearbox input shaft
- Inner plates with friction lining
- Transfers torque to gearbox

**3. Pressure Plate:**
- Presses plates together
- Spring-loaded

**4. Release Bearing:**
- Releases pressure when clutch pressed

---

### Working Principle

**Engaged (Normal running):**
- Spring pressure pushes plates together
- Friction between plates
- Power transmitted: Engine → Gearbox

**Disengaged (Clutch pedal pressed):**
- Release bearing pushes pressure plate back
- Springs compressed
- Plates separate
- No power transmission

---

### Torque Transmission

**Torque capacity:**
$$
T = \mu \times F \times R_{mean} \times n \times 2
$$

Where:
- μ = Coefficient of friction (0.25-0.35)
- F = Axial force (N)
- $R_{mean}$ = Mean radius of friction surface (m)
- n = Number of friction surfaces
- For multi-plate: n = 2(N-1), where N = number of plates

---

**Key:** More plates → More friction surfaces → Higher torque capacity

---

### Clutch Maintenance

**Check:**
- Free play (20-30 mm at pedal)
- Smooth engagement
- No slippage under load

**Adjustments:**
- Pedal free play
- Release bearing clearance

---

## ⚙️ Transmission / Gearbox

### Purpose

**Vary speed and torque** to match load conditions

**Why needed:**
- Engine has limited rpm range (1500-2500)
- Field operations need different speeds (3-35 km/h)
- Heavy loads need high torque (low speed)
- Transport needs high speed (low torque)

---

### Speed-Torque Relationship

**Power constant:**
$$
P = T \times \omega
$$

At constant power:
- **Low gear:** Low speed, **High torque** (ploughing)
- **High gear:** High speed, **Low torque** (transport)

**Trade-off:** Speed ↑, Torque ↓ (and vice versa)

---

### Gear Ratio

**Definition:**
$$
\boxed{i = \frac{N_{input}}{N_{output}} = \frac{T_{output}}{T_{input}}}
$$

$$
= \frac{\text{Number of teeth on driven gear}}{\text{Number of teeth on driving gear}}
$$

---

**Example:**
- Driving gear (pinion): 20 teeth
- Driven gear: 40 teeth
- Gear ratio, i = 40/20 = 2:1

**Effect:**
- Output speed = Input / 2
- Output torque = Input × 2

---

### Types of Gearbox

**1. Sliding Mesh:**
- Gears slide on shaft to engage
- Difficult shifting
- **Obsolete** in modern tractors

**2. Constant Mesh:**
- Gears always in mesh
- Dog clutch engages
- Easier shifting

**3. Synchromesh:**
- Synchronizes speeds before engagement
- **Smoothest shifting**
- Used in modern tractors

---

### Tractor Gearbox Configuration

**Typical medium tractor:**
- **8-16 forward gears**
- **2-4 reverse gears**

**Arrangement:**
- Main gearbox: 4 gears (L1, L2, H1, H2)
- Range gearbox: 2-4 ranges (Slow, Medium, Fast)
- Total = Main × Range (e.g., 4 × 4 = 16 forward)

---

**Speed ranges (typical):**

| Gear | Speed (km/h) | Use |
|------|--------------|-----|
| **L1** | 2-4 | Heavy tillage (ploughing) |
| **L2** | 4-6 | Seeding, harrowing |
| **M1-M2** | 6-12 | Cultivation, light work |
| **H1-H2** | 12-20 | Transport (field) |
| **Road** | 20-35 | Road transport |

---

### Gear Train Calculation

**For compound gear train:**
$$
\boxed{i_{total} = i_1 \times i_2 \times i_3 \times ...}
$$

**Output speed:**
$$
N_{out} = \frac{N_{in}}{i_{total}}
$$

**Output torque:**
$$
T_{out} = T_{in} \times i_{total} \times \eta
$$
(η = efficiency, ~95% per gear pair)

---

## 🔀 Differential

### Purpose

**Allows wheels to rotate at different speeds** when turning

**Why needed:**
- Outer wheel travels longer path than inner wheel
- If wheels locked together → skidding, tire wear

---

### Location

- Between two rear wheels (2WD tractor)
- Also in front axle (4WD tractor)

---

### Working Principle

**Straight line:**
- Both wheels rotate at same speed
- Differential gears rotate with carrier (no spinning)

**Turning:**
- Outer wheel needs to go faster
- Inner wheel slows down
- Differential pinions rotate
- **Speed difference accommodated**

**Formula:**
$$
N_{carrier} = \frac{N_{left} + N_{right}}{2}
$$

---

### Components

**1. Crown Wheel (Ring Gear):**
- Large gear, driven by propeller shaft pinion
- Typically 40-60 teeth

**2. Bevel Pinion:**
- Small gear on propeller shaft
- Typically 10-15 teeth

**3. Differential Pinions (Spider Gears):**
- Small gears on carrier (2 or 4)
- Mesh with side gears

**4. Side Gears:**
- Connected to axle shafts (left and right)
- Driven by pinions

---

### Final Drive Gear Ratio

$$
i_{FD} = \frac{\text{Crown wheel teeth}}{\text{Pinion teeth}}
$$

**Typical:** 4:1 to 6:1

**Example:**
- Crown wheel: 50 teeth
- Pinion: 10 teeth
- Ratio = 50/10 = 5:1

**Effect:** Propeller shaft rotates 5× faster than wheels

---

### Differential Lock

**Problem:** On slippery soil
- One wheel spins (low traction)
- Other wheel stationary
- Tractor stuck!

**Solution: Differential Lock**
- Locks both wheels together
- Both rotate at same speed
- Better traction in mud, sand

**Usage:** Engage only when stuck, disengage for turns

---

## 🔩 Final Drive

### Purpose

**Further reduce speed, increase torque** before wheels

**Types:**

**1. Spur Gear Type:**
- Simple, compact
- Common in medium tractors

**2. Planetary Gear Type:**
- More compact
- Higher reduction
- Used in heavy tractors

---

### Total Speed Reduction

**From engine to wheels:**
$$
i_{total} = i_{gearbox} \times i_{final\ drive} \times i_{differential}
$$

**Example:**
- Gearbox: 4:1
- Differential: 5:1
- Final drive: 3:1
- Total = 4 × 5 × 3 = 60:1

**Effect:**
- Engine: 2000 rpm
- Wheels: 2000 / 60 = 33.3 rpm

---

### Wheel Speed and Tractor Speed

**Wheel rpm to tractor speed:**
$$
V = \frac{\pi D N}{60000} \text{ km/h}
$$

Where:
- D = Wheel diameter (mm)
- N = Wheel rpm

**Or:**
$$
V = \pi D N \times 60 \text{ (D in m, V in m/min)}
$$

---

## 🔗 Power Take-Off (PTO)

### Definition

**Rotating shaft** at rear of tractor to operate machinery

---

### Purpose

**Transmit power** from engine to:
- Rotary tillers
- Threshers
- Pumps
- Mowers
- Balers
- Sprayers

---

### PTO Types

**By Engagement:**

**1. Transmission PTO:**
- Driven from gearbox
- Stops when clutch pressed
- **Common in older tractors**

**2. Independent/Live PTO:**
- Separate clutch for PTO
- **Continues running even when tractor clutch pressed**
- **Standard in modern tractors**
- Better for stationary work

---

### Standard PTO Speeds

**Two standards:**

**1. Type I (1000 rpm):**
- Shaft diameter: 1-3/8 inch (35 mm)
- 6 splines
- High-power implements

**2. Type II (540 rpm):**
- Shaft diameter: 1-3/8 inch
- 6 or 21 splines
- **Most common**

**Memory:** **540 rpm** is standard for most implements

---

### PTO Power

**Relationship with engine power:**
$$
\text{PTO Power} = 0.80 \text{ to } 0.85 \times \text{Engine Power}
$$

**Example:**
- 50 HP tractor
- PTO power ≈ 40-42.5 HP

**Losses (~15-20%):**
- Gears
- Bearings
- Clutch friction

---

### PTO Speed Calculation

**From engine speed:**
$$
N_{PTO} = \frac{N_{engine}}{i_{PTO}}
$$

**Typical PTO gear ratio:**
- For 540 rpm: ~4:1 (engine 2000-2200 rpm)
- For 1000 rpm: ~2:1

---

### PTO Torque

**At constant power:**
$$
T_{PTO} = \frac{P_{PTO} \times 9550}{N_{PTO}}
$$

**Or:**
$$
P_{PTO} = \frac{2\pi N_{PTO} T_{PTO}}{60000}
$$

---

### PTO Safety

**Dangers:**
- Rotating shaft can catch clothing
- High torque
- Unguarded shaft = extreme hazard

**Safety measures:**
- **Always use PTO guard**
- Keep away when running
- Disengage before servicing

---

## 🔧 Hydraulic System

### Purpose

**Lift and control implements** using hydraulic power

---

### Components

**1. Hydraulic Pump:**
- **Function:** Generate hydraulic pressure
- **Type:** Gear pump or piston pump
- **Drive:** From engine (gear or belt)
- **Pressure:** 140-180 bar (typical)
- **Flow rate:** 20-40 L/min

---

**2. Control Valve:**
- **Function:** Direct oil flow
- **Positions:** 
  - Raise (lift)
  - Hold (neutral)
  - Lower
  - Float (for scraping)

---

**3. Hydraulic Cylinder:**
- **Function:** Convert hydraulic pressure to mechanical force
- **Type:** Double-acting (can push and pull)
- **Stroke:** 400-600 mm (typical)

**Force:**
$$
F = P \times A
$$
- P = Pressure (Pa)
- A = Piston area (m²)

**Example:**
- Pressure: 150 bar = 15 MPa = 15 × 10⁶ Pa
- Piston diameter: 80 mm, Area = 0.005 m²
- Force = 15 × 10⁶ × 0.005 = 75,000 N = 75 kN

---

**4. Oil Reservoir:**
- Stores hydraulic oil
- Capacity: 30-60 liters

**5. Oil Filter:**
- Removes particles
- Essential for pump and valve life

---

### Hydraulic Lift Capacity

**Typical lifting capacity:**
- Small tractor: 800-1200 kg
- Medium tractor: 1500-2500 kg
- Large tractor: >3000 kg

**Measured at:** 610 mm behind hitch points (standard)

---

### Types of Hitch Control

**1. Position Control:**
- Maintains implement at set height
- For operations needing constant depth (ploughing)

**2. Draft Control:**
- Senses load on implement
- Adjusts depth automatically
- Maintains constant draft force

**3. Float Position:**
- Allows implement to follow ground contour
- For scrapers, blades

---

### Hydraulic Remote Outlets

**External hydraulic power:**
- For front-end loaders
- For hydraulic motors on implements
- Typically 1-3 remote outlets (SCVs)

---

## 🔺 Three-Point Hitch

### Definition

**Standard implement attachment system** using three links

---

### Components

**1. Two Lower Links:**
- Attach to implement lower ends
- Adjustable length
- Lift arms connected to hydraulic cylinder

**2. One Top Link:**
- Connects to implement top
- Adjustable length
- Controls pitch angle

---

### Categories (Based on Tractor Size)

| Category | Tractor HP | Pin Diameter |
|----------|------------|--------------|
| **Category I** | 20-45 HP | 22-25 mm |
| **Category II** | 40-100 HP | 28-32 mm |
| **Category III** | >80 HP | 37-45 mm |

**Memory:** Bigger tractor → Higher category → Larger pins

---

### Advantages

**Why 3-point hitch:**
- ✅ Quick attach/detach
- ✅ Standardized (universal)
- ✅ Hydraulic lift
- ✅ Good depth control
- ✅ Weight transfer to tractor (better traction)

---

### Implement Attachment

**Steps:**
1. Back tractor to implement
2. Attach lower links (both sides)
3. Attach top link
4. Adjust top link for correct pitch
5. Raise to transport height

---

### Check Chains (Stabilizers)

**Purpose:**
- Prevent side-swaying of implement
- Especially needed for offset implements

**Adjustment:**
- Tight: Rigid (for transport)
- Loose: Allow some movement (for field work)

---

## 🚜 Drawbar

### Definition

**Rigid or swinging bar** at rear for pulling trailed implements

---

### Types

**1. Fixed Drawbar:**
- Rigid attachment
- For straight-line pulling

**2. Swinging Drawbar:**
- Can pivot side-to-side
- Better for turns
- **More common**

---

### Drawbar Height

**Standard:** 400-500 mm from ground

**Importance:**
- Correct height → horizontal pull
- Too high → Rear wheels lift (dangerous!)
- Too low → Implement digs in

---

### Drawbar Power

**Already covered earlier:**
$$
DBP = \frac{P \times V}{3.6} \text{ (kW)}
$$

---

## 📊 Power Flow Summary

### From Engine to Wheels (2WD)

```
Engine (100%)
  ↓
Clutch (loss ~2%)
  ↓
Gearbox (loss ~5%)
  ↓
Differential (loss ~3%)
  ↓
Final Drive (loss ~3%)
  ↓
Wheels (Drive) (~87%)
  ↓ Slippage (8-15%)
  ↓ Rolling resistance
Drawbar Power (55-75%)
```

---

### To PTO

```
Engine (100%)
  ↓
PTO Gears (loss ~15-20%)
  ↓
PTO Shaft (80-85%)
```

**Note:** PTO more efficient than drawbar (fewer losses)

---

## 🔧 Maintenance

### Daily Checks
- Hydraulic oil level
- Leaks
- PTO guard in place

### Weekly/50 Hours
- Check gear oil level (gearbox, differential)
- Grease PTO shaft
- Check hitch linkages

### 250-500 Hours
- Change gearbox oil
- Change hydraulic filter
- Adjust clutch
- Check tire pressure

---

## 🎯 Key Points for GATE

**High Priority:**
- ✓ Gear ratio calculation
- ✓ PTO speed (540/1000 rpm)
- ✓ PTO power (80-85% of engine)
- ✓ Differential purpose and working
- ✓ Clutch types (single/multi-plate)
- ✓ 3-point hitch categories
- ✓ Hydraulic lift capacity
- ✓ Speed-torque trade-off

**Moderate Priority:**
- Gearbox types
- Differential lock
- Hydraulic pressure (140-180 bar)
- Drawbar types

**Formulas:**
- Gear ratio: i = N_in / N_out
- PTO power: 0.80-0.85 × Engine power
- Hydraulic force: F = P × A
- Wheel speed: V = πDN/60000

---

## 📈 Typical Specifications

**Medium Tractor (40-45 HP):**
- Clutch: Multi-plate, dry
- Gears: 8-12 forward, 2-4 reverse
- Differential: Bevel gear, 5:1 ratio
- PTO: 540 rpm (standard), independent
- Hydraulic lift: 1500-2000 kg
- Hitch: Category I
- Drawbar: Swinging type

---

## 🔗 Related Topics

- [Sources of Power](../Sources_of_Power/README.md)
- [Tractor Systems](../Tractor_Systems/README.md)
- [Solutions - PYQs](./Solutions.md)
- [Quick Reference](./CheatSheet.md)

---

**Last Updated:** November 2025  
**Next:** Practice with PYQ Solutions!

---

*Understanding power transmission is key to tractor operation!*

⚙️ **Keep Learning!** 🚜
