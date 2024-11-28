## 1. Basic Operations on Matrices

### Given Matrices:
$$
A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} \;
B = \begin{pmatrix} 5 & 6 \\ 7 & 8 \end{pmatrix} \;
C = \begin{pmatrix} -1 & 2 \\ 3 & 0 \end{pmatrix} \;
D = \begin{pmatrix} -1 & 2 \\ 3 & 4 \\ 0 & 6 \end{pmatrix} \;
E = \begin{pmatrix} 1 & 2 & 4 \\ 5 & 7 & 8 \end{pmatrix}
$$

---

### 1. **Matrix Additions and Subtractions**  
$$
A + B = \begin{pmatrix} 1+5 & 2+6 \\ 3+7 & 4+8 \end{pmatrix} = \begin{pmatrix} 6 & 8 \\ 10 & 12 \end{pmatrix}
$$

$$
B - A = \begin{pmatrix} 5-1 & 6-2 \\ 7-3 & 8-4 \end{pmatrix} = \begin{pmatrix} 4 & 4 \\ 4 & 4 \end{pmatrix}
$$

$$
A + C = \begin{pmatrix} 1+(-1) & 2+2 \\ 3+3 & 4+0 \end{pmatrix} = \begin{pmatrix} 0 & 4 \\ 6 & 4 \end{pmatrix}
$$

$$
D + E = \text{Not Defined (incompatible dimensions)}.
$$

---

### 2. **Scalar Multiplications**  
$$
\frac{1}{2}A = \begin{pmatrix} \frac{1}{2} & 1 \\ \frac{3}{2} & 2 \end{pmatrix}.
$$

$$
2B = \begin{pmatrix} 10 & 12 \\ 14 & 16 \end{pmatrix}.
$$

$$
-3C = \begin{pmatrix} 3 & -6 \\ -9 & 0 \end{pmatrix}.
$$

$$
4D = \begin{pmatrix} -4 & 8 \\ 12 & 16 \\ 0 & 24 \end{pmatrix}.
$$

---

### 3. **Matrix Products**  
$$
A \cdot B = \begin{pmatrix} 1\cdot5 + 2\cdot7 & 1\cdot6 + 2\cdot8 \\ 3\cdot5 + 4\cdot7 & 3\cdot6 + 4\cdot8 \end{pmatrix} = \begin{pmatrix} 19 & 22 \\ 43 & 50 \end{pmatrix}.
$$

$$
B \cdot A = \begin{pmatrix} 5\cdot1 + 6\cdot3 & 5\cdot2 + 6\cdot4 \\ 7\cdot1 + 8\cdot3 & 7\cdot2 + 8\cdot4 \end{pmatrix} = \begin{pmatrix} 23 & 34 \\ 31 & 46 \end{pmatrix}.
$$

$$
A \cdot D = \text{Not Defined (incompatible dimensions)}.
$$

$$
D \cdot E = \begin{pmatrix} 
-1\cdot1 + 2\cdot5 + 4\cdot0 & -1\cdot2 + 2\cdot7 + 4\cdot6 & -1\cdot4 + 2\cdot8 + 4\cdot8 \\ 
3\cdot1 + 4\cdot5 + 0\cdot0 & 3\cdot2 + 4\cdot7 + 0\cdot6 & 3\cdot4 + 4\cdot8 + 0\cdot8 \\ 
0\cdot1 + 6\cdot5 + 6\cdot0 & 0\cdot2 + 6\cdot7 + 6\cdot6 & 0\cdot4 + 6\cdot8 + 6\cdot8 
\end{pmatrix}.
$$

## 2. Determinants 2x2 and 3x3

#### 2x2 Matrices
For a 2x2 matrix 

$$ M = \begin{pmatrix} a & b \\ c & d \end{pmatrix} $$

, the determinant is calculated as:

$$
\text{det}(M) = ad - bc.
$$

1. For 

$$ A = \begin{pmatrix} 2 & 3 \\ 1 & 4 \end{pmatrix} $$

 =

$$
\text{det}(A) = (2)(4) - (3)(1) = 8 - 3 = 5.
$$

2. For 

$$ B = \begin{pmatrix} 5 & 6 \\ 7 & 8 \end{pmatrix} $$

 =

$$
\text{det}(B) = (5)(8) - (6)(7) = 40 - 42 = -2.
$$

3. For 

$$ C = \begin{pmatrix} -1 & 2 \\ 3 & 0 \end{pmatrix} $$

 =

$$
\text{det}(C) = (-1)(0) - (2)(3) = 0 - 6 = -6.
$$

---

#### 3x3 Matrices
For a 3x3 matrix 

$$ M = \begin{pmatrix} a & b & c \\ d & e & f \\ g & h & i \end{pmatrix} $$

, the determinant is:

$$
\text{det}(M) = a(ei - fh) - b(di - fg) + c(dh - eg).
$$

1. For 

$$ D = \begin{pmatrix} 1 & 0 & 2 \\ -1 & 3 & 1 \\ 2 & 4 & -2 \end{pmatrix} $$

=

$$
\text{det}(D) = 1(3(-2) - 1(4)) - 0(-1(-2) - 1(2)) + 2((-1)(4) - 3(2)),
$$

$$
\text{det}(D) = 1(-6 - 4) + 0 + 2(-4 - 6) = -10 - 20 = -30.
$$

2. For 

$$ E = \begin{pmatrix} 3 & 1 & -1 \\ 0 & 2 & 4 \\ 5 & 3 & 2 \end{pmatrix} $$

=

$$
\text{det}(E) = 3(2(2) - 4(3)) - 1(0(2) - 4(5)) + (-1)(0(3) - 2(5)),
$$

$$
\text{det}(E) = 3(4 - 12) - 1(0 - 20) + (-1)(0 - 10) = 3(-8) - (-20) - (-10) = -24 + 20 + 10 = 6.
$$

3. For 

$$ F = \begin{pmatrix} 2 & -3 & 1 \\ 1 & 4 & -2 \\ 1 & 5 & 3 \end{pmatrix} $$

=

$$
\text{det}(F) = 2(4(3) - (-2)(5)) - (-3)(1(3) - (-2)(1)) + 1(1(5) - 4(1)),
$$

$$
\text{det}(F) = 2(12 + 10) + 3(3 + 2) + 1(5 - 4) = 2(22) + 3(5) + 1(1) = 44 + 15 + 1 = 60.
$$

---

### Final Results
- **2x2 Matrices**:

$$ \text{det}(A) = 5 $$

$$ \text{det}(B) = -2 $$

$$ \text{det}(C) = -6 $$

- **3x3 Matrices**:

$$ \text{det}(D) = -30 $$

$$ \text{det}(E) = 6 $$

$$ \text{det}(F) = 60 $$
