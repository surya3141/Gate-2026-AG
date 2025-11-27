# 🔢 Post-Harvest Machinery PYQ Solutions

> Previous Year Questions with detailed solutions for GATE Agricultural Engineering

---

## 📊 Solutions Summary

| Year | Questions | Difficulty Distribution | Topics Covered |
|------|-----------|-------------------------|----------------|
| 2024 | 3 | Easy: 1, Medium: 2 | Moisture, Storage, Dryer |
| 2023 | 2 | Medium: 2 | Grading, Milling |
| 2022 | 2 | Easy: 1, Medium: 1 | Cleaning, Capacity |
| 2021 | 3 | Easy: 1, Medium: 1, Hard: 1 | Drying, Silo, Aeration |
| 2020 | 2 | Easy: 1, Medium: 1 | Parboiling, Conveyor |
| **Total** | **12** | **Easy: 4, Medium: 7, Hard: 1** | **All Major Topics** |

---

## 2024 Questions

### Question 1 (Easy) - Moisture Content #MoistureContent #2024
**Paddy is stored at 20% moisture content (wet basis). Convert this to dry basis.**

**Solution:**

Given:
- MC (wet basis) = 20%

**Formula for conversion:**
$$
MC_{db} = \frac{MC_{wb}}{100 - MC_{wb}} \times 100
$$

**Substitute:**
$$
MC_{db} = \frac{20}{100-20} \times 100 = \frac{20}{80} \times 100 = 25\%
$$

**Understanding:**

In 100 kg grain at 20% wb:
- Water = 20 kg
- Dry matter = 80 kg

**Wet basis:** Water/Total = 20/100 = 20%
**Dry basis:** Water/Dry matter = 20/80 = 25%

**Why different?**
- Wet basis: Denominator includes water
- Dry basis: Denominator is only dry matter

**Dry basis is always HIGHER than wet basis** (for same grain)

**Verification - Reverse calculation:**
$$
MC_{wb} = \frac{MC_{db}}{100+MC_{db}} \times 100 = \frac{25}{100+25} \times 100 = \frac{25}{125} \times 100 = 20\% \quad \checkmark
$$

**Answer:** 25% (dry basis)

**Time:** 2 minutes | **Marks:** 1

---

### Question 2 (Medium) - Water Removal #Drying #2024
**A farmer has 2000 kg of wheat at 18% moisture content (wet basis). How much water must be removed to reduce moisture to 12% for safe storage?**

**Solution:**

Given:
- Initial weight (W_i) = 2000 kg
- Initial MC (M_i) = 18% wb
- Final MC (M_f) = 12% wb

**Formula:**
$$
W_r = W_i \times \frac{M_i - M_f}{100 - M_f}
$$

Where:
- W_r = Water to remove (kg)

**Calculate:**
$$
W_r = 2000 \times \frac{18-12}{100-12} = 2000 \times \frac{6}{88} = 2000 \times 0.0682 = 136.4 \text{ kg}
$$

**Final weight after drying:**
$$
W_f = W_i - W_r = 2000 - 136.4 = 1863.6 \text{ kg}
$$

**Verification:**

Initial water content:
$$
W_{water,i} = 2000 \times 0.18 = 360 \text{ kg}
$$

Final water content:
$$
W_{water,f} = 1863.6 \times 0.12 = 223.6 \text{ kg}
$$

Water removed:
$$
W_r = 360 - 223.6 = 136.4 \text{ kg} \quad \checkmark
$$

**Practical Implications:**
- Weight loss: 136.4/2000 = 6.8%
- Farmer loses 6.8% weight but gains quality
- Storage cost reduced (lighter)
- Sale by weight, so financial loss offset by better price

**Answer:** 136.4 kg (or approximately 136 kg)

**Time:** 4 minutes | **Marks:** 2

---

### Question 3 (Medium) - Silo Capacity #Storage #2024
**A cylindrical silo has 8 m diameter and 24 m height. If wheat (bulk density 0.80 t/m³) is stored to 90% of height, calculate the storage capacity in metric tons.**

**Solution:**

Given:
- Diameter (D) = 8 m
- Total height (H) = 24 m
- Fill height = 90% of 24 = 0.9 × 24 = 21.6 m
- Bulk density (ρ) = 0.80 t/m³

**Step 1: Calculate volume**

