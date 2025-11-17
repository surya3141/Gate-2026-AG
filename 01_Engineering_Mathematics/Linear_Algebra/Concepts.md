# 🔢 Linear Algebra - Concepts & Theory

> Comprehensive guide to Linear Algebra for GATE AG

---

## 📚 Table of Contents

1. [Matrices](#1-matrices)
2. [Determinants](#2-determinants)
3. [System of Linear Equations](#3-system-of-linear-equations)
4. [Eigenvalues and Eigenvectors](#4-eigenvalues-and-eigenvectors)
5. [Rank of Matrix](#5-rank-of-matrix)
6. [Linear Transformations](#6-linear-transformations)

---

## 1. Matrices

### 1.1 Definition and Types

A **matrix** is a rectangular array of numbers arranged in rows and columns.

$$
A = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix}_{m \times n}
$$

#### Types of Matrices

**1. Row Matrix:** $1 \times n$ matrix
$$
A = \begin{bmatrix} a_1 & a_2 & \cdots & a_n \end{bmatrix}
$$

**2. Column Matrix:** $m \times 1$ matrix
$$
A = \begin{bmatrix} a_1 \\ a_2 \\ \vdots \\ a_m \end{bmatrix}
$$

**3. Square Matrix:** $n \times n$ matrix (rows = columns)

**4. Diagonal Matrix:** Square matrix with non-zero elements only on main diagonal
$$
D = \begin{bmatrix} d_1 & 0 & 0 \\ 0 & d_2 & 0 \\ 0 & 0 & d_3 \end{bmatrix}
$$

**5. Identity Matrix:** Diagonal matrix with all diagonal elements = 1
$$
I = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}
$$

**6. Zero/Null Matrix:** All elements are zero

**7. Symmetric Matrix:** $A = A^T$ (element $a_{ij} = a_{ji}$)

**8. Skew-Symmetric Matrix:** $A = -A^T$ (element $a_{ij} = -a_{ji}$, diagonal = 0)

**9. Orthogonal Matrix:** $AA^T = A^TA = I$

---

### 1.2 Matrix Operations

#### Addition and Subtraction
Only possible for matrices of same order $(m \times n)$

$$
C = A + B \implies c_{ij} = a_{ij} + b_{ij}
$$

**Properties:**
- Commutative: $A + B = B + A$
- Associative: $(A + B) + C = A + (B + C)$

#### Scalar Multiplication
$$
kA = \begin{bmatrix} ka_{11} & ka_{12} \\ ka_{21} & ka_{22} \end{bmatrix}
$$

#### Matrix Multiplication
For $A_{m \times n}$ and $B_{n \times p}$, the product $C = AB$ is $m \times p$

$$
c_{ij} = \sum_{k=1}^{n} a_{ik}b_{kj}
$$

**Properties:**
- Generally NOT commutative: $AB \neq BA$
- Associative: $(AB)C = A(BC)$
- Distributive: $A(B + C) = AB + AC$

**Example:**
$$
\begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix} = \begin{bmatrix} 19 & 22 \\ 43 & 50 \end{bmatrix}
$$

#### Transpose
Interchange rows and columns: $(A^T)_{ij} = A_{ji}$

**Properties:**
- $(A^T)^T = A$
- $(A + B)^T = A^T + B^T$
- $(AB)^T = B^TA^T$
- $(kA)^T = kA^T$

---

### 1.3 Inverse of Matrix

For square matrix $A$, the inverse $A^{-1}$ exists if $\det(A) \neq 0$

$$
AA^{-1} = A^{-1}A = I
$$

#### Finding Inverse

**Method 1: Adjoint Method** (for $2 \times 2$ and $3 \times 3$)

$$
A^{-1} = \frac{1}{\det(A)} \text{adj}(A)
$$

**For $2 \times 2$ matrix:**
$$
A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \implies A^{-1} = \frac{1}{ad-bc} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}
$$

**Method 2: Gauss-Jordan Elimination**

Write $[A | I]$ and reduce to $[I | A^{-1}]$

**Properties of Inverse:**
- $(AB)^{-1} = B^{-1}A^{-1}$
- $(A^T)^{-1} = (A^{-1})^T$
- $(A^{-1})^{-1} = A$
- $\det(A^{-1}) = \frac{1}{\det(A)}$

---

## 2. Determinants

### 2.1 Definition

For square matrix $A_{n \times n}$, determinant is a scalar value denoted as $\det(A)$ or $|A|$

#### For $2 \times 2$ Matrix:
$$
\det \begin{bmatrix} a & b \\ c & d \end{bmatrix} = ad - bc
$$

#### For $3 \times 3$ Matrix:
$$
\det \begin{bmatrix} a & b & c \\ d & e & f \\ g & h & i \end{bmatrix} = a(ei - fh) - b(di - fg) + c(dh - eg)
$$

**Expansion by minors:**
$$
\det(A) = \sum_{j=1}^{n} a_{ij}C_{ij}
$$
where $C_{ij} = (-1)^{i+j}M_{ij}$ (cofactor)

---

### 2.2 Properties of Determinants

1. **Row/Column Interchange:** Changes sign
   $$\det(A') = -\det(A)$$

2. **Scalar Multiplication:**
   $$\det(kA) = k^n\det(A)$$ for $n \times n$ matrix

3. **Transpose:**
   $$\det(A^T) = \det(A)$$

4. **Product:**
   $$\det(AB) = \det(A) \cdot \det(B)$$

5. **Triangular Matrix:** Determinant = product of diagonal elements

6. **Row/Column of Zeros:** $\det(A) = 0$

7. **Two identical rows/columns:** $\det(A) = 0$

8. **Adding multiple of one row to another:** Determinant unchanged

---

### 2.3 Applications

- **Singular Matrix:** $\det(A) = 0$ (non-invertible)
- **Non-singular Matrix:** $\det(A) \neq 0$ (invertible)
- **Area/Volume:** Determinant represents area (2D) or volume (3D) transformation

---

## 3. System of Linear Equations

### 3.1 General Form

$$
\begin{cases}
a_{11}x_1 + a_{12}x_2 + \cdots + a_{1n}x_n = b_1 \\
a_{21}x_1 + a_{22}x_2 + \cdots + a_{2n}x_n = b_2 \\
\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \cdots + a_{mn}x_n = b_m
\end{cases}
$$

**Matrix Form:** $AX = B$

---

### 3.2 Solution Methods

#### Cramer's Rule (for $n \times n$ system with $\det(A) \neq 0$)

$$
x_i = \frac{\det(A_i)}{\det(A)}
$$

where $A_i$ is matrix $A$ with $i$-th column replaced by $B$

**Example:** For $2 \times 2$ system:
$$
\begin{cases}
a_1x + b_1y = c_1 \\
a_2x + b_2y = c_2
\end{cases}
$$

$$
x = \frac{\begin{vmatrix} c_1 & b_1 \\ c_2 & b_2 \end{vmatrix}}{\begin{vmatrix} a_1 & b_1 \\ a_2 & b_2 \end{vmatrix}}, \quad y = \frac{\begin{vmatrix} a_1 & c_1 \\ a_2 & c_2 \end{vmatrix}}{\begin{vmatrix} a_1 & b_1 \\ a_2 & b_2 \end{vmatrix}}
$$

#### Matrix Inverse Method

If $\det(A) \neq 0$:
$$
X = A^{-1}B
$$

#### Gauss Elimination Method

Reduce augmented matrix $[A|B]$ to row-echelon form

---

### 3.3 Solution Types

**Case 1:** $\det(A) \neq 0$ → **Unique solution**

**Case 2:** $\det(A) = 0$ and rank$(A)$ = rank$([A|B])$ → **Infinite solutions**

**Case 3:** $\det(A) = 0$ and rank$(A) <$ rank$([A|B])$ → **No solution**

---

## 4. Eigenvalues and Eigenvectors

### 4.1 Definitions

For square matrix $A$ and scalar $\lambda$:

**Eigenvalue $\lambda$:** Satisfies $\det(A - \lambda I) = 0$

**Eigenvector $X$:** Non-zero vector satisfying $AX = \lambda X$

---

### 4.2 Characteristic Equation

$$
\det(A - \lambda I) = 0
$$

**For $2 \times 2$ matrix:**
$$
A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}
$$

Characteristic equation:
$$
\lambda^2 - (a+d)\lambda + (ad-bc) = 0
$$

Or: $\lambda^2 - \text{tr}(A)\lambda + \det(A) = 0$

---

### 4.3 Properties

1. **Sum of eigenvalues** = Trace of matrix
   $$\sum \lambda_i = \text{tr}(A) = \sum a_{ii}$$

2. **Product of eigenvalues** = Determinant
   $$\prod \lambda_i = \det(A)$$

3. **Eigenvalues of $A^T$** = Eigenvalues of $A$

4. **Eigenvalues of $A^{-1}$** = $\frac{1}{\lambda_i}$

5. **Eigenvalues of $A^k$** = $\lambda_i^k$

6. **Symmetric matrix** has real eigenvalues

7. **Orthogonal matrix** has eigenvalues with $|\lambda| = 1$

---

### 4.4 Finding Eigenvectors

**Step 1:** Find eigenvalues from $\det(A - \lambda I) = 0$

**Step 2:** For each $\lambda_i$, solve $(A - \lambda_i I)X = 0$

**Example:**
$$
A = \begin{bmatrix} 3 & 1 \\ 1 & 3 \end{bmatrix}
$$

Characteristic equation: $(3-\lambda)^2 - 1 = 0$ → $\lambda = 4, 2$

For $\lambda_1 = 4$:
$$
\begin{bmatrix} -1 & 1 \\ 1 & -1 \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} = 0 \implies X_1 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}
$$

