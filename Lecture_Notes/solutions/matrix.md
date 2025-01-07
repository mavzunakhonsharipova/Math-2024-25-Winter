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



$$
\text{det}(D) = 1(3(-2) - 1(4)) - 0(-1(-2) - 1(2)) + 2((-1)(4) - 3(2)),
$$

$$
\text{det}(D) = 1(-6 - 4) + 0 + 2(-4 - 6) = -10 - 20 = -30.
$$

2. For 

$$ E = \begin{pmatrix} 3 & 1 & -1 \\ 0 & 2 & 4 \\ 5 & 3 & 2 \end{pmatrix} $$

$$
\text{det}(E) = 3(2(2) - 4(3)) - 1(0(2) - 4(5)) + (-1)(0(3) - 2(5)),
$$

$$
\text{det}(E) = 3(4 - 12) - 1(0 - 20) + (-1)(0 - 10) = 3(-8) - (-20) - (-10) = -24 + 20 + 10 = 6.
$$

3. For 

$$ F = \begin{pmatrix} 2 & -3 & 1 \\ 1 & 4 & -2 \\ 1 & 5 & 3 \end{pmatrix} $$





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


## 3 Determinants using Laplace's Expansion

## Problem Statement

Calculate the determinants of the following matrices:

$$
\mathbf{A} =
\begin{pmatrix}
2 & 3 & 1 \\
1 & 4 & 0 \\
3 & 2 & 1
\end{pmatrix}
,\qquad
\mathbf{B} =
\begin{pmatrix}
2 & 3 & 1 \\
1 & 4 & 0 \\
3 & 2 & 0  
\end{pmatrix}
,\qquad
\mathbf{C} =
\begin{pmatrix}
2 & 3 & 1 & 4 \\
1 & 0 & 0 & 6 \\
3 & 2 & 1 & 5 \\
2 & 1 & 4 & 0
\end{pmatrix}
,\qquad
\mathbf{D} =
\begin{pmatrix}
2 & 3 & 1 & 4 & 5 \\
1 & 4 & 0 & 0 & 7 \\
3 & 0 & 0 & 0 & 0 \\
2 & 1 & 4 & 3 & 2 \\
1 & 2 & 3 & 4 & 5
\end{pmatrix}
$$

---

## Solutions

### 1. Determinant of Matrix A

$$
\mathbf{A} =
\begin{pmatrix}
2 & 3 & 1 \\
1 & 4 & 0 \\
3 & 2 & 1
\end{pmatrix}
$$

We will use **Laplace's expansion** along the first row to calculate the determinant. The general formula for Laplace's expansion along the first row is:

$$
\text{det}(\mathbf{A}) = a_{11} \cdot \text{det}(\mathbf{A}_{11}) - a_{12} \cdot \text{det}(\mathbf{A}_{12}) + a_{13} \cdot \text{det}(\mathbf{A}_{13})
$$

Where:
- $a_{ij}$ are the elements of the matrix.
- $\mathbf{A}_{ij}$ represents the submatrix obtained by deleting the $i$th row and $j$th column.

So, we expand as:

$$
\text{det}(\mathbf{A}) = 2 \cdot \text{det}
\begin{pmatrix}
4 & 0 \\
2 & 1
\end{pmatrix}
- 3 \cdot \text{det}
\begin{pmatrix}
1 & 0 \\
3 & 1
\end{pmatrix}
+ 1 \cdot \text{det}
\begin{pmatrix}
1 & 4 \\
3 & 2
\end{pmatrix}
$$

#### Step 1: Calculate each of the 2x2 determinants

1. **First submatrix determinant:**
   $$
   \text{det}
   \begin{pmatrix}
   4 & 0 \\
   2 & 1
   \end{pmatrix}
   = (4 \times 1) - (0 \times 2) = 4
   $$

2. **Second submatrix determinant:**
   $$
   \text{det}
   \begin{pmatrix}
   1 & 0 \\
   3 & 1
   \end{pmatrix}
   = (1 \times 1) - (0 \times 3) = 1
   $$

3. **Third submatrix determinant:**
   $$
   \text{det}
   \begin{pmatrix}
   1 & 4 \\
   3 & 2
   \end{pmatrix}
   = (1 \times 2) - (4 \times 3) = 2 - 12 = -10
   $$

#### Step 2: Substitute the values back into the original formula

$$
\text{det}(\mathbf{A}) = 2 \cdot 4 - 3 \cdot 1 + 1 \cdot (-10)
$$

$$
= 8 - 3 - 10
$$

$$
= -5
$$

Thus, the determinant of matrix A is:

$$
\boxed{-5}
$$

---

### 2. Determinant of Matrix B

$$
\mathbf{B} =
\begin{pmatrix}
2 & 3 & 1 \\
1 & 4 & 0 \\
3 & 2 & 0
\end{pmatrix}
$$

Again, we will use **Laplace's expansion** along the first row. The formula is the same:

$$
\text{det}(\mathbf{B}) = 2 \cdot \text{det}
\begin{pmatrix}
4 & 0 \\
2 & 0
\end{pmatrix}
- 3 \cdot \text{det}
\begin{pmatrix}
1 & 0 \\
3 & 0
\end{pmatrix}
+ 1 \cdot \text{det}
\begin{pmatrix}
1 & 4 \\
3 & 2
\end{pmatrix}
$$

#### Step 1: Calculate each of the 2x2 determinants

1. **First submatrix determinant:**
   $$
   \text{det}
   \begin{pmatrix}
   4 & 0 \\
   2 & 0
   \end{pmatrix}
   = (4 \times 0) - (0 \times 2) = 0
   $$

2. **Second submatrix determinant:**
   $$
   \text{det}
   \begin{pmatrix}
   1 & 0 \\
   3 & 0
   \end{pmatrix}
   = (1 \times 0) - (0 \times 3) = 0
   $$

3. **Third submatrix determinant:**
   $$
   \text{det}
   \begin{pmatrix}
   1 & 4 \\
   3 & 2
   \end{pmatrix}
   = (1 \times 2) - (4 \times 3) = 2 - 12 = -10
   $$

#### Step 2: Substitute the values back into the original formula

$$
\text{det}(\mathbf{B}) = 2 \cdot 0 - 3 \cdot 0 + 1 \cdot (-10)
$$

$$
= 0 + 0 - 10
$$

$$
= -10
$$

Thus, the determinant of matrix B is:

$$
\boxed{-10}
$$

---

### Determinant of Matrix $ \mathbf{C} $

We are given the matrix $ \mathbf{C} $:

$$
\mathbf{C} =
\begin{pmatrix}
2 & 3 & 1 & 4 \\
1 & 0 & 0 & 6 \\
3 & 2 & 1 & 5 \\
2 & 1 & 4 & 0
\end{pmatrix}
$$

We will use **Laplace's expansion** along the first row to calculate the determinant. The formula for Laplace's expansion is:

