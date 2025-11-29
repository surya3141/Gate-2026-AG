# ⚙️ Size Reduction - CheatSheet

> **Quick Reference for GATE 2026**

---

## 🔥 Critical Formulas (MUST MEMORIZE)

### Energy Laws

```
Kick's:      E = Kk × log(Di/Df)
Rittinger's: E = Kr × (1/Df - 1/Di)
Bond's:      E = Ei × (1/√Df - 1/√Di)
```

### Reduction Ratio
```
R = Di / Df
```

### Screen Mesh
```
Opening (mm) ≈ 25.4 / Mesh number
Higher mesh = Finer screen
```

---

## 📋 Must-Know Values

### When to Use Each Law

| Law | Best For | Energy Ranking (fine grinding) |
|-----|----------|-------------------------------|
| **Kick's** | **Coarse crushing (>50mm)** | **Lowest** |
| **Bond's** | **General (1-50mm)** | **Medium** |
| **Rittinger's** | **Fine grinding (<1mm)** | **Highest** |

**Memory:** "RBK" - Rittinger > Bond > Kick for fine grinding

### Equipment Selection

| Mill | Product Size | Best Application | Key Feature |
|------|--------------|------------------|-------------|
| Jaw | Very coarse | Primary crushing | Compression |
| **Hammer** | **Coarse-Medium** | **Animal feed** | **Impact (versatile)** |
| **Roller** | **Fine** | **Flour milling** | **Compression** |
| Ball | Very fine | Ultra-fine | Attrition + impact |

**GATE favorites:**
- Hammer mill = General purpose/animal feed
- Roller mill = Flour milling
- Ball mill = Attrition AND impact

### Typical Reduction Ratios

| Equipment | Ratio | Memory |
|-----------|-------|--------|
| Jaw | 3-9:1 | ~5:1 |
| Roller | 4-8:1 | ~5:1 |
| **Hammer** | **10-40:1** | **~20:1 (highest)** |
| Ball | >50:1 | Very high |

### Screen Mesh Quick Reference

| Mesh | Opening (mm) | Use |
|------|--------------|-----|
| 4 | ~5 | Coarse |
| 8 | ~2.5 | Coarse |
| 20 | ~0.85 | Medium |
| 50 | ~0.30 | Fine |
| 100 | ~0.15 | Very fine |

**Rule:** Opening ≈ 25/Mesh (rough)

---

## 🎯 Quick Calculation Steps

### Problem Type 1: Reduction Ratio (15 seconds)

**Given:** Di = 40 mm, Df = 5 mm

**Steps:**
1. Write: R = Di/Df
2. Calculate: = 40/5 = **8**

### Problem Type 2: Kick's Law (1 minute)

**Given:** Di = 50 mm, Df = 10 mm, Kk = 10 kJ/kg

**Steps:**
1. Write: E = Kk × log(Di/Df)
2. Calculate R: = 50/10 = 5
3. Find log(5): = 0.699
4. Multiply: = 10 × 0.699 = **6.99 kJ/kg**

### Problem Type 3: Rittinger's Law (1 minute)

**Given:** Di = 50 mm, Df = 10 mm, Kr = 100 kJ·mm/kg

**Steps:**
1. Write: E = Kr × (1/Df - 1/Di)
2. Calculate: = 100 × (1/10 - 1/50)
3. = 100 × (0.1 - 0.02) = 100 × 0.08
4. Result: = **8 kJ/kg**

### Problem Type 4: Mesh to Opening (30 seconds)

**Given:** Mesh number = 20

**Steps:**
1. Write: Opening ≈ 25.4/Mesh
2. Calculate: = 25.4/20 = **1.27 mm**

Or use rough: ≈ 25/20 ≈ **1.25 mm**

### Problem Type 5: Equipment Selection (15 seconds)

**Question:** "Most suitable for animal feed grinding?"

**Steps:**
1. Identify need: General purpose, medium size
2. Answer: **Hammer mill**

**Question:** "For flour milling?"
**Answer:** **Roller mill**

---

## 💡 Memory Techniques

### 1. "RBK for Fine"
For **fine grinding**, energy requirement order:
- **R**ittinger (highest)
- **B**ond
- **K**ick (lowest)

For **coarse crushing**, reverse order!