$$
V = \frac{\pi D^2 h}{4}
$$

Where h = fill height = 21.6 m

$$
V = \frac{3.14159 \times 8^2 \times 21.6}{4} = \frac{3.14159 \times 64 \times 21.6}{4}
$$

$$
V = \frac{4344.35}{4} = 1086.1 \text{ m}^3
$$

**Step 2: Calculate mass**

$$
M = V \times \rho = 1086.1 \times 0.80 = 868.9 \text{ tons}
$$

**Why not fill to 100% height?**
- Need headspace for loading
- Prevent spillage
- Aeration system requires space
- Typical fill: 85-95% of height

**Additional Calculations:**

**If filled to 100%:**
$$
V_{100} = \frac{3.14159 \times 64 \times 24}{4} = 1206.4 \text{ m}^3
$$
$$
M_{100} = 1206.4 \times 0.80 = 965.1 \text{ tons}
$$

Difference = 965.1 - 868.9 = 96.2 tons lost by filling to 90%

**Wall pressure at bottom (bonus):**
$$
P = k \times \rho \times g \times h = 0.4 \times 800 \times 9.81 \times 21.6 = 67,900 \text{ Pa} = 67.9 \text{ kPa}
$$

**Answer:** 869 tons (or approximately 870 tons)

**Time:** 5 minutes | **Marks:** 2

---

## 2023 Questions

### Question 4 (Medium) - Color Sorter #Grading #2023
**A rice color sorter has 128 channels and operates at 3 tons/hour capacity per channel. If the rejection rate is 5%, calculate:**
**(a) Total throughput capacity**
**(b) Mass of rejected grain per hour**

**Solution:**

Given:
- Number of channels = 128
- Capacity per channel = 3 t/h
- Rejection rate = 5%

**Part (a): Total Throughput**

$$
\text{Total capacity} = \text{Channels} \times \text{Capacity/channel}
$$

$$
\text{Total capacity} = 128 \times 3 = 384 \text{ t/h}
$$

**Part (b): Rejected Grain**

$$
\text{Rejected grain} = \text{Total capacity} \times \frac{\text{Rejection rate}}{100}
$$

$$
\text{Rejected} = 384 \times \frac{5}{100} = 384 \times 0.05 = 19.2 \text{ t/h}
$$

**Understanding Rejection Rate:**

**Not all rejected = defective!**
- True defects: 3-4%
- Good grain rejected: 1-2% (false positives)
- Total rejection: 5%

**Why good grain rejected?**
- Borderline color
- Sensor sensitivity
- High-speed operation
- Better to be safe

**Economic Analysis:**

Assuming rice price = ₹30/kg:
- Rejected per day (20 h) = 19.2 × 20 = 384 tons
- Value = 384,000 kg × ₹30 = ₹1,15,20,000 per day

**But rejected grain can be:**
- Sold as lower grade
- Reprocessed
- Animal feed
- Not total loss!

**Quality Improvement:**
- Input: 384 t with 5% defects
- Output: 364.8 t with <0.5% defects
- Much better market value

**Answers:**
- (a) Total capacity = 384 t/h
- (b) Rejected grain = 19.2 t/h

**Time:** 4 minutes | **Marks:** 2

---

### Question 5 (Medium) - Rice Milling Yield #Milling #2023
**A rice mill processes 10 tons of paddy. The outputs are:**
**- Husk: 2.0 tons**
**- Bran: 0.9 tons**
**- Broken rice: 1.2 tons**
**- Head rice: 5.6 tons**

**Calculate:**
**(a) Total milled rice recovery**
**(b) Head rice recovery (HRR)**
**(c) Degree of milling (bran removal %)**

**Solution:**

Given:
- Paddy input = 10 tons
- Husk = 2.0 tons (20%)
- Bran = 0.9 tons (9%)
- Broken rice = 1.2 tons
- Head rice = 5.6 tons
- Loss/moisture = 10 - (2.0 + 0.9 + 1.2 + 5.6) = 0.3 tons

**Part (a): Total Milled Rice Recovery**

$$
\text{Milled rice} = \text{Head rice} + \text{Broken rice} = 5.6 + 1.2 = 6.8 \text{ tons}
$$

$$
\text{Recovery (\%)} = \frac{6.8}{10} \times 100 = 68\%
$$