For $\lambda_2 = 2$:
$$
X_2 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}
$$

---

## 5. Rank of Matrix

### 5.1 Definition

**Rank** of matrix $A$ is the maximum number of linearly independent rows (or columns).

Denoted as: rank$(A)$ or $\rho(A)$

---

### 5.2 Methods to Find Rank

#### Method 1: Row Echelon Form

Reduce matrix to row echelon form; rank = number of non-zero rows

#### Method 2: Determinant Method

- If there exists $r \times r$ minor $\neq 0$, and all $(r+1) \times (r+1)$ minors = 0, then rank = $r$

---

### 5.3 Properties

1. $0 \leq$ rank$(A) \leq \min(m,n)$ for $m \times n$ matrix

2. rank$(A) =$ rank$(A^T)$

3. rank$(AB) \leq \min($rank$(A)$, rank$(B))$

4. For $n \times n$ matrix:
   - rank$(A) = n$ → Full rank (non-singular)
   - rank$(A) < n$ → Rank deficient (singular)

5. rank$(A + B) \leq$ rank$(A) +$ rank$(B)$

---

## 6. Linear Transformations

### 6.1 Definition

A **linear transformation** $T: \mathbb{R}^n \to \mathbb{R}^m$ satisfies:

1. $T(u + v) = T(u) + T(v)$
2. $T(ku) = kT(u)$