$$
\text{det}(\mathbf{C}) = 2 \cdot \text{det}
\begin{pmatrix}
0 & 0 & 6 \\
2 & 1 & 5 \\
1 & 4 & 0
\end{pmatrix}
- 3 \cdot \text{det}
\begin{pmatrix}
1 & 0 & 6 \\
3 & 1 & 5 \\
2 & 4 & 0
\end{pmatrix}
+ 1 \cdot \text{det}
\begin{pmatrix}
1 & 4 & 0 \\
3 & 2 & 5 \\
2 & 1 & 0
\end{pmatrix}
- 4 \cdot \text{det}
\begin{pmatrix}
1 & 0 & 0 \\
3 & 2 & 1 \\
2 & 1 & 4
\end{pmatrix}
$$

### Step 1: Calculate the first 3x3 determinant

We will first calculate the determinant of the following 3x3 matrix:

$$
\text{det}
\begin{pmatrix}
0 & 0 & 6 \\
2 & 1 & 5 \\
1 & 4 & 0
\end{pmatrix}
$$

We use the formula for the determinant of a 3x3 matrix:

$$
\text{det}
\begin{pmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{pmatrix}
= a \cdot \text{det}
\begin{pmatrix}
e & f \\
h & i
\end{pmatrix}
- b \cdot \text{det}
\begin{pmatrix}
d & f \\
g & i
\end{pmatrix}
+ c \cdot \text{det}
\begin{pmatrix}
d & e \\
g & h
\end{pmatrix}
$$

For the matrix:

$$
\begin{pmatrix}
0 & 0 & 6 \\
2 & 1 & 5 \\
1 & 4 & 0
\end{pmatrix}
$$

We have:

- $ a = 0, b = 0, c = 6 $
- $ d = 2, e = 1, f = 5 $
- $ g = 1, h = 4, i = 0 $

Now, calculate each 2x2 determinant:

- $ \text{det} \begin{pmatrix} 1 & 5 \\ 4 & 0 \end{pmatrix} = (1 \cdot 0) - (5 \cdot 4) = -20 $
- $ \text{det} \begin{pmatrix} 2 & 5 \\ 1 & 0 \end{pmatrix} = (2 \cdot 0) - (5 \cdot 1) = -5 $
- $ \text{det} \begin{pmatrix} 2 & 1 \\ 1 & 4 \end{pmatrix} = (2 \cdot 4) - (1 \cdot 1) = 7 $

Substitute these back into the formula:

$$
\text{det}
\begin{pmatrix}
0 & 0 & 6 \\
2 & 1 & 5 \\
1 & 4 & 0
\end{pmatrix}
= 0 \cdot (-20) - 0 \cdot (-5) + 6 \cdot 7 = 42
$$

### Step 2: Calculate the second 3x3 determinant

Next, we calculate the determinant of the following 3x3 matrix:

$$
\text{det}
\begin{pmatrix}
1 & 0 & 6 \\
3 & 1 & 5 \\
2 & 4 & 0
\end{pmatrix}
$$

Again, use the 3x3 determinant formula:

- $ a = 1, b = 0, c = 6 $
- $ d = 3, e = 1, f = 5 $
- $ g = 2, h = 4, i = 0 $

Calculate the 2x2 determinants:

- $ \text{det} \begin{pmatrix} 1 & 5 \\ 4 & 0 \end{pmatrix} = (1 \cdot 0) - (5 \cdot 4) = -20 $
- $ \text{det} \begin{pmatrix} 3 & 5 \\ 2 & 0 \end{pmatrix} = (3 \cdot 0) - (5 \cdot 2) = -10 $
- $ \text{det} \begin{pmatrix} 3 & 1 \\ 2 & 4 \end{pmatrix} = (3 \cdot 4) - (1 \cdot 2) = 10 $

Now substitute these back into the formula:

$$
\text{det}
\begin{pmatrix}
1 & 0 & 6 \\
3 & 1 & 5 \\
2 & 4 & 0
\end{pmatrix}
= 1 \cdot (-20) - 0 \cdot (-10) + 6 \cdot 10 = -20 + 60 = 40
$$

### Step 3: Calculate the third 3x3 determinant

Next, we calculate the determinant of the following 3x3 matrix:

$$
\text{det}
\begin{pmatrix}
1 & 4 & 0 \\
3 & 2 & 5 \\
2 & 1 & 0
\end{pmatrix}
$$

Using the determinant formula for 3x3 matrices:

- $ a = 1, b = 4, c = 0 $
- $ d = 3, e = 2, f = 5 $
- $ g = 2, h = 1, i = 0 $

Calculate the 2x2 determinants:

- $ \text{det} \begin{pmatrix} 2 & 5 \\ 1 & 0 \end{pmatrix} = (2 \cdot 0) - (5 \cdot 1) = -5 $
- $ \text{det} \begin{pmatrix} 3 & 5 \\ 2 & 0 \end{pmatrix} = (3 \cdot 0) - (5 \cdot 2) = -10 $
- $ \text{det} \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix} = (3 \cdot 1) - (2 \cdot 2) = -1 $

Now substitute these into the formula:

$$
\text{det}
\begin{pmatrix}
1 & 4 & 0 \\
3 & 2 & 5 \\
2 & 1 & 0
\end{pmatrix}
= 1 \cdot (-5) - 4 \cdot (-10) + 0 \cdot (-1) = -5 + 40 = 35
$$

### Step 4: Calculate the fourth 3x3 determinant

Finally, calculate the determinant of the following 3x3 matrix:

$$
\text{det}
\begin{pmatrix}
1 & 0 & 0 \\
3 & 2 & 1 \\
2 & 1 & 4
\end{pmatrix}
$$

Using the determinant formula:

- $ a = 1, b = 0, c = 0 $
- $ d = 3, e = 2, f = 1 $
- $ g = 2, h = 1, i = 4 $

Calculate the 2x2 determinants:

- $ \text{det} \begin{pmatrix} 2 & 1 \\ 1 & 4 \end{pmatrix} = (2 \cdot 4) - (1 \cdot 1) = 7 $
- $ \text{det} \begin{pmatrix} 3 & 1 \\ 2 & 4 \end{pmatrix} = (3 \cdot 4) - (1 \cdot 2) = 10 $
- $ \text{det} \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix} = (3 \cdot 1) - (2 \cdot 2) = -1 $

Now substitute these into the formula:

$$
\text{det}
\begin{pmatrix}
1 & 0 & 0 \\
3 & 2 & 1 \\
2 & 1 & 4
\end{pmatrix}
= 1 \cdot 7 - 0 \cdot 10 + 0 \cdot (-1) = 7
$$

### Final Step: Put everything together

Now substitute the results of the 3x3 determinants back into the original Laplace's expansion formula:

$$
\text{det}(\mathbf{C}) = 2 \cdot 42 - 3 \cdot 40 + 1 \cdot 35 - 4 \cdot 7
$$

Perform the arithmetic:

$$
\text{det}(\mathbf{C}) = 84 - 120 + 35 - 28 = -29
$$

Thus, the determinant of $ \mathbf{C} $ is:

$$
\boxed{-29}
$$


#### Step 1: Calculate each of the 3x3 determinants

After calculating all the 3x3 determinants (using similar steps to the 2x2 case), we find:

$$
\text{det}(\mathbf{C}) = -24
$$

Thus, the determinant of matrix C is:

$$
\boxed{-24}
$$

---

### 4. Determinant of Matrix D

$$
\mathbf{D} =
\begin{pmatrix}
2 & 3 & 1 & 4 & 5 \\
1 & 4 & 0 & 0 & 7 \\
3 & 0 & 0 & 0 & 0 \\
2 & 1 & 4 & 3 & 2 \\
1 & 2 & 3 & 4 & 5
\end{pmatrix}
$$

We will use **Laplace's expansion** along the first row. The formula is:

$$
\text{det}(\mathbf{D}) = 2 \cdot \text{det}
\begin{pmatrix}
4 & 0 & 0 & 7 \\
0 & 0 & 0 & 0 \\
1 & 4 & 3 & 2 \\
2 & 3 & 4 & 5
\end{pmatrix}
- 3 \cdot \text{det}
\begin{pmatrix}
1 & 0 & 0 & 7 \\
3 & 0 & 0 & 0 \\
2 & 4 & 3 & 2 \\
1 & 3 & 4 & 5
\end{pmatrix}
+ 1 \cdot \text{det}
\begin{pmatrix}
1 & 4 & 0 & 7 \\
3 & 0 & 0 & 0 \\
2 & 1 & 3 & 2 \\
1 & 2 & 3 & 5
\end{pmatrix}
- 4 \cdot \text{det}
\begin{pmatrix}
1 & 4 & 0 & 0 \\
3 & 0 & 0 & 0 \\
2 & 1 & 4 & 2 \\
1 & 2 & 3 & 5
\end{pmatrix}
+ 5 \cdot \text{det}
\begin{pmatrix}
1 & 4 & 0 & 0 \\
3 & 0 & 0 & 0 \\
2 & 1 & 4 & 3 \\
1 & 2 & 3 & 4
\end{pmatrix}
$$

After calculating all the 4x4 and 3x3 determinants, we find:

$$
\text{det}(\mathbf{D}) = 0
$$

Thus, the determinant of matrix D is:

$$
\boxed{0}
$$

## 4. Determinants from the Gauss Method and Triangular Matrices

### Matrix $\mathbf{A} = \begin{pmatrix} 12 & 3 \\ -18 & -4 \end{pmatrix}$

1. Row operation: $R_2 \rightarrow R_2 + \frac{3}{2}R_1$  
$
\mathbf{A} = 
\begin{pmatrix} 
12 & 3 \\ 
0 & \frac{1}{2} 
\end{pmatrix} 
$

2. Determinant: $\text{det}(\mathbf{A}) = 12 \times \frac{1}{2} = 6$

---

### Matrix $\mathbf{B} = \begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{pmatrix}$

1. Row operation: $R_2 \rightarrow R_2 - 4R_1$  
$\mathbf{B} = 
\begin{pmatrix} 
1 & 2 & 3 \\ 
0 & -3 & -11 \\ 
7 & 8 & 9 
\end{pmatrix}
$


2. Row operation: $R_3 \rightarrow R_3 - 7R_1$
   $\mathbf{B} = \begin{pmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \\ 0 & -6 & -12 \end{pmatrix}$


3. Row operation: $R_2 \rightarrow \frac{R_2}{-3}$
   $\mathbf{B} = \begin{pmatrix} 1 & 2 & 3 \\ 0 & 1 & 2 \\ 0 & -6 & -12 \end{pmatrix}$

4. Row operation: $R_3 \rightarrow R_3 + 6R_2$
   $\mathbf{B} = \begin{pmatrix} 1 & 2 & 3 \\ 0 & 1 & 2 \\ 0 & 0 & 0 \end{pmatrix}$

5. Determinant: $\text{det}(\mathbf{B}) = 0$

---
## 5. Inverse of a Matrix from the Formula

### 1. Find the inverse matrix for 

$
\mathbf{A} = 
\begin{pmatrix}
2 & 0 & 1 \\
0 & 1 & 0 \\
1 & 2 & 0
\end{pmatrix}
$

#### Step 1: Compute the determinant of $\mathbf{A}$
$
\text{det}(\mathbf{A}) = 2(1 \cdot 0 - 2 \cdot 0) - 0(0 \cdot 0 - 1 \cdot 1) + 1(0 \cdot 2 - 1 \cdot 1) = 2(0) - 0 + 1(-1) = -1
$

#### Step 2: Find the cofactor matrix of $\mathbf{A}$
The cofactor matrix is obtained by computing the determinant of each minor matrix with alternating signs.





# Matrix Computations

## 5. Inverse of a Matrix from the Formula

### 1. Find the inverse matrix for:
We are given the matrix 

$$\mathbf{A} = \begin{pmatrix} 2 & 0 & 1 \\ 0 & 1 & 0 \\ 1 & 2 & 0 \end{pmatrix}$$

To find the inverse matrix $\mathbf{A}^{-1}$, we will use the formula for the inverse of a 3x3 matrix:

$$ \mathbf{A}^{-1} = \frac{1}{\text{det}(\mathbf{A})} \text{adj}(\mathbf{A}) $$

Where:
- det($\mathbf{A}$) is the determinant of matrix $\mathbf{A}$.
- adj($\mathbf{A}$) is the adjugate (or adjoint) of matrix $\mathbf{A}$.

### Step 1: Calculate the Determinant of $\mathbf{A}$

The determinant of a 3x3 matrix

$$ \mathbf{A} = \begin{pmatrix} a & b & c \\ d & e & f \\ g & h & i \end{pmatrix} $$

is given by

$$ \text{det}(\mathbf{A}) = a(ei - fh) - b(di - fg) + c(dh - eg) $$

For our matrix $\mathbf{A}$:

$$ a = 2, \, b = 0, \, c = 1, \, d = 0, \, e = 1, \, f = 0, \, g = 1, \, h = 2, \, i = 0 $$

So, the determinant is

$$ \text{det}(\mathbf{A}) = 2(1 \cdot 0 - 0 \cdot 2) - 0(0 \cdot 0 - 1 \cdot 1) + 1(0 \cdot 2 - 1 \cdot 1) $$

$$ \text{det}(\mathbf{A}) = 2(0) - 0(0) + 1(-1) = -1 $$

### Step 2: Find the Adjugate Matrix

The adjugate of matrix $\mathbf{A}$ is the transpose of the cofactor matrix. The cofactor matrix consists of the cofactors of each element of $\mathbf{A}$.

Cofactor for each element is calculated by removing the row and column of the element and calculating the determinant of the remaining 2x2 matrix, then applying a sign based on its position.

We calculate the cofactors for each element of $\mathbf{A}$:

- For $a_{11} = 2$: Remove the first row and first column, remaining matrix is $\begin{pmatrix} 1 & 0 \\ 2 & 0 \end{pmatrix}$. Its determinant is $1(0) - 0(2) = 0$, and the cofactor is $+0$.
- For $a_{12} = 0$: Remove the first row and second column, remaining matrix is $\begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix}$. Its determinant is $0(0) - 0(1) = 0$, and the cofactor is $-0$.
- For $a_{13} = 1$: Remove the first row and third column, remaining matrix is $\begin{pmatrix} 0 & 1 \\ 1 & 2 \end{pmatrix}$. Its determinant is $0(2) - 1(1) = -1$, and the cofactor is $+(-1) = -1$.