**Part (b): Head Rice Recovery (HRR)**

$$
\text{HRR (\%)} = \frac{\text{Head rice}}{\text{Paddy}} \times 100 = \frac{5.6}{10} \times 100 = 56\%
$$

**Part (c): Degree of Milling**

After dehusking, brown rice = 10 - 2.0 = 8.0 tons

$$
\text{Bran removal (\%)} = \frac{0.9}{8.0} \times 100 = 11.25\%
$$

**Analysis:**

**Milling Recovery (68%):**
- Below average (typical: 70-72%)
- Indicates quality issues or over-milling

**HRR (56%):**
- Good (typical: 55-65%)
- Higher HRR = Better quality paddy + Processing
- Better price for head rice vs broken

**Broken Rice (1.2 tons = 12% of paddy):**
- Acceptable (typical: 10-15%)
- Used for flour, animal feed, brewing

**Husk (20%):**
- Normal (typical: 18-20%)
- Used as fuel in boilers
- Ash for cement industry

**Bran (9%):**
- Normal (typical: 8-10%)
- Sold for oil extraction, animal feed
- Rich in vitamins, fiber

**Improving HRR:**
- Better paddy variety
- Proper drying (avoid over-drying → cracking)
- Gentle milling
- Two-stage whitening
- Less breakage

**Answers:**
- (a) Milled rice recovery = 68%
- (b) Head rice recovery = 56%
- (c) Degree of milling = 11.25%

**Time:** 6 minutes | **Marks:** 2

---

## 2022 Questions

### Question 6 (Easy) - Cleaning Equipment #Cleaning #2022
**In a gravity separator for grain cleaning, how are heavier stones separated from lighter grain?**

**Options:**
(a) By sieving through different sized openings  
(b) By air aspiration blowing away stones  
(c) By fluidization and differential stratification on vibrating deck  
(d) By magnetic attraction

**Solution:**

**Gravity Separator Working:**

**Principle:** Separation based on **specific gravity (density)** differences.

**Components:**
1. Perforated deck (inclined 2-6°)
2. Air flow upward through perforations
3. Vibrating mechanism

**Process:**

**Step 1: Fluidization**
- Mixture fed onto deck
- Air flows upward through perforations
- Material becomes semi-fluid (fluidized bed)

**Step 2: Stratification**
- Lighter grain: Lifted more by air
- Heavier stones: Less lifted, sink to bottom
- Layers form: Heavy at bottom, light on top

**Step 3: Separation by Vibration**
- Deck vibrates (200-300 vpm)
- Direction: Perpendicular to slope
- Heavy particles (stones): Move UPWARD (against slope)
- Light particles (grain): Move DOWNWARD (with slope)

**Why upward movement for heavy?**
- Bottom layer (stones) in contact with deck
- Vibration pushes them up incline
- Top layer (grain) slides down

**Step 4: Collection**
- Heavy stones exit at top
- Light grain exits at bottom
- Intermediate products at middle outlets

**Why NOT Other Options?**

**(a) Sieving:**
- Separates by SIZE, not density
- Grain and stones may be similar size

**(b) Air aspiration:**
- Blows away LIGHT materials (chaff)
- Cannot blow heavy stones

**(d) Magnetic:**
- Only for ferrous metals
- Stones are non-magnetic

**Answer:** (c) By fluidization and differential stratification on vibrating deck

**Time:** 3 minutes | **Marks:** 1

---

### Question 7 (Medium) - Storage Capacity #Storage #2022
**A rectangular godown measures 25 m × 12 m × 5 m (height). Wheat bags (50 kg each) are stacked to 4 m height with 55% space utilization. Calculate the storage capacity in metric tons.**

**Solution:**

Given:
- Length (L) = 25 m
- Width (W) = 12 m
- Total height = 5 m
- Stack height (h) = 4 m
- Space utilization = 55% = 0.55
- Bag weight = 50 kg = 0.05 tons

**Step 1: Calculate storage volume**

$$
V = L \times W \times h = 25 \times 12 \times 4 = 1200 \text{ m}^3
$$

**Step 2: Effective volume (accounting for gaps)**

$$
V_{eff} = V \times \text{Space utilization} = 1200 \times 0.55 = 660 \text{ m}^3
$$

**Step 3: Calculate capacity**

