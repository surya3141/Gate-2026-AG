# 🚜 Tractor Systems - Quick Reference CheatSheet

> Last-minute revision for GATE Agricultural Engineering

---

## 🔢 Critical Power Formulas

### Brake Power (BP)
$$
\boxed{\text{BP (kW)} = \frac{2\pi NT}{60000} = \frac{NT}{9550}}
$$

- N = Engine speed (rpm)
- T = Torque (N·m)

**Memory:** **Divide (N × T) by 9550**

---

### Indicated & Friction Power
$$
\boxed{\text{FP} = \text{IP} - \text{BP}}
$$

- IP = Power inside cylinder
- BP = Power at crankshaft
- FP = Lost to friction

---

### Drawbar Power
$$
\boxed{\text{DBP (kW)} = \frac{P \times V}{3.6}}
$$

- P = Pull (kN)
- V = Speed (km/h)

**SI form:**
$$
DBP = F \times v \text{ (F in N, v in m/s)}
$$

---

## 📈 Efficiency Formulas

### Mechanical Efficiency
$$
\boxed{\eta_m = \frac{\text{BP}}{\text{IP}} \times 100\%}
$$

**Typical:** 75-85%

---

### Brake Thermal Efficiency
$$
\boxed{\eta_{bth} = \frac{\text{BP} \times 3600}{\dot{m}_f \times CV} \times 100\%}
$$

- BP in kW
- $\dot{m}_f$ in kg/h
- CV in kJ/kg

**Or using SFC:**
$$
\eta_{bth} = \frac{3600}{SFC \times CV} \times 100\%
$$

**Typical:**
- Diesel: **30-40%**
- Petrol: 25-30%

---

### Tractive Efficiency
$$
\boxed{\eta_t = \frac{\text{DBP}}{\text{BP}} \times 100\%}
$$

**Typical:** 55-75%

---

### Volumetric Efficiency
$$
\boxed{\eta_v = \frac{\text{Actual air intake}}{\text{Swept volume}} \times 100\%}
$$

**Typical:** 80-90%

---

## ⛽ Fuel Consumption

### Specific Fuel Consumption (SFC)
$$
\boxed{\text{SFC} = \frac{m_f}{\text{BP} \times t} \text{ (g/kWh)}}
$$

**Or:**
$$
\text{SFC} = \frac{\text{Fuel rate (kg/h)}}{\text{BP (kW)}} \times 1000
$$

---

### Standard Values (MEMORIZE!)

| Engine Type | SFC (g/kWh) |
|-------------|-------------|
| **Diesel** | **200-250** ⭐ |
| **Petrol** | 280-320 |

**Memory:** **"Diesel ≈ 225"** (midpoint)

---

## ⚙️ Engine Fundamentals

### Compression Ratio
$$
\boxed{r = \frac{V_s + V_c}{V_c}}
$$

- $V_s$ = Swept volume
- $V_c$ = Clearance volume

---

**Standard Values:**

| Engine | Compression Ratio |
|--------|-------------------|
| **Diesel** | **16:1 to 22:1** |
| **Petrol** | 8:1 to 12:1 |

**Memory:** **"Diesel doubles petrol"**

---

### Displacement Volume
$$
\boxed{V_s = \frac{\pi D^2}{4} \times L \times n}
$$

- D = Bore (m)
- L = Stroke (m)
- n = Number of cylinders

**Units:** Usually in liters (L) or cc

---

### 4-Stroke Cycle

**4 strokes = 2 revolutions**

1. **Suction** (down)
2. **Compression** (up)
3. **Power** (down) ← Work here
4. **Exhaust** (up)

**Power stroke:** Once per 2 revolutions

---

## 🎯 Tractor Performance

### Wheel Slip
$$
\boxed{\text{Slip (\%)} = \frac{d_t - d_a}{d_t} \times 100}
$$

**Or (using revolutions):**
$$
Slip = \left(1 - \frac{N_t}{N_a}\right) \times 100
$$

- $N_t$ = No-load revolutions
- $N_a$ = Loaded revolutions

---

**Optimal Slip:** **8-15%** ⭐

| Slip | Status |
|------|--------|
| <8% | Under-utilized, low pull |
| **8-15%** | **Optimal** ✓ |
| >15% | Excessive, high fuel loss |
| >20% | Poor traction, add ballast |

---

### Traction Coefficient
$$
\mu_t = \frac{\text{Drawbar pull}}{\text{Weight on drive wheels}}
$$

**Typical:** 0.4-0.7

---

### Rolling Resistance
$$
R_r = \mu_r \times W
$$

**Coefficient ($\mu_r$) values:**

| Surface | $\mu_r$ |
|---------|---------|
| **Concrete** | 0.02-0.03 |
| **Firm soil** | 0.08-0.12 |
| **Soft soil** | 0.15-0.25 |

---

## 🔧 Engine Specifications (Typical 40 HP Tractor)