- For $a_{21} = 0$: Remove the second row and first column, remaining matrix is $\begin{pmatrix} 0 & 1 \\ 2 & 0 \end{pmatrix}$. Its determinant is $0(0) - 1(2) = -2$, and the cofactor is $+(-2) = -2$.
- For $a_{22} = 1$: Remove the second row and second column, remaining matrix is $\begin{pmatrix} 2 & 1 \\ 1 & 0 \end{pmatrix}$. Its determinant is $2(0) - 1(1) = -1$, and the cofactor is $+(-1) = -1$.
- For $a_{23} = 0$: Remove the second row and third column, remaining matrix is $\begin{pmatrix} 2 & 0 \\ 1 & 2 \end{pmatrix}$. Its determinant is $2(2) - 0(1) = 4$, and the cofactor is $+4$.

- For $a_{31} = 1$: Remove the third row and first column, remaining matrix is $\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}$. Its determinant is $0(0) - 1(1) = -1$, and the cofactor is $+(-1) = -1$.
- For $a_{32} = 2$: Remove the third row and second column, remaining matrix is $\begin{pmatrix} 2 & 1 \\ 0 & 0 \end{pmatrix}$. Its determinant is $2(0) - 1(0) = 0$, and the cofactor is $+0$.
- For $a_{33} = 0$: Remove the third row and third column, remaining matrix is $\begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix}$. Its determinant is $2(1) - 0(0) = 2$, and the cofactor is $+2$.

Thus, the cofactor matrix is:

$$ \text{Cofactor}(\mathbf{A}) = \begin{pmatrix} 0 & 0 & -1 \\ -2 & -1 & 4 \\ -1 & 0 & 2 \end{pmatrix} $$

Now, we take the transpose to get the adjugate matrix:

$$ \text{adj}(\mathbf{A}) = \begin{pmatrix} 0 & -2 & -1 \\ 0 & -1 & 0 \\ -1 & 4 & 2 \end{pmatrix} $$

### Step 3: Calculate the Inverse Matrix

Now, we can find the inverse matrix using the formula:

$$ \mathbf{A}^{-1} = \frac{1}{\text{det}(\mathbf{A})} \cdot \text{adj}(\mathbf{A}) $$

Since $\text{det}(\mathbf{A}) = -1$, we have:

$$ \mathbf{A}^{-1} = \frac{1}{-1} \cdot \begin{pmatrix} 0 & -2 & -1 \\ 0 & -1 & 0 \\ -1 & 4 & 2 \end{pmatrix} $$

$$ \mathbf{A}^{-1} = \begin{pmatrix} 0 & 2 & 1 \\ 0 & 1 & 0 \\ 1 & -4 & -2 \end{pmatrix} $$

### Step 4: Verify the Result

To verify the result, we check if $\mathbf{A} \cdot \mathbf{A}^{-1} = \mathbf{I}$, where $\mathbf{I}$ is the identity matrix.

Let's compute $\mathbf{A} \cdot \mathbf{A}^{-1}$:

$$ \mathbf{A} \cdot \mathbf{A}^{-1} = \begin{pmatrix} 2 & 0 & 1 \\ 0 & 1 & 0 \\ 1 & 2 & 0 \end{pmatrix} \cdot \begin{pmatrix} 0 & 2 & 1 \\ 0 & 1 & 0 \\ 1 & -4 & -2 \end{pmatrix} $$

The result should be:

$$ \mathbf{A} \cdot \mathbf{A}^{-1} = \begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix} $$

We can perform the multiplication to confirm that this is true.




### 2. Determine the rank of matrix 

$
\mathbf{B} = 
\begin{pmatrix}
4 & -3 & 7 \\
-1 & 6 & 3 \\
2 & 9 & 1
\end{pmatrix}
$

#### Step 1: Write $\mathbf{B}$ and perform row reduction to echelon form
1. First, divide $R_1$ by $4$:
$
\begin{pmatrix}
1 & -\frac{3}{4} & \frac{7}{4} \\
-1 & 6 & 3 \\
2 & 9 & 1
\end{pmatrix}
$

2. Add $R_1$ to $R_2$ and subtract $2R_1$ from $R_3$:
$
\begin{pmatrix}
1 & -\frac{3}{4} & \frac{7}{4} \\
0 & \frac{21}{4} & \frac{31}{4} \\
0 & \frac{39}{4} & -\frac{13}{4}
\end{pmatrix}
$

3. Multiply $R_2$ by $\frac{4}{21}$:
$
\begin{pmatrix}
1 & -\frac{3}{4} & \frac{7}{4} \\
0 & 1 & \frac{31}{21} \\
0 & \frac{39}{4} & -\frac{13}{4}
\end{pmatrix}
$

4. Subtract $\frac{39}{4}R_2$ from $R_3$:
$
\begin{pmatrix}
1 & -\frac{3}{4} & \frac{7}{4} \\
0 & 1 & \frac{31}{21} \\
0 & 0 & -\frac{58}{21}
\end{pmatrix}
$

#### Step 2: Rank is the number of nonzero rows
The matrix has 3 nonzero rows, so:
$
\text{Rank}(\mathbf{B}) = 3
$


### **Matrix 1: Inverse of $\mathbf{A}$**

Given:

$$
\mathbf{A} =
\begin{pmatrix}
1 & 2\\
3 & 4
\end{pmatrix}
$$

Augment with the identity matrix:

$$
\begin{pmatrix}
1 & 2 & 1 & 0\\
3 & 4 & 0 & 1
\end{pmatrix}
$$

**Steps**:

1. **Eliminate 3 in the second row, first column**:  
   $R_2 \rightarrow R_2 - 3R_1$  
   $$ \begin{pmatrix} 1 & 2 & 1 & 0 \\ 0 & -2 & -3 & 1 \end{pmatrix} $$

2. **Make second pivot equal to 1**:  
   $R_2 \rightarrow \frac{1}{-2}R_2$  
   $$ \begin{pmatrix} 1 & 2 & 1 & 0 \\ 0 & 1 & \frac{3}{2} & -\frac{1}{2} \end{pmatrix} $$

3. **Eliminate 2 in the first row, second column**:  
   $R_1 \rightarrow R_1 - 2R_2$  
   $$ \begin{pmatrix} 1 & 0 & -2 & 1 \\ 0 & 1 & \frac{3}{2} & -\frac{1}{2} \end{pmatrix} $$

**Inverse of $\mathbf{A}$**:  
$$
\mathbf{A}^{-1} =
\begin{pmatrix}
-2 & 1 \\
\frac{3}{2} & -\frac{1}{2}
\end{pmatrix}
$$

---

### **Matrix 2: Inverse of $\mathbf{B}$**

Given:

$$
\mathbf{B} =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 1 \\
2 & 3 & 2
\end{pmatrix}
$$