### 2. "Hammer for Ham(burger)"
**Hammer mill** = Animal feed (for hamburgers!)
- Most versatile
- General-purpose
- 10-40:1 reduction

### 3. "Roll the Flour"
**Roller mill** = **Flour** milling
- Smooth rollers
- Fine grinding
- Controlled size

### 4. "Ball Grinds All (to dust)"
**Ball mill** = **Finest** grinding
- Attrition + Impact
- >50:1 reduction
- Ultra-fine product

### 5. "Higher Mesh, Finer Mesh"
**Mesh number ↑ → Opening size ↓**
- 4 mesh = coarse (~5 mm)
- 100 mesh = fine (~0.15 mm)

### 6. "Log for Large, Inverse for Little"
- **Kick's:** **log**(R) → for **large** (coarse) crushing
- **Rittinger's:** **1/D** terms → for **little** (fine) grinding
- **Bond's:** **√D** → in between

---

## ⚠️ Common Mistakes

### Mistake 1: Confusing energy laws
❌ **Wrong:** Using Kick's law for fine grinding
✅ **Correct:** Rittinger for fine, Kick for coarse, Bond for general

### Mistake 2: Equipment selection
❌ **Wrong:** Tray dryer for size reduction
✅ **Correct:** Dryers dry, mills grind! (Hammer, roller, ball mills)

### Mistake 3: Ball mill mechanism
❌ **Wrong:** Ball mill operates on impact only
✅ **Correct:** **Attrition AND impact** (both mechanisms)

### Mistake 4: Reduction ratio
❌ **Wrong:** R = Df/Di (inverted)
✅ **Correct:** R = Di/Df (initial ÷ final)

### Mistake 5: Mesh interpretation
❌ **Wrong:** Higher mesh = larger opening
✅ **Correct:** Higher mesh = MORE openings per inch = SMALLER opening

---

## 🎯 Pre-Exam Checklist

### Formulas to Write First:
```
1. Kick: E = Kk × log(Di/Df)
2. Rittinger: E = Kr × (1/Df - 1/Di)
3. Bond: E = Ei × (1/√Df - 1/√Di)
4. R = Di / Df
5. Opening ≈ 25.4 / Mesh
```

### Equipment Quick Reference:
- **Hammer:** General purpose, animal feed, 10-40:1
- **Roller:** Flour milling, fine, 4-8:1
- **Ball:** Ultra-fine, attrition+impact, >50:1

### Quick Checks:
- ✅ For fine grinding: Rittinger highest energy
- ✅ For coarse crushing: Kick gives lowest energy
- ✅ Hammer mill = most versatile
- ✅ Higher mesh = finer screen
- ✅ Reduction ratio always >1

---

## 📊 Exam Strategy

### Time Allocation:
- **Equipment selection:** 15 seconds
- **Reduction ratio:** 15 seconds
- **Energy calculation (simple):** 1 minute
- **Mesh calculation:** 30 seconds
- **Comparison question:** 30 seconds

### Priority Topics:
1. 🔥🔥🔥 **Energy laws** (which law for what)
2. 🔥🔥 **Equipment selection** (hammer/roller/ball)
3. 🔥 **Reduction ratio**
4. **Ball mill mechanism** (attrition+impact)
5. **Mesh number concept**

### If Short on Time:
1. Memorize: RBK order for fine grinding
2. Hammer = general, Roller = flour, Ball = finest
3. Ball mill = attrition + impact
4. Higher mesh = finer
5. R = Di/Df

---

## 🚀 Last-Minute Tips

### Write on entry:
```
RBK fine: Rittinger > Bond > Kick
Hammer: Animal feed (10-40:1)
Roller: Flour (4-8:1)
Ball: Attrition + Impact
High Mesh = Fine
```

### Mental checklist:
- [ ] Three energy laws clear?
- [ ] Equipment selection ready?
- [ ] Reduction ratio formula?
- [ ] Mesh concept understood?
- [ ] Ball mill = attrition+impact?

### During exam:
1. Law selection: Check if fine/coarse grinding
2. Equipment: Match application (feed→hammer, flour→roller)
3. Ball mill question: Always "attrition AND impact"
4. Mesh: Higher number = finer screen
5. Energy comparison: Remember RBK order

---

*[Theory](./README.md) | [Solutions](./Solutions.md) | [Section Home](../README.md)*