| Parameter | Value |
|-----------|-------|
| **Cylinders** | 3-4 |
| **Type** | 4-stroke diesel |
| **Displacement** | 2.5-3.5 L |
| **Compression ratio** | 17:1 to 19:1 |
| **Rated speed** | 2000-2200 rpm |
| **Max torque** | ~160-200 N·m |
| **SFC** | 210-230 g/kWh |
| **Cooling** | Liquid (water) |

---

## 💧 Cooling System

### Components & Functions

| Component | Function | Detail |
|-----------|----------|--------|
| **Radiator** | Cools water | 15-25 L capacity |
| **Water pump** | Circulates | Centrifugal, belt-driven |
| **Thermostat** | Controls temp | Opens at 80-85°C |
| **Fan** | Air flow | Belt or electric |
| **Coolant** | Heat transfer | 50% water + 50% antifreeze |

---

### Thermostat Operation

**Cold engine (<80°C):**
- Valve closed
- Coolant bypasses radiator
- Fast warm-up

**Hot engine (>80°C):**
- Valve opens
- Coolant flows through radiator
- Normal cooling

**Memory:** **"80°C opens"**

---

### Pressurized System

**Radiator cap:** 0.5-1.0 bar

**Effect:** Raises boiling point
- Unpressurized: 100°C
- Pressurized (0.7 bar): ~110-115°C

**Benefit:** Higher operating temperature → better efficiency

---

## 🛢️ Lubrication System

### Oil Functions (5 main)

1. **Reduce friction**
2. **Cool** components
3. **Seal** piston rings
4. **Clean** (suspends particles)
5. **Protect** against corrosion

**Memory:** **"FRCSP"** (Friction, Reduce, Cool, Seal, Protect)

---

### Components

| Component | Function |
|-----------|----------|
| **Sump** | Oil reservoir (10-20 L) |
| **Oil pump** | Circulates (2-4 bar) |
| **Oil filter** | Removes particles |
| **Oil cooler** | Cools oil (if fitted) |

---

### Oil Specifications

**Viscosity Grade:**
- **SAE 15W-40** (most common)
- SAE 20W-50 (hot climates)

**Quality:**
- API CF, CF-4, CI-4 (diesel)

**Change interval:** 150-250 hours

---

## ⚡ Electrical System

### Key Components

| Component | Voltage | Function |
|-----------|---------|----------|
| **Battery** | 12V | Energy storage (60-100 Ah) |
| **Alternator** | 12V | Generates, charges (35-70 A) |
| **Starter motor** | 12V | Cranks engine (2-3 kW) |
| **Lights** | 12V | Illumination |

---

### Battery

**Type:** Lead-acid, 12V

**Cells:** 6 cells × 2V = 12V

**Capacity:** 60-100 Ah

**Voltage status:**
- Fully charged: 12.6-12.8V
- 50% charged: 12.2V
- Discharged: <12V

---

## 🚜 Tractor Power Forms

### Three Outputs

**1. Drawbar Power (DBP):**
- For pulling implements
- **Efficiency:** 60-75% of engine power

**2. PTO Power:**
- For operating machines
- **Efficiency:** 80-85% of engine power

**3. Belt Power:**
- Rarely used now
- For stationary work

**Memory:** **"PTO > Drawbar"** (less losses)

---

### PTO Speeds (Standard)

- **540 rpm** (Type I) - Common
- **1000 rpm** (Type II) - High-power

---

## 🧮 Quick Calculation Tricks

### BP from Torque (Fast!)

**Given:** N = 2000 rpm, T = 150 N·m

**Formula:** BP = NT/9550

$$
BP = \frac{2000 \times 150}{9550} = \frac{300,\!000}{9550} ≈ 31.4 \text{ kW}
$$

**Trick:** Multiply N × T, divide by ~10,000 (rough estimate)

---

### Compression Ratio (Quick)

**Given:** Swept = 500 cc, Clearance = 25 cc

$$
r = \frac{500 + 25}{25} = \frac{525}{25} = 21
$$

**Trick:** Add both, divide by clearance

---

### DBP (Fast!)

**Given:** Pull = 6 kN, Speed = 6 km/h

$$
DBP = \frac{6 \times 6}{3.6} = \frac{36}{3.6} = 10 \text{ kW}
$$

**Trick:** (P × V) ÷ 3.6

---

## 📊 Comparison Tables

### Diesel vs Petrol Engine

| Parameter | Diesel | Petrol |
|-----------|--------|--------|
| **Compression ratio** | 16-22:1 | 8-12:1 |
| **Ignition** | Auto (heat) | Spark plug |
| **Efficiency** | 30-40% | 25-30% |
| **SFC** | 200-250 g/kWh | 280-320 g/kWh |
| **Fuel injection** | Yes | Carburetor/injection |
| **Torque** | High at low rpm | Peak at higher rpm |
| **Use in tractor** | ✓ Common | ✗ Rare |

---

### Power Efficiency Cascade