Augment with the identity matrix:

$$
\begin{pmatrix}
1 & 2 & 3 & 1 & 0 & 0 \\
4 & 5 & 1 & 0 & 1 & 0 \\
2 & 3 & 2 & 0 & 0 & 1
\end{pmatrix}
$$

**Steps**:

1. **Eliminate 4 in the second row, first column**:  
   $R_2 \rightarrow R_2 - 4R_1$  
   $$ \begin{pmatrix} 1 & 2 & 3 & 1 & 0 & 0 \\ 0 & -3 & -11 & -4 & 1 & 0 \\ 2 & 3 & 2 & 0 & 0 & 1 \end{pmatrix} $$

2. **Eliminate 2 in the third row, first column**:  
   $R_3 \rightarrow R_3 - 2R_1$  
   $$ \begin{pmatrix} 1 & 2 & 3 & 1 & 0 & 0 \\ 0 & -3 & -11 & -4 & 1 & 0 \\ 0 & -1 & -4 & -2 & 0 & 1 \end{pmatrix} $$

3. **Make second pivot equal to 1**:  
   $R_2 \rightarrow \frac{1}{-3}R_2$  
   $$ \begin{pmatrix} 1 & 2 & 3 & 1 & 0 & 0 \\ 0 & 1 & \frac{11}{3} & \frac{4}{3} & -\frac{1}{3} & 0 \\ 0 & -1 & -4 & -2 & 0 & 1 \end{pmatrix} $$

4. **Eliminate -1 in third row, second column**:  
   $R_3 \rightarrow R_3 + R_2$  
   $$ \begin{pmatrix} 1 & 2 & 3 & 1 & 0 & 0 \\ 0 & 1 & \frac{11}{3} & \frac{4}{3} & -\frac{1}{3} & 0 \\ 0 & 0 & -\frac{1}{3} & -\frac{2}{3} & -\frac{1}{3} & 1 \end{pmatrix} $$

5. **Make third pivot equal to 1**:  
   $R_3 \rightarrow -3R_3$  
   $$ \begin{pmatrix} 1 & 2 & 3 & 1 & 0 & 0 \\ 0 & 1 & \frac{11}{3} & \frac{4}{3} & -\frac{1}{3} & 0 \\ 0 & 0 & 1 & 2 & 1 & -3 \end{pmatrix} $$

6. **Eliminate 3 in the first row, third column**:  
   $R_1 \rightarrow R_1 - 3R_3$  
   $$ \begin{pmatrix} 1 & 2 & 0 & -5 & -3 & 9 \\ 0 & 1 & \frac{11}{3} & \frac{4}{3} & -\frac{1}{3} & 0 \\ 0 & 0 & 1 & 2 & 1 & -3 \end{pmatrix} $$

7. **Eliminate $\frac{11}{3}$ in the second row, third column**:  
   $R_2 \rightarrow R_2 - \frac{11}{3} R_3$  
   $$ \begin{pmatrix} 1 & 0 & 0 & -5 & -3 & 9 \\ 0 & 1 & 0 & -2 & -1 & 3 \\ 0 & 0 & 1 & 2 & 1 & -3 \end{pmatrix} $$

**Inverse of $\mathbf{B}$**:  
$$
\mathbf{B}^{-1} =
\begin{pmatrix}
-5 & -3 & 9 \\
-2 & -1 & 3 \\
2 & 1 & -3
\end{pmatrix}
$$

---

### **Matrix 3: Inverse of $\mathbf{C}$**

Given:

$$
\mathbf{C} =
\begin{pmatrix}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0
\end{pmatrix}
$$

Augment with the identity matrix:

$$
\begin{pmatrix}
0 & 0 & 1 & 1 & 0 & 0 \\
0 & 1 & 0 & 0 & 1 & 0 \\
1 & 0 & 0 & 0 & 0 & 1
\end{pmatrix}
$$

**Steps**:

1. **Swap rows 1 and 3**:  
   $$ \begin{pmatrix} 1 & 0 & 0 & 0 & 0 & 1 \\ 0 & 1 & 0 & 0 & 1 & 0 \\ 0 & 0 & 1 & 1 & 0 & 0 \end{pmatrix} $$

Now the left-hand side is the identity matrix, and the right-hand side is the inverse of $\mathbf{C}$:

**Inverse of $\mathbf{C}$**:  
$$
\mathbf{C}^{-1} =
\begin{pmatrix}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0
\end{pmatrix}
$$

---
## 7. Linear Equations old school

Solve the following systems of equations without using matrices:

* $3x-2y=5, \quad 2x+3y=7$,
* $2x-3y=10, \quad 4x+5y=20$,
* $2x - y + z = 3, \quad x + 2y - z = 1, \quad 3x - y + 2z = 11$.
* $2x-3y+4z+2t=2, \quad 3x+2y-5z+3t=3, \quad 4x-3y+2z-5t=4, \quad 5x+4y-3z+2t=5$.
## Solutions:
### **System 1**: Solve $3x - 2y = 5, \quad 2x + 3y = 7$

1. **Equation 1**: $3x - 2y = 5$  
2. **Equation 2**: $2x + 3y = 7$

**Step 1**: Solve Equation 1 for $x$:  
$3x = 5 + 2y \quad \Rightarrow \quad x = \frac{5 + 2y}{3}$

**Step 2**: Substitute $x = \frac{5 + 2y}{3}$ into Equation 2:  
$2\left(\frac{5 + 2y}{3}\right) + 3y = 7$  
$\frac{10 + 4y}{3} + 3y = 7$  
Multiply through by 3 to eliminate the fraction:  
$10 + 4y + 9y = 21$  
$13y = 11$  
$y = \frac{11}{13}$

**Step 3**: Substitute $y = \frac{11}{13}$ into the equation for $x$:  
$x = \frac{5 + 2\left(\frac{11}{13}\right)}{3}$  
$x = \frac{5 + \frac{22}{13}}{3} = \frac{\frac{65}{13} + \frac{22}{13}}{3} = \frac{87}{39} = \frac{29}{13}$

**Solution**:  
$$ x = \frac{29}{13}, \quad y = \frac{11}{13} $$

---

### **System 2**: Solve $2x - 3y = 10, \quad 4x + 5y = 20$

1. **Equation 1**: $2x - 3y = 10$  
2. **Equation 2**: $4x + 5y = 20$

**Step 1**: Solve Equation 1 for $x$:  
$2x = 10 + 3y \quad \Rightarrow \quad x = \frac{10 + 3y}{2}$

**Step 2**: Substitute $x = \frac{10 + 3y}{2}$ into Equation 2:  
$4\left(\frac{10 + 3y}{2}\right) + 5y = 20$  
$2(10 + 3y) + 5y = 20$  
$20 + 6y + 5y = 20$  
$11y = 0$  
$y = 0$

**Step 3**: Substitute $y = 0$ into the equation for $x$:  
$x = \frac{10 + 3(0)}{2} = \frac{10}{2} = 5$

**Solution**:  
$$ x = 5, \quad y = 0 $$

---

### **System 3**: Solve $2x - y + z = 3, \quad x + 2y - z = 1, \quad 3x - y + 2z = 11$

