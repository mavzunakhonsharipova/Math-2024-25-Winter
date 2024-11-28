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