**Method 1: Using bulk density**

Wheat bulk density in bags ≈ 0.75 t/m³

$$
\text{Capacity} = V_{eff} \times \rho = 660 \times 0.75 = 495 \text{ tons}
$$

**Method 2: Using bag count**

Volume per bag = 0.05 tons ÷ 0.75 t/m³ = 0.067 m³

Number of bags = 660 ÷ 0.067 = 9,850 bags

Capacity = 9,850 × 0.05 = 492.5 tons

**Why 55% Space Utilization?**

**Gaps between:**
- Bags in stack (irregular shape)
- Stacks (aisles for access)
- Walls (clearance)
- Different lots (separation)

**Breakdown:**
- Bag stacking: 75-80% efficiency
- Aisles and clearances: 20-25% loss
- Overall: 55-60%

**For bulk storage:** 90-95% utilization (no bags, fewer gaps)

**Practical Considerations:**

**Why not stack to 5 m?**
- Bottom bags crushed (weight pressure)
- Safety hazard
- Difficult to handle top bags
- 4 m ≈ 15-16 bag layers (safe limit)

**Answer:** 495 tons (or 490-500 tons acceptable)

**Time:** 4 minutes | **Marks:** 2

---

## 2021 Questions

### Question 8 (Easy) - Parboiling #Parboiling #2021
**What is the primary purpose of parboiling paddy before milling?**

**Options:**
(a) To reduce moisture content  
(b) To increase head rice yield and improve nutritional value  
(c) To remove husk easily  
(d) To improve whiteness of rice

**Solution:**

**Parboiling Process:**

**Steps:**
1. Soaking (in hot water, 3-6 hours)
2. Steaming (under pressure, 10-20 min)
3. Drying (to 14% MC)

**What Happens During Parboiling:**

**Gelatinization:**
- Starch molecules absorb water
- Swell and become gel-like
- Bind together within grain

**Nutrient Migration:**
- Water-soluble vitamins (B-complex) in bran
- Migrate into endosperm
- Locked in after gelatinization

**Grain Hardening:**
- Starch gel hardens on cooling
- Grain becomes tougher
- More resistant to breakage

---

**Effects of Parboiling:**

**1. Increased Head Rice Yield (PRIMARY):**
- Unparboiled: 55-60% HRR
- Parboiled: 65-70% HRR
- 10-15% improvement!
- Less breakage during milling

**2. Improved Nutrition:**
- Vitamin B1, B2, B3 move to endosperm
- Normally lost with bran removal
- Parboiled rice retains vitamins

**3. Easier Milling:**
- Husk-rice separation better
- Less breakage
- Higher throughput

**4. Better Storage:**
- More resistant to insects
- Harder texture deters pests

---

**Why NOT Other Options?**

**(a) Reduce moisture:**
- WRONG - Parboiling ADDS moisture (soaking!)
- Drying is separate step after parboiling

**(c) Remove husk easily:**
- Minimal effect on dehusking
- Husk removal same as normal paddy

