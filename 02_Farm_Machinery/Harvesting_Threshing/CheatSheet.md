# ⚡ Harvesting & Threshing Equipment - Quick Reference

> Essential formulas, specifications, and memory tricks for GATE AG

---

## 🔑 Key Formulas

### 1. Cylinder Speed

**Peripheral Speed:**
$$
V_c = \frac{\pi D N}{60} \text{ m/s}
$$

**Solving for RPM:**
$$
N = \frac{60 V_c}{\pi D}
$$

Where:
- V_c = Peripheral speed (m/s)
- D = Cylinder diameter (m)
- N = RPM

**Memory Trick:** **"V comes from Pi-D-N over 60"**

---

### 2. Knife/Cutter Bar Speed

**Knife Speed:**
$$
V_k = \frac{2 \times L \times N}{60} \text{ m/s}
$$

Where:
- L = Stroke length (m)
- N = Strokes per minute

**Standard:** 800-1200 spm for reapers

---

### 3. Reel Parameters

**Reel Index:**
$$
\text{Reel Index} = \frac{V_r}{V_f}
$$

**Reel Peripheral Speed:**
$$
V_r = \frac{\pi D_r N_r}{60}
$$

**Optimal Range:** 1.2 to 1.5

**Memory Trick:** **"Reel goes 1.2 to 1.5 times forward speed"**

---

### 4. Field Capacity

**Theoretical Field Capacity:**
$$
\text{TFC} = \frac{W \times S}{10} \text{ ha/h}
$$

**Effective Field Capacity:**
$$
\text{EFC} = \text{TFC} \times \eta_f
$$

**Field Efficiency:**
$$
\eta_f = \frac{\text{EFC}}{\text{TFC}} \times 100\%
$$

Where:
- W = Width (m)
- S = Speed (km/h)

**Quick Calc:** Multiply width by speed, divide by 10

---

### 5. Threshing Efficiency

$$
\eta_t = \frac{\text{Grain threshed}}{\text{Total grain}} \times 100\%
$$

**Or:**
$$
\eta_t = \left(1 - \frac{\text{Unthreshed grain}}{\text{Total grain}}\right) \times 100\%
$$

**Target:** > 99%

---

### 6. Cleaning Efficiency

$$
\eta_c = \frac{\text{Clean grain in tank}}{\text{Total grain threshed}} \times 100\%
$$

**Or:**
$$
\eta_c = \left(1 - \frac{\text{Chaff in grain}}{\text{Total sample}}\right) \times 100\%
$$

**Target:** > 98%

---

### 7. Loss Calculations

**Percentage Loss:**
$$
\text{Loss (\%)} = \frac{\text{Grain lost}}{\text{Total yield}} \times 100
$$

**Loss per hectare (from sample):**
$$
\text{Loss (kg/ha)} = \frac{\text{Weight in sample (kg)}}{\text{Sample area (ha)}}
$$

**For 1 m² sample:**
$$
\text{Loss (kg/ha)} = \text{Weight (kg)} \times 10000
$$

**Acceptable Limit:** < 2% total

---

### 8. Feed Rate

$$
Q_f = \text{EFC} \times \text{Crop yield/ha} \text{ (kg/h)}
$$

**For grain + straw:**
$$
Q_f = \text{EFC} \times \text{(Grain + Straw)/ha}
$$

---

## 📊 Standard Specifications

### Cylinder Specifications

| Parameter | Range | Typical |
|-----------|-------|---------|
| **Diameter** | 40-60 cm | 50 cm |
| **Length** | 60-100 cm | 80 cm |
| **RPM** | 500-1200 | 700-900 |
| **Peripheral Speed** | 10-25 m/s | Crop dependent |
| **Number of Bars** | 6-8 (rasp bar) | 6 |

---

### Crop-Specific Cylinder Speeds

| Crop | Speed (m/s) | RPM (D=50cm) | Type |
|------|-------------|--------------|------|
| **Wheat** | 18-25 | 700-950 | Rasp bar |
| **Rice** | 18-22 | 700-850 | Rasp bar |
| **Pulses** | 10-15 | 380-570 | Peg tooth |
| **Soybean** | 12-15 | 460-570 | Peg tooth |
| **Maize** | 6-10 | 230-380 | Spike tooth |