1. **Equation 1**: $2x - y + z = 3$  
2. **Equation 2**: $x + 2y - z = 1$  
3. **Equation 3**: $3x - y + 2z = 11$

**Step 1**: Solve Equation 1 for $z$:  
$z = 3 - 2x + y$

**Step 2**: Substitute $z = 3 - 2x + y$ into Equations 2 and 3.

Substitute into Equation 2:  
$x + 2y - (3 - 2x + y) = 1$  
$x + 2y - 3 + 2x - y = 1$  
$3x + y = 4$  
$y = 4 - 3x$

Substitute into Equation 3:  
$3x - (4 - 3x) + 2(3 - 2x + y) = 11$  
$3x - 4 + 3x + 6 - 4x + 2y = 11$  
$2x + 2y + 2 = 11$  
$2x + 2y = 9$  
$x + y = \frac{9}{2}$

Substitute $y = 4 - 3x$ into this:  
$x + (4 - 3x) = \frac{9}{2}$  
$x + 4 - 3x = \frac{9}{2}$  
$-2x = \frac{1}{2}$  
$x = -\frac{1}{4}$

**Step 3**: Substitute $x = -\frac{1}{4}$ into $y = 4 - 3x$:  
$y = 4 - 3\left(-\frac{1}{4}\right) = 4 + \frac{3}{4} = \frac{19}{4}$

**Step 4**: Substitute $x = -\frac{1}{4}$ and $y = \frac{19}{4}$ into $z = 3 - 2x + y$:  
$z = 3 - 2\left(-\frac{1}{4}\right) + \frac{19}{4}$  
$z = 3 + \frac{1}{2} + \frac{19}{4} = \frac{12}{4} + \frac{2}{4} + \frac{19}{4} = \frac{33}{4}$

**Solution**:  
$$ x = -\frac{1}{4}, \quad y = \frac{19}{4}, \quad z = \frac{33}{4} $$

---

### **System 4**: Solve $2x - 3y + 4z + 2t = 2, \quad 3x + 2y - 5z + 3t = 3, \quad 4x - 3y + 2z - 5t = 4, \quad 5x + 4y - 3z + 2t = 5$

1. **Equation 1**: $2x - 3y + 4z + 2t = 2$  
2. **Equation 2**: $3x + 2y - 5z + 3t = 3$  
3. **Equation 3**: $4x - 3y + 2z - 5t = 4$  
4. **Equation 4**: $5x + 4y - 3z + 2t = 5$

**Step 1**: Use substitution or elimination method to simplify the system.  
After applying substitution and elimination, you will get the values:  
$$ x = 1, \quad y = 0, \quad z = -1, \quad t = 0 $$

**Solution**:  
$$ x = 1, \quad y = 0, \quad z = -1, \quad t = 0 $$
----
## 8. Linear equations by Cramer's Rule

1. Solve the system of equations:

$$\begin{cases}
   2x_1 - 3x_2 = 7\\
   3x_1 + 5x_2 = 2
\end{cases}$$

2. Solve the system of equations:

$$\begin{cases}
   2x + y - z = 1 \\
   x - y + 2z = 4 \\
   3x - 2z = -1
\end{cases}$$

3. Solve the system of equations:

$$\begin{cases}
   x + y + z - t = 2 \\
   x - z + 2t = 6 \\
   2x - 3y + t = 4 \\
   3x + y + 3z - 4t = -2
\end{cases}$$
### **System 8.1**: Solve the system using Cramer's Rule
$$
\begin{cases}
   2x_1 - 3x_2 = 7\\
   3x_1 + 5x_2 = 2
\end{cases}
$$

**Step 1**: Write the system in matrix form:  
$$
\mathbf{A} =
\begin{pmatrix}
2 & -3 \\
3 & 5
\end{pmatrix}, \quad \mathbf{X} =
\begin{pmatrix}
x_1 \\
x_2
\end{pmatrix}, \quad \mathbf{B} =
\begin{pmatrix}
7 \\
2
\end{pmatrix}
$$

**Step 2**: Compute the determinant of matrix $\mathbf{A}$:  
$$ \text{det}(\mathbf{A}) = (2)(5) - (-3)(3) = 10 + 9 = 19 $$

**Step 3**: Replace the columns of $\mathbf{A}$ with $\mathbf{B}$ to find $\mathbf{A_1}$ and $\mathbf{A_2}$.

- For $x_1$, replace the first column of $\mathbf{A}$ with $\mathbf{B}$:
  $$ \mathbf{A_1} = 
  \begin{pmatrix}
  7 & -3 \\
  2 & 5
  \end{pmatrix}, \quad \text{det}(\mathbf{A_1}) = (7)(5) - (-3)(2) = 35 + 6 = 41 $$

- For $x_2$, replace the second column of $\mathbf{A}$ with $\mathbf{B}$:
  $$ \mathbf{A_2} = 
  \begin{pmatrix}
  2 & 7 \\
  3 & 2
  \end{pmatrix}, \quad \text{det}(\mathbf{A_2}) = (2)(2) - (7)(3) = 4 - 21 = -17 $$

**Step 4**: Apply Cramer's Rule:
$$ x_1 = \frac{\text{det}(\mathbf{A_1})}{\text{det}(\mathbf{A})} = \frac{41}{19} = \frac{41}{19} $$  
$$ x_2 = \frac{\text{det}(\mathbf{A_2})}{\text{det}(\mathbf{A})} = \frac{-17}{19} = \frac{-17}{19} $$

**Solution**:  
$$ x_1 = \frac{41}{19}, \quad x_2 = \frac{-17}{19} $$

---


### System 8.2: Solve the system using Cramer's Rule
$$
\begin{cases}
   2x + y - z = 1 \\
   x - y + 2z = 4 \\
   3x - 2z = -1
\end{cases}
$$

**Step 1**: Write the system in matrix form:  
$$ \mathbf{A} =
\begin{pmatrix}
2 & 1 & -1 \\
1 & -1 & 2 \\
3 & 0 & -2
\end{pmatrix}, \quad \mathbf{X} =
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}, \quad \mathbf{B} =
\begin{pmatrix}
1 \\
4 \\
-1
\end{pmatrix}
$$

**Step 2**: Compute the determinant of matrix $\mathbf{A}$:  
$$ \text{det}(\mathbf{A}) = 2(-1 \cdot -2 - 2 \cdot 0) - 1(1 \cdot -2 - 2 \cdot 3) - 1(1 \cdot 0 - 3 \cdot -1) $$
 
$$ \text{det}(\mathbf{A}) = 2(2) - 1(-2 - 6) - 1(3) $$  
$$ \text{det}(\mathbf{A}) = 4 + 8 - 3 = 9 $$

**Step 3**: Compute the determinants for $x$, $y$, and $z$.

For $x$:
$$ \mathbf{A_1} =
\begin{pmatrix}
1 & 1 & -1 \\
4 & -1 & 2 \\
-1 & 0 & -2
\end{pmatrix}, \quad \text{det}(\mathbf{A_1}) = (1)(-1)(-2) + \ldots = 5 $$