**(d) Improve whiteness:**
- OPPOSITE - Parboiled rice is slightly YELLOW
- Starch gelatinization causes color change
- Market preference varies (some prefer, some don't)

**Disadvantages of Parboiling:**
- Yellowish color (cultural preference issue)
- Different taste/texture
- Additional processing cost
- Energy required

**But advantages outweigh for:**
- Commercial milling (yield++)
- Nutrition programs
- Export (less breakage in transport)

**Answer:** (b) To increase head rice yield and improve nutritional value

**Time:** 3 minutes | **Marks:** 1

---

### Question 9 (Medium) - Dryer Performance #Drying #2021
**A batch dryer with 5-ton capacity dries paddy from 24% to 14% MC (wet basis) in 8 hours. The dryer uses 120 kg of rice husk as fuel with a heating value of 12 MJ/kg. Calculate the specific energy consumption in MJ per kg of water removed.**

**Solution:**

Given:
- Grain capacity = 5 tons = 5000 kg
- Initial MC (M_i) = 24% wb
- Final MC (M_f) = 14% wb
- Drying time = 8 hours
- Fuel used = 120 kg
- Heating value = 12 MJ/kg

**Step 1: Calculate water removed**

$$
W_r = W_i \times \frac{M_i - M_f}{100-M_f}
$$

$$
W_r = 5000 \times \frac{24-14}{100-14} = 5000 \times \frac{10}{86} = 5000 \times 0.116 = 581.4 \text{ kg}
$$

**Step 2: Calculate total energy input**

$$
E_{input} = \text{Fuel} \times \text{Heating value} = 120 \times 12 = 1440 \text{ MJ}
$$

**Step 3: Calculate specific energy consumption**

$$
\text{SEC} = \frac{E_{input}}{W_r} = \frac{1440}{581.4} = 2.477 \text{ MJ/kg water}
$$

**Analysis:**

**Theoretical minimum energy:**
- Latent heat of vaporization = 2.5 MJ/kg
- This SEC (2.477) is VERY CLOSE to theoretical!
- Indicates IMPOSSIBLE efficiency (>100%)

**Likely scenario:**
- Question is simplified
- Real SEC should be 4-10 MJ/kg water
- Accounts for:
  - Heating grain
  - Heating air
  - Heat losses
  - Exhaust heat

**Realistic Calculation (if we consider):**

Only 30-40% of fuel energy goes to evaporation:
$$
\text{Realistic SEC} = \frac{1440}{581.4 \times 0.35} = \frac{1440}{203.5} = 7.08 \text{ MJ/kg water}
$$

This is more reasonable!

**Comparison with Standards:**

| Dryer Type | Typical SEC (MJ/kg water) |
|------------|---------------------------|
| **Efficient dryer** | 4-6 |
| **Average dryer** | 6-8 |
| **Poor dryer** | 8-12 |
| **Theoretical min** | 2.5 |

**Answer:** 2.48 MJ/kg water (as per given data)

*Note: In real scenarios, expect 4-10 MJ/kg water due to losses*

**Time:** 6 minutes | **Marks:** 2

---

### Question 10 (Hard) - Aeration System Design #Aeration #2021
**Design an aeration system for a flat storage of 10 m × 10 m × 4 m height filled with wheat. The recommended specific airflow is 8 m³/min per ton. Wheat bulk density is 0.80 t/m³. Calculate:**
**(a) Total grain mass**
**(b) Required airflow rate**
**(c) If perforated ducts of 30 cm diameter are used with air velocity of 10 m/s through duct, calculate the number of ducts needed**

**Solution:**

Given:
- Storage dimensions: L = 10 m, W = 10 m, H = 4 m
- Bulk density (ρ) = 0.80 t/m³
- Specific airflow = 8 m³/min per ton
- Duct diameter (d) = 30 cm = 0.3 m
- Air velocity in duct (v) = 10 m/s

**Part (a): Total Grain Mass**

$$
V = L \times W \times H = 10 \times 10 \times 4 = 400 \text{ m}^3
$$

$$
M = V \times \rho = 400 \times 0.80 = 320 \text{ tons}
$$

**Part (b): Required Airflow Rate**

$$
Q_{total} = M \times \text{Specific airflow} = 320 \times 8 = 2560 \text{ m}^3\text{/min}
$$

**Part (c): Number of Ducts**

**Step 1: Calculate airflow per duct**

Cross-sectional area of duct:
$$
A = \frac{\pi d^2}{4} = \frac{3.14159 \times 0.3^2}{4} = \frac{0.2827}{4} = 0.0707 \text{ m}^2
$$

Airflow per duct:
$$
Q_{duct} = A \times v = 0.0707 \times 10 = 0.707 \text{ m}^3\text{/s}
$$

Convert to m³/min:
$$
Q_{duct} = 0.707 \times 60 = 42.4 \text{ m}^3\text{/min}
$$

**Step 2: Calculate number of ducts**

$$
N = \frac{Q_{total}}{Q_{duct}} = \frac{2560}{42.4} = 60.4 \approx 61 \text{ ducts}
$$

**Step 3: Duct layout (practical design)**

**For 10 m × 10 m floor:**

Arrange ducts in grid pattern:
- Duct spacing: 1.2-1.5 m (typical)
- Use spacing = 1.25 m

Number of ducts in each direction:
$$
n = \frac{10}{1.25} + 1 = 9 \text{ ducts per direction}
$$

If grid pattern (cross ducts):
- Main ducts (length-wise): 9 ducts
- Cross ducts (width-wise): 9 ducts
- Total duct points: 9 × 9 = 81 intersection points

**But calculated need:** 61 ducts

**Practical layout options:**

**Option 1: Parallel ducts**
- 61 ducts parallel
- Spacing: 10/61 = 0.164 m (too close! Not practical)

**Option 2: Fewer, longer ducts with more perforations**
- Use 8-10 main ducts across 10 m
- Spacing: 1.2 m
- More perforations along length
- Reduce velocity in ducts

**Option 3: Increase duct diameter**
- Use larger ducts (40-50 cm)
- Fewer ducts needed
- More economical

**Practical Solution:**
Use 8-10 ducts of 40 cm diameter with optimized spacing

**Answers:**
- (a) Total grain mass = 320 tons
- (b) Required airflow = 2560 m³/min
- (c) Number of 30 cm ducts = 61 (theoretical)
  - Practical: Use 8-10 larger ducts (40-50 cm) with 1.2 m spacing

**Time:** 10 minutes | **Marks:** 2

---

## 2020 Questions

### Question 11 (Easy) - Material Handling #Conveyor #2020
**Which material handling equipment is most suitable for vertically lifting grain to a height of 30 meters in a silo?**

**Options:**
(a) Belt conveyor  
(b) Screw conveyor  
(c) Bucket elevator  
(d) Pneumatic conveyor

**Solution:**

**Requirements:**
- VERTICAL lifting
- Height: 30 m (tall silo)
- Material: Grain

**Equipment Analysis:**

**Belt Conveyor:**
- Horizontal or slight incline (max 20-25°)
- Cannot handle vertical or steep slopes
- ❌ Not suitable for 30 m vertical

**Screw Conveyor:**
- Horizontal or incline up to 45°
- Short distances (10-20 m max)
- High power for inclination
- ❌ Not practical for 30 m vertical

**Bucket Elevator:**
- **VERTICAL lifting** ✓
- Height: Up to 50-60 m ✓
- Continuous operation ✓
- High capacity ✓
- Reliable ✓
- **BEST CHOICE**

**Pneumatic Conveyor:**
- Can handle vertical
- Flexible routing
- But: High power consumption
- Lower capacity
- Not preferred for regular silo filling

---

**Bucket Elevator Details:**

**Design:**
- Continuous belt or chain
- Buckets attached at intervals
- Runs over pulleys (top and bottom)
- Enclosed in casing

**Operation:**
1. Grain falls into buckets at bottom
2. Buckets carry grain upward
3. Discharge at top (centrifugal or gravity)
4. Empty buckets return down

**Specifications for Silos:**
- Height: 20-50 m (30 m ✓)
- Capacity: 10-200 t/h
- Bucket spacing: 30-50 cm
- Speed: 1-2 m/s
- Power: 5-20 HP

**Types:**
- Centrifugal discharge (high speed)
- Positive discharge (low speed)
- Continuous (closely spaced buckets)

**Advantages:**
- Compact footprint
- High capacity
- Gentle handling
- Low maintenance
- Proven for grain

**Answer:** (c) Bucket elevator

**Time:** 2 minutes | **Marks:** 1

---

### Question 12 (Medium) - Cleaning Efficiency #Cleaning #2020
**A grain cleaner processes 1200 kg/h of wheat containing 8% impurities. After cleaning, the output has 1.5% impurities. If 90 kg of good grain is lost with impurities, calculate:**
**(a) Cleaning efficiency**
**(b) Grain loss percentage**

**Solution:**

Given:
- Input rate = 1200 kg/h
- Input impurity = 8%
- Output impurity = 1.5%
- Good grain lost = 90 kg

**Analysis of Input:**

Total impurity in input:
$$
I_{in} = 1200 \times 0.08 = 96 \text{ kg}
$$

Good grain in input:
$$
G_{in} = 1200 \times 0.92 = 1104 \text{ kg}
$$

**Output Streams:**

**Clean grain output:**
Let clean output = C kg

Impurity in clean output:
$$
I_{clean} = C \times 0.015
$$

Good grain in clean output:
$$
G_{clean} = C \times 0.985
$$

**Reject/Waste output:**
Total waste = Input - Clean output = 1200 - C

Contains:
- Impurities removed
- Good grain lost (90 kg)

---

**Mass Balance:**

Good grain IN = Good grain in CLEAN + Good grain LOST
$$
1104 = G_{clean} + 90
$$
$$
G_{clean} = 1014 \text{ kg}
$$

Since clean output has 98.5% good grain:
$$
C = \frac{G_{clean}}{0.985} = \frac{1014}{0.985} = 1029.4 \text{ kg}
$$

Impurity in clean output:
$$
I_{clean} = 1029.4 \times 0.015 = 15.4 \text{ kg}
$$

**Impurity removed:**
$$
I_{removed} = I_{in} - I_{clean} = 96 - 15.4 = 80.6 \text{ kg}
$$

---

**Part (a): Cleaning Efficiency**

$$
\eta_c = \frac{\text{Impurity removed}}{\text{Total impurity in input}} \times 100
$$

$$
\eta_c = \frac{80.6}{96} \times 100 = 83.96\% \approx 84\%
$$

**Part (b): Grain Loss Percentage**

$$
\text{Loss (\%)} = \frac{\text{Good grain lost}}{\text{Good grain in input}} \times 100
$$

$$
\text{Loss} = \frac{90}{1104} \times 100 = 8.15\%
$$

**Interpretation:**

**Cleaning efficiency (84%):**
- Acceptable (typical: 85-95%)
- 84% of impurities removed
- 16% impurities remain in output

**Grain loss (8.15%):**
- HIGH! (acceptable: 2-5%)
- Indicates poor adjustment
- Too aggressive cleaning
- Economic loss

**Improvement suggestions:**
- Adjust sieve openings (larger)
- Reduce fan speed (less good grain blown away)
- Better calibration
- Multi-stage cleaning

**Answers:**
- (a) Cleaning efficiency = 84%
- (b) Grain loss = 8.15%

**Time:** 7 minutes | **Marks:** 2

---

## 📈 Difficulty Analysis

| Difficulty | Count | Percentage | Topics |
|------------|-------|------------|--------|
| **Easy** | 4 | 33% | Concept-based, identification |
| **Medium** | 7 | 58% | Calculations, analysis |
| **Hard** | 1 | 9% | Multi-step design problem |

---

## 🎯 Topic-wise Breakdown

| Topic | Questions | Key Concepts |
|-------|-----------|--------------|
| **Moisture & Drying** | 3 | MC conversion, water removal, SEC |
| **Storage** | 2 | Capacity calculation, silo design |
| **Milling** | 1 | Yield, HRR, recovery |
| **Grading** | 1 | Color sorter, throughput |
| **Cleaning** | 2 | Gravity separator, efficiency |
| **Aeration** | 1 | Airflow, duct design |
| **Parboiling** | 1 | Purpose, benefits |
| **Handling** | 1 | Equipment selection |

---

## 💡 Preparation Tips

### For Easy Questions (1 mark):
- Equipment functions and applications
- Basic principles (gravity separation, parboiling)
- Equipment selection for given task

### For Medium Questions (2 marks):
- Moisture content conversions (wb ↔ db)
- Water removal calculations
- Storage capacity (silo, godown)
- Milling yield and recovery
- Efficiency calculations

### For Hard Questions:
- Multi-step design (aeration system)
- Combined concepts
- Practical layout considerations

---

## 🧮 Formula Quick Reference

### Moisture Content
$$
MC_{db} = \frac{MC_{wb}}{100-MC_{wb}} \times 100
$$

### Water Removal
$$
W_r = W_i \times \frac{M_i - M_f}{100 - M_f}
$$

### Silo Capacity
$$
M = \frac{\pi D^2 H}{4} \times \rho
$$

### Cleaning Efficiency
$$
\eta = \frac{\text{Impurity removed}}{\text{Total impurity}} \times 100
$$

### Milling Recovery
$$
\text{Recovery} = \frac{\text{Output}}{\text{Input}} \times 100
$$

### Airflow
$$
Q = M \times \text{Specific airflow}
$$

---

## 🔗 Quick Links

- [Post-Harvest Theory](./README.md)
- [Quick Reference](./CheatSheet.md)
- [Farm Machinery Index](../README.md)

---

**Total Questions:** 12  
**Last Updated:** November 2025  
**Source:** GATE AG Previous Year Papers (2020-2024)

---

*For theory concepts, see [Post-Harvest README](./README.md)*  
*For quick revision, see [Post-Harvest Cheat Sheet](./CheatSheet.md)*