**Engine Power (100%):**
- ↓ Friction loss (15-25%)
- **= Brake Power (75-85%)**
- ↓ Transmission loss (5-10%)
- ↓ Slip + rolling resistance (10-15%)
- **= Drawbar Power (55-75%)**

---

## ⚠️ Common Exam Mistakes

### Mistake 1: Power Formula
❌ Using 60 instead of 60000  
✅ **BP = 2πNT / 60000 (kW)**

---

### Mistake 2: Slip Direction
❌ Thinking fewer revolutions = slip  
✅ **More revolutions under load = positive slip**

---

### Mistake 3: 4-Stroke Cycle
❌ 4 revolutions  
✅ **2 revolutions** per cycle

---

### Mistake 4: SFC Units
❌ kg/kWh  
✅ **g/kWh** (1000× smaller)

---

### Mistake 5: DBP Units
❌ Using m/s speed  
✅ **Formula needs km/h:** DBP = PV/3.6

---

### Mistake 6: Typical Values
❌ Not remembering ranges  
✅ Know: SFC 200-250, η_bth 30-40%, slip 8-15%

---

## 🎓 Memory Techniques

### "9550 Power"
**BP (kW) = NT / 9550**  
Memory: "Nine-five-five-O for power"

---

### "3.6 Drawbar"
**DBP = PV / 3.6**  
Memory: "Three-point-six converts"

---

### "225 SFC"
**Diesel SFC ≈ 225 g/kWh** (midpoint 200-250)

---

### "80 Thermostat"
**Opens at 80-85°C**

---

### "12% Slip Optimal"
**Target: 8-15%, center = 12%**

---

### "2 for 4"
**4-stroke = 2 revolutions**

---

### "75-85 Mechanical"
**Mechanical efficiency: 75-85%**

---

## 📋 Pre-Exam Checklist

**Must Remember:**
- [ ] **BP = NT / 9550** (in kW)
- [ ] **DBP = PV / 3.6** (P in kN, V in km/h)
- [ ] **SFC:** Diesel 200-250 g/kWh
- [ ] **η_m = BP/IP × 100%**
- [ ] **η_t = DBP/BP × 100%**
- [ ] **η_bth:** Diesel 30-40%
- [ ] **Compression ratio:** Diesel 16-22:1
- [ ] **4-stroke:** 2 revolutions
- [ ] **Slip:** Optimal 8-15%
- [ ] **Thermostat:** Opens at 80-85°C

---

## 🔥 High-Yield Topics

**Must Know (Every GATE):**
1. ✓ BP calculation from torque ⭐⭐⭐
2. ✓ Efficiency formulas (mechanical, thermal) ⭐⭐⭐
3. ✓ SFC typical values ⭐⭐
4. ✓ Compression ratio ⭐⭐
5. ✓ Drawbar power ⭐⭐
6. ✓ Tractive efficiency ⭐⭐

**Moderate Priority:**
- Slip calculation
- Displacement volume
- 4-stroke cycle
- Cooling/lubrication basics

**Lower Priority:**
- Detailed component descriptions
- Historical data
- Maintenance schedules

---

## 💡 Last-Minute Tips

**If short on time, FOCUS ON:**
1. ✓ Power formulas (BP, DBP)
2. ✓ Efficiency definitions
3. ✓ Standard values (SFC, compression ratio)
4. ✓ 4-stroke cycle basics
5. ✓ Slip optimal range

**Can skip:**
- Detailed lubrication paths
- Electrical system specifics
- Component materials

---

## 🎯 Final Formula Card

**Top 6 - Commit to Memory:**

$$
\boxed{BP = \frac{NT}{9550} \text{ kW}}
$$

$$
\boxed{DBP = \frac{P \times V}{3.6} \text{ kW}}
$$

$$
\boxed{\eta_m = \frac{BP}{IP} \times 100\%}
$$

$$
\boxed{\eta_t = \frac{DBP}{BP} \times 100\%}
$$

$$
\boxed{r = \frac{V_s + V_c}{V_c}}
$$

$$
\boxed{Slip = \left(1 - \frac{N_t}{N_a}\right) \times 100}
$$

---

## 📱 Quick Reference Card

**Write on exam rough sheet:**

```
BP = NT/9550 kW
DBP = PV/3.6 kW
η_m = BP/IP × 100%
η_t = DBP/BP × 100%
SFC diesel: 200-250 g/kWh
η_bth diesel: 30-40%
Compression diesel: 16-22:1
4-stroke = 2 revolutions
Slip optimal: 8-15%
Thermostat: 80°C
```

---

**Last Updated:** November 2025  
**Exam Ready!** ✓

---

## 🔗 Navigation

- [Detailed Theory](./README.md)
- [PYQ Solutions](./Solutions.md)
- [Back to Farm Power](../README.md)

---

*Quick, focused, exam-ready! All the best! 🎯*

🚜 **Tractor Your Way to Success!** 🏆