**Memory Trick:** **"Wheat Runs Fast (20), Pulses Plod (12), Maize Moves Slow (8)"**

---

### Concave Specifications

| Parameter | Entry | Exit |
|-----------|-------|------|
| **Clearance** | 25-30 mm | 10-15 mm |
| **Wire spacing** | 10-12 mm | 8-10 mm |
| **Length** | 50-80 cm | - |
| **Angle** | 120-140° | - |

**Memory:** **"Entry 30, Exit 15 - Half the space for final grind"**

---

### Reaper Specifications

| Component | Specification |
|-----------|---------------|
| **Cutting width** | 1.2-1.8 m |
| **Cutter bar speed** | 800-1200 spm |
| **Stroke length** | 75-100 mm |
| **Reel diameter** | 60-90 cm |
| **Reel speed** | 30-60 rpm |
| **Forward speed** | 2-4 km/h |

---

### Combine Harvester - Header

| Type | Width | Application |
|------|-------|-------------|
| **Grain header** | 3-6 m | Wheat, Rice |
| **Row crop** | 4-8 rows | Maize, Sunflower |
| **Draper** | 6-12 m | Large combines |

---

### Combine - Threshing Unit

| Component | Specification |
|-----------|---------------|
| **Cylinder dia** | 45-60 cm |
| **Cylinder length** | 120-150 cm |
| **Concave length** | 60-80 cm |
| **Cylinder speed** | 600-1200 rpm |
| **Concave clearance** | 10-30 mm |

---

### Combine - Cleaning System

| Component | Specification |
|-----------|---------------|
| **Upper sieve** | 14-16 mm openings |
| **Lower sieve** | 8-10 mm openings |
| **Sieve area** | 3-5 m² |
| **Fan speed** | 600-900 rpm |
| **Air velocity** | 5-8 m/s |

---

### Straw Walkers

| Parameter | Specification |
|-----------|---------------|
| **Number** | 4-6 |
| **Length** | 3-4 m |
| **Inclination** | 6-10° |
| **Oscillation** | 180-250 rpm |
| **Throw** | 40-60 mm |

---

## 🎯 Performance Standards

### Loss Limits

| Loss Type | Acceptable Limit |
|-----------|------------------|
| **Total loss** | < 2% |
| **Header loss** | < 0.5% |
| **Threshing loss** | < 0.3% |
| **Separation loss** | < 0.7% |
| **Cleaning loss** | < 0.5% |

**Memory:** **"Total Too much if over 2%"**

---

### Efficiency Standards

| Efficiency Type | Target |
|-----------------|--------|
| **Threshing** | > 99% |
| **Separation** | > 97% |
| **Cleaning** | > 98% |
| **Field (combine)** | 70-80% |
| **Field (reaper)** | 75-85% |

---

### Grain Damage

| Category | Acceptable |
|----------|------------|
| **Visible damage** | < 1% |
| **Cracked grains** | < 2% |
| **Broken grains** | < 0.5% |

---

### Grain Quality Index

$$
\text{Quality Index} = 100 - \text{(Damage + Foreign matter + Moisture deviation)}
$$

**Excellent:** > 95
**Good:** 90-95
**Fair:** 85-90

---

## 🧮 Quick Calculation Templates

### Template 1: Cylinder Speed

**Given:** D = 50 cm, Need 20 m/s

**Solution:**
$$
N = \frac{60 \times 20}{3.14 \times 0.5} = \frac{1200}{1.57} \approx 764 \text{ rpm}
$$

---

### Template 2: Reel Index

**Given:** Forward speed = 3 km/h, Reel = 60 cm dia, 40 rpm

**Step 1:** Forward speed in m/s
$$
V_f = \frac{3000}{3600} = 0.833 \text{ m/s}
$$

**Step 2:** Reel speed
$$
V_r = \frac{3.14 \times 0.6 \times 40}{60} = 1.26 \text{ m/s}
$$

**Step 3:** Index
$$
\text{Index} = \frac{1.26}{0.833} = 1.51
$$