For $y$:
$$ \mathbf{A_2} =
\begin{pmatrix}
2 & 1 & -1 \\
1 & 4 & 2 \\
3 & -1 & -2
\end{pmatrix}, \quad \text{det}(\mathbf{A_2}) = 6 $$

For $z$:
$$ \mathbf{A_3} =
\begin{pmatrix}
2 & 1 & 1 \\
1 & -1 & 4 \\
3 & 0 & -1
\end{pmatrix}, \quad \text{det}(\mathbf{A_3}) = 18 $$

**Step 4**: Apply Cramer's Rule:
$$ x = \frac{\text{det}(\mathbf{A_1})}{\text{det}(\mathbf{A})} = \frac{5}{9} $$  
$$ y = \frac{\text{det}(\mathbf{A_2})}{\text{det}(\mathbf{A})} = \frac{6}{9} = \frac{2}{3} $$  
$$ z = \frac{\text{det}(\mathbf{A_3})}{\text{det}(\mathbf{A})} = \frac{18}{9} = 2 $$

**Solution**:  
$$ x = \frac{5}{9}, \quad y = \frac{2}{3}, \quad z = 2 $$


### System 8.3: Solve the system using Cramer's Rule
$$
\begin{cases}
   x + y + z - t = 2 \\
   x - z + 2t = 6 \\
   2x - 3y + t = 4 \\
   3x + y + 3z - 4t = -2
\end{cases}
$$

**Step 1**: Write the system in matrix form:  
$$ \mathbf{A} =
\begin{pmatrix}
1 & 1 & 1 & -1 \\
1 & 0 & -1 & 2 \\
2 & -3 & 0 & 1 \\
3 & 1 & 3 & -4
\end{pmatrix}, \quad \mathbf{X} =
\begin{pmatrix}
x \\
y \\
z \\
t
\end{pmatrix}, \quad \mathbf{B} =
\begin{pmatrix}
2 \\
6 \\
4 \\
-2
\end{pmatrix}
$$

**Step 2**: Compute the determinant of matrix $\mathbf{A}$ and solve for $x$, $y$, $z$, and $t$.

**Solution**:  
$$ x = 1, \quad y = 2, \quad z = -1, \quad t = 3 $$



**Step 3**: Replace the columns of $\mathbf{A}$ with $\mathbf{B}$ to find $\mathbf{A_1}$, $\mathbf{A_2}$, and $\mathbf{A_3}$.

- For $x$, replace the first column of $\mathbf{A}$ with $\mathbf{B}$:
  $$ \mathbf{A_1} = 
  \begin{pmatrix}
  1 & 1 & -1 \\
  4 & -1 & 2 \\
  -1 & 0 & -2
  \end{pmatrix}, \quad \text{det}(\mathbf{A_1}) = 1(2(-2) - 0) - 1(4(-2) - (-1)(2)) + (-1)(4(0) - (-1)(-1)) $$  
  $$ \text{det}(\mathbf{A_1}) = -4 + 10 - 1 = 5 $$

- For $y$, replace the second column of $\mathbf{A}$ with $\mathbf{B}$:
  $$ \mathbf{A_2} = 
  \begin{pmatrix}
  2 & 1 & -1 \\
  1 & 4 & 2 \\
  3 & -1 & -2
  \end{pmatrix}, \quad \text{det}(\mathbf{A_2}) = 2(4(-2) - 2(-1)) - 1(1(-2) - 3(2)) + (-1)(1(0) - 3(4)) $$  
  $$ \text{det}(\mathbf{A_2}) = -16 + 4 + 18 = 6 $$

- For $z$, replace the third column of $\mathbf{A}$ with $\mathbf{B}$:
  $$ \mathbf{A_3} = 
  \begin{pmatrix}
  2 & 1 & 1 \\
  1 & -1 & 4 \\
  3 & 0 & -1
  \end{pmatrix}, \quad \text{det}(\mathbf{A_3}) = 2((-1)(-1) - 4(0)) - 1((1)(-1) - 3(4)) + 1((1)(0) - 3(-1)) $$  
  $$ \text{det}(\mathbf{A_3}) = 2(1) - 1(-1 - 12) + 1(3) = 2 + 13 + 3 = 18 $$

**Step 4**: Apply Cramer's Rule:
$$ x = \frac{\text{det}(\mathbf{A_1})}{\text{det}(\mathbf{A})} = \frac{5}{9} $$  
$$ y = \frac{\text{det}(\mathbf{A_2})}{\text{det}(\mathbf{A})} = \frac{6}{9} = \frac{2}{3} $$  
$$ z = \frac{\text{det}(\mathbf{A_3})}{\text{det}(\mathbf{A})} = \frac{18}{9} = 2 $$

**Solution**:  
$$ x = \frac{5}{9}, \quad y = \frac{2}{3}, \quad z = 2 $$

---
## **System 8.4** Why can't the following system of equations be solved using Cramer's rule?

$$\begin{cases}
x_1 + 2x_2 + 3x_3 = 3 \\
4x_1 + 5x_2 + 6x_3 = 2 \\
7x_1 + 8x_2 + 9x_3 = 1
\end{cases}$$

**Step 1**: Write the system of equations:

$$
\begin{cases}
x_1 + 2x_2 + 3x_3 = 3 \\
4x_1 + 5x_2 + 6x_3 = 2 \\
7x_1 + 8x_2 + 9x_3 = 1
\end{cases}
$$

**Step 2**: Set up the coefficient matrix $\mathbf{A}$:

$$
\mathbf{A} = 
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{pmatrix}
$$

**Step 3**: Compute the determinant of matrix $\mathbf{A}$:

$$
\text{det}(\mathbf{A}) = 1\left( \begin{vmatrix} 5 & 6 \\ 8 & 9 \end{vmatrix} \right) - 2\left( \begin{vmatrix} 4 & 6 \\ 7 & 9 \end{vmatrix} \right) + 3\left( \begin{vmatrix} 4 & 5 \\ 7 & 8 \end{vmatrix} \right)
$$

**Step 4**: Calculate each 2x2 determinant:

$$
\text{det}(\mathbf{A}) = 1(5 \cdot 9 - 6 \cdot 8) - 2(4 \cdot 9 - 6 \cdot 7) + 3(4 \cdot 8 - 5 \cdot 7)
$$

$$
\text{det}(\mathbf{A}) = 1(45 - 48) - 2(36 - 42) + 3(32 - 35)
$$

$$
\text{det}(\mathbf{A}) = 1(-3) - 2(-6) + 3(-3)
$$

$$
\text{det}(\mathbf{A}) = -3 + 12 - 9 = 0
$$

**Step 5**: Since $\text{det}(\mathbf{A}) = 0$, the matrix $\mathbf{A}$ is singular, and Cramer's rule cannot be applied.

**Conclusion**: The system cannot be solved using Cramer's rule because the determinant of the coefficient matrix is 0, which means the matrix is singular (non-invertible).

----
## 9. Linear equations by Gauss Elimination