Can be represented as: $T(x) = Ax$ for some matrix $A$

---

### 6.2 Properties

- **Kernel (Null Space):** $\text{ker}(T) = \{x : T(x) = 0\}$
- **Image (Range):** $\text{Im}(T) = \{T(x) : x \in \mathbb{R}^n\}$
- **Rank-Nullity Theorem:** dim(ker) + dim(Im) = $n$

---

### 6.3 Special Transformations

**1. Rotation:** Rotates vector by angle $\theta$
$$
R(\theta) = \begin{bmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{bmatrix}
$$

**2. Scaling:** Scales by factors $k_1, k_2$
$$
S = \begin{bmatrix} k_1 & 0 \\ 0 & k_2 \end{bmatrix}
$$

**3. Reflection:** Reflects across axis

**4. Projection:** Projects onto subspace

---

## 💡 Key Takeaways

### Must Remember
1. ✅ $2 \times 2$ determinant and inverse formulas
2. ✅ Properties of determinants
3. ✅ Characteristic equation: $\det(A - \lambda I) = 0$
4. ✅ Sum of eigenvalues = Trace, Product = Determinant
5. ✅ Cramer's rule for $2 \times 2$ systems

### Common Errors to Avoid
⚠️ Matrix multiplication is not commutative  
⚠️ $(AB)^T = B^TA^T$ (order reverses)  
⚠️ $\det(A+B) \neq \det(A) + \det(B)$  
⚠️ $\det(kA) = k^n\det(A)$ for $n \times n$ matrix, not $k\det(A)$  

---

## 🔗 Related Topics

- [Calculus](../Calculus/Concepts.md) - Uses matrices in Jacobians
- [Differential Equations](../Differential_Equations/Concepts.md) - System of DEs
- [Numerical Methods](../Numerical_Methods/Concepts.md) - Matrix methods

---

## 📚 Practice Resources

- [PYQ Solutions](./PYQ_Solutions.md) - Solved previous year questions
- [Cheat Sheet](./CheatSheet.md) - Quick revision formulas
- [Back to Engineering Mathematics](../README.md)

---

<div align="center">

**Master these concepts through practice! 🎯**

[⬅️ Back](../README.md) | [Next: PYQ Solutions ➡️](./PYQ_Solutions.md)

</div>