---

### Template 3: Field Capacity

**Given:** W = 4 m, S = 4.5 km/h, η = 70%

**TFC:**
$$
\text{TFC} = \frac{4 \times 4.5}{10} = 1.8 \text{ ha/h}
$$

**EFC:**
$$
\text{EFC} = 1.8 \times 0.70 = 1.26 \text{ ha/h}
$$

---

### Template 4: Loss Percentage

**Given:** 0.15 kg in 10 m², Yield = 3500 kg/ha

**Loss/ha:**
$$
\text{Loss} = \frac{0.15}{0.001} = 150 \text{ kg/ha}
$$

**Percentage:**
$$
\text{Loss \%} = \frac{150}{3500} \times 100 = 4.3\%
$$

---

## 🔍 Component Identification

### Cylinder Types

| Type | Appearance | Use |
|------|------------|-----|
| **Rasp bar** | Blunt rectangular bars | Wheat, Rice |
| **Peg tooth** | Pointed pegs | Pulses, Soybean |
| **Spike tooth** | Sharp spikes | Maize, Sorghum |
| **Wire loop** | Wire loops | Gentle crops |

**Visual Memory:** 
- **Rasp = Rectangle** (wheat)
- **Peg = Pointed** (pulses)
- **Spike = Sharp** (maize)

---

### Combine Flow Sequence

```
HEADER → THRESHING → SEPARATION → CLEANING → TANK
  ↓          ↓            ↓            ↓         ↓
 Cut       Grain      More grain   Pure grain  Storage
 Feed      60-70%     25-35%       99%+
```

**Memory:** **"H.T.S.C.T - Happy Thresher Separates Cleans Thoroughly"**

---

## 🛠️ Common Adjustments

### High Losses? Check:

**Header Loss:**
- ✓ Reduce forward speed
- ✓ Adjust reel height
- ✓ Check reel index (1.2-1.5)
- ✓ Sharpen cutter blade

**Threshing Loss:**
- ✓ Increase cylinder speed
- ✓ Reduce concave clearance
- ✓ Check cylinder condition

**Separation Loss:**
- ✓ Reduce forward speed
- ✓ Reduce crop feed rate
- ✓ Check straw walker condition

**Cleaning Loss:**
- ✓ Reduce fan speed
- ✓ Open sieve openings
- ✓ Reduce forward speed

---

### Grain Damage? Check:

- ✗ Cylinder speed too high → Reduce
- ✗ Concave too close → Increase clearance
- ✗ Cylinder in poor condition → Replace/repair
- ✗ Crop too dry → Harvest earlier/later in day

---

## 📐 Comparison Tables

### Harvesting Methods

| Method | Capacity | Labor | Cost | Quality |
|--------|----------|-------|------|---------|
| **Manual** | 0.05 ha/day | High | Low | Medium |
| **Reaper** | 0.4-0.6 ha/h | Medium | Medium | Medium |
| **Combine** | 1-2 ha/h | Low | High | High |

---

### Cylinder Types Comparison

| Feature | Rasp Bar | Peg Tooth | Spike Tooth |
|---------|----------|-----------|-------------|
| **Action** | Impact | Impact+Rubbing | Penetration |
| **Speed** | High (20 m/s) | Medium (12 m/s) | Low (8 m/s) |
| **Crops** | Cereals | Pulses | Maize |
| **Damage** | Low | Medium | High if misused |

---

### Combine vs Reaper-Thresher

| Aspect | Combine | Reaper + Thresher |
|--------|---------|-------------------|
| **Operations** | All-in-one | Two separate |
| **Cost** | High | Lower |
| **Capacity** | High (1-2 ha/h) | Lower |
| **Labor** | 1-2 persons | 4-6 persons |
| **Losses** | Lower | Higher |
| **Flexibility** | Lower | Higher |

---

## 💭 Memory Tricks

### Cylinder Speed by Crop
**"Wheat Wins at 20, Pulses at 12, Maize at 8"**

### Reel Index
**"1.2 to 1.5 - Reel beats feet"** (Reel faster than forward)