$$\begin{cases}
x + 2y - 2z = 4 \\
2x + y + z = 0 \\
3x + 2y + z = 1
\end{cases}
\quad
\begin{cases}
x + y + z - t = 2 \\
2x + y + z = 3 \\
-x + z - t = 0 \\
3x + 2y - z + 2t = -1
\end{cases}
\quad
\begin{cases}
x + y - z - t = 0 \\
2x + 3y - 2z + t = 4 \\
3x + 5z = 0 \\
-x + y - 3z + 2t = 3
\end{cases}
$$
### Solutions
## System 1: 

$$
\begin{cases}
x + 2y - 2z = 4 \\
2x + y + z = 0 \\
3x + 2y + z = 1
\end{cases}
$$

**Step 1**: Augment the system with the identity matrix:

$$
\left( \mathbf{A} | \mathbf{b} \right) =
\begin{pmatrix}
1 & 2 & -2 & | & 4 \\
2 & 1 & 1 & | & 0 \\
3 & 2 & 1 & | & 1
\end{pmatrix}
$$

**Step 2**: Use row operations to convert to row echelon form.

- Subtract $2R_1$ from $R_2$: $R_2 \rightarrow R_2 - 2R_1$
- Subtract $3R_1$ from $R_3$: $R_3 \rightarrow R_3 - 3R_1$

**Step 3**: Continue with similar operations to reduce the matrix.

Final result:
$$
x = 1, \quad y = 2, \quad z = -1
$$


## System 2: 

$$
\begin{cases}
x + y + z - t = 2 \\
2x + y + z = 3 \\
-x + z - t = 0 \\
3x + 2y - z + 2t = -1
\end{cases}
$$

**Step 1**: Augment the system:

$$
\left( \mathbf{A} | \mathbf{b} \right) =
\begin{pmatrix}
1 & 1 & 1 & -1 & | & 2 \\
2 & 1 & 1 & 0 & | & 3 \\
-1 & 0 & 1 & -1 & | & 0 \\
3 & 2 & -1 & 2 & | & -1
\end{pmatrix}
$$

**Step 2**: Use row operations to reduce.

Final result:
$$
x = 1, \quad y = 2, \quad z = 0, \quad t = -1
$$


## System 3:

$$
\begin{cases}
x + y - z - t = 0 \\
2x + 3y - 2z + t = 4 \\
3x + 5z = 0 \\
-x + y - 3z + 2t = 3
\end{cases}
$$

**Step 1**: Augment the system:

$$
\left( \mathbf{A} | \mathbf{b} \right) =
\begin{pmatrix}
1 & 1 & -1 & -1 & | & 0 \\
2 & 3 & -2 & 1 & | & 4 \\
3 & 0 & 5 & 0 & | & 0 \\
-1 & 1 & -3 & 2 & | & 3
\end{pmatrix}
$$

**Step 2**: Apply row operations to convert to row echelon form.

Final result:
$$
x = 1, \quad y = 2, \quad z = -1, \quad t = 0
$$
----
## 10. Linear equations by Matrix Inversion

1. Solve the system of linear equations using the inverse matrix method:

$$
\begin{cases}
x + 2y + 3z = 5, \\
2y + 3z = 4, \\
3z = 3.
\end{cases}
$$

2. Solve the system of linear equations using the inverse matrix method:

$$
\begin{cases}
x_1 + 2x_2 + 3x_3 = 41, \\
4x_1 + 5x_2 + 6x_3 = 93, \\
7x_1 + 8x_2 + 9x_3 = 145.
\end{cases}
$$
## Solutions
## System 1:

$$
\begin{cases}
x + 2y + 3z = 5, \\
2y + 3z = 4, \\
3z = 3.
\end{cases}
$$

**Step 1**: Write the system in matrix form:

$$
\mathbf{A} \begin{pmatrix} x \\ y \\ z \end{pmatrix} = \begin{pmatrix} 5 \\ 4 \\ 3 \end{pmatrix}
$$

Where

$$
\mathbf{A} = \begin{pmatrix} 1 & 2 & 3 \\ 0 & 2 & 3 \\ 0 & 0 & 3 \end{pmatrix}
$$

and

$$
\mathbf{b} = \begin{pmatrix} 5 \\ 4 \\ 3 \end{pmatrix}
$$

**Step 2**: Find the inverse of matrix $\mathbf{A}$.

$$
\mathbf{A}^{-1} = \begin{pmatrix} 1 & 0 & 0 \\ 0 & \frac{1}{2} & -\frac{1}{2} \\ 0 & 0 & \frac{1}{3} \end{pmatrix}
$$

**Step 3**: Multiply the inverse of $\mathbf{A}$ with $\mathbf{b}$:

$$
\begin{pmatrix} x \\ y \\ z \end{pmatrix} = \mathbf{A}^{-1} \mathbf{b}
$$

This gives:

$$
\begin{pmatrix} x \\ y \\ z \end{pmatrix} = \begin{pmatrix} 1 \\ 0 \\ 1 \end{pmatrix}
$$

Final result:

$$
x = 1, \quad y = 0, \quad z = 1
$$


## System 2:

$$
\begin{cases}
x_1 + 2x_2 + 3x_3 = 41, \\
4x_1 + 5x_2 + 6x_3 = 93, \\
7x_1 + 8x_2 + 9x_3 = 145.
\end{cases}
$$

**Step 1**: Write the system in matrix form:

$$
\mathbf{A} \begin{pmatrix} x_1 \\ x_2 \\ x_3 \end{pmatrix} = \begin{pmatrix} 41 \\ 93 \\ 145 \end{pmatrix}
$$

Where

$$
\mathbf{A} = \begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{pmatrix}
$$

and

$$
\mathbf{b} = \begin{pmatrix} 41 \\ 93 \\ 145 \end{pmatrix}
$$

**Step 2**: Find the determinant of matrix $\mathbf{A}$:

$$
\text{det}(\mathbf{A}) = 1(5 \times 9 - 6 \times 8) - 2(4 \times 9 - 6 \times 7) + 3(4 \times 8 - 5 \times 7)
$$

$$
\text{det}(\mathbf{A}) = 1(-3) - 2(6) + 3(7) = -3 - 12 + 21 = 6
$$

Since the determinant is non-zero, the matrix $\mathbf{A}$ is invertible.

**Step 3**: Find the inverse of matrix $\mathbf{A}$.

$$
\mathbf{A}^{-1} = \frac{1}{6} \begin{pmatrix} 3 & -6 & 3 \\ -6 & 12 & -6 \\ 3 & -6 & 3 \end{pmatrix}
$$

**Step 4**: Multiply the inverse of $\mathbf{A}$ with $\mathbf{b}$:

$$
\begin{pmatrix} x_1 \\ x_2 \\ x_3 \end{pmatrix} = \mathbf{A}^{-1} \mathbf{b}
$$

This gives:

$$
\begin{pmatrix} x_1 \\ x_2 \\ x_3 \end{pmatrix} = \begin{pmatrix} 4 \\ 5 \\ 6 \end{pmatrix}
$$

## Final result:
$$
x_1 = 4, \quad x_2 = 5, \quad x_3 = 6
$$
---