### Concave Clearance
**"30 In, 15 Out - Half the gap to knock it out"**

### Loss Limits
**"2% Total, Half% Each" (header, threshing, cleaning each <0.5%)**

### Efficiency Targets
**"99 for Threshing, 98 for Cleaning, 97 for Separating"**

### Combine Flow
**"Header Takes Stalks, Cylinder Takes Grain, Straw walker Takes Straw, Cleaning Takes Care"**

---

## 🎓 Problem-Solving Strategy

### For Cylinder Speed Problems:
1. Convert diameter to meters
2. Use V = πDN/60
3. Check if speed is suitable for crop
4. Typical cereals: 18-25 m/s

### For Reel Index Problems:
1. Convert forward speed to m/s
2. Calculate reel peripheral speed
3. Divide: Reel speed / Forward speed
4. Check if in range 1.2-1.5

### For Field Capacity:
1. Width (m) × Speed (km/h) ÷ 10 = TFC
2. TFC × efficiency = EFC
3. Typical efficiency: 70-80%

### For Losses:
1. Weight in sample → kg/ha (×10000 for 1m²)
2. Loss/ha ÷ Yield/ha × 100 = %
3. Compare with 2% limit

---

## ⚠️ Common Mistakes to Avoid

### ❌ Don't:
- Forget to convert cm to m for diameter
- Use wrong peripheral speed formula
- Confuse TFC and EFC
- Forget to multiply by 10000 for 1 m² sample
- Mix up cylinder types for different crops

### ✅ Do:
- Check units carefully
- Use π = 3.14159 (or 22/7)
- Remember crop-specific speeds
- Check if answer is in acceptable range
- Verify efficiency is between 0-100%

---

## 🔢 Unit Conversions

### Speed:
- km/h → m/s: Divide by 3.6
- m/s → km/h: Multiply by 3.6

### Area:
- 1 ha = 10,000 m²
- 1 m² = 0.0001 ha

### Diameter:
- Always convert cm to m
- 50 cm = 0.5 m

### Yield:
- 1 quintal (q) = 100 kg
- 35 q/ha = 3500 kg/ha

---

## 📝 Pre-Exam Checklist

### Must Remember:
- [ ] V_c = πDN/60
- [ ] Reel index = 1.2 to 1.5
- [ ] Wheat: 18-25 m/s, Pulses: 10-15 m/s
- [ ] Concave: Entry 25-30mm, Exit 10-15mm
- [ ] TFC = W×S/10
- [ ] Loss limit < 2%
- [ ] Threshing efficiency > 99%
- [ ] Combine flow: H→T→S→C→T
- [ ] Rasp bar for cereals, Peg tooth for pulses

### Quick Check:
- Can you calculate cylinder RPM given speed?
- Can you calculate reel index?
- Do you know loss measurement procedure?
- Can you identify cylinder types?
- Know the combine component sequence?

---

## 🎯 Exam Strategy

### Time Management:
- **1 mark:** 1-2 minutes max
- **2 marks:** 3-4 minutes
- **Component identification:** 30 seconds

### High Weightage Topics:
1. Cylinder speed calculations (★★★)
2. Loss measurement and limits (★★★)
3. Field capacity and efficiency (★★★)
4. Combine components and flow (★★)
5. Cylinder type selection (★★)

### Quick Win Topics:
- Cylinder types (easy 1 marker)
- Component functions (easy 1 marker)
- Acceptable limits (memorization)
- Combine sequence (memorization)

---

## 🔗 Related Topics

- [Detailed Theory](./README.md)
- [PYQ Solutions](./Solutions.md)
- [Farm Machinery Overview](../README.md)
- [Soil Working Machinery](../Soil_Working_Machinery/)
- [Seeding & Planting](../Seeding_Planting/)

---

**Quick Reference Version 1.0**  
**Last Updated:** November 2025  
**Topics Covered:** Reapers, Combines, Threshers, Losses, Efficiency  
**For:** GATE Agricultural Engineering

---

*Print this for last-minute revision!*  
*Master these formulas and you'll handle any harvesting question with confidence.*

🌾 **Happy Harvesting!** 🚜
