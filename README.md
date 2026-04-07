# test1
forclass
# 📘 Adaptive Filter Algorithm (NLMS)

---

## 🔧 Initialization
> $\hat{h}(0) = \text{zeros}(p)$

---

## ⚙️ Computation
For $n = 0, 1, 2, \dots$

---

### 📐 Input Vector Definition
$$
\mathbf{x}(n) =
\begin{bmatrix}
x(n), x(n-1), \dots, x(n-p+1)
\end{bmatrix}^{T}
$$

---

### 📉 Error Signal
$$
e(n) = d(n) - \hat{h}^{H}(n)\mathbf{x}(n)
$$

---

### 🔄 Coefficient Update Rule
$$
\hat{h}(n+1) =
\hat{h}(n) +
\frac{\mu \, e^{*}(n)\mathbf{x}(n)}
{\mathbf{x}^{H}(n)\mathbf{x}(n)}
$$

---

## 🧠 Summary
- **Initialization**: Start with zero vector  
- **Input Vector**: Past $p$ samples  
- **Error Calculation**: Desired minus estimated output  
- **Update Rule**: Normalized LMS adjustment  

---

## 🧩 Notes
- $H$ 表示 **Hermitian transpose（共軛轉置）**
- $*$ 表示 **複數共軛**
- $\mu$ 為 **學習率 (step size)**
- 分母 $\mathbf{x}^{H}(n)\mathbf{x}(n)$ 用於 **正規化 (Normalization)**

---

## 📌 Structure Overview
| Step | Formula |
|------|--------|
| Init | $\hat{h}(0) = \text{zeros}(p)$ |
| Input | $\mathbf{x}(n)$ |
| Error | $e(n)$ |
| Update | $\hat{h}(n+1)$ |

---

## 🧮 Algorithm Type
**Normalized Least Mean Squares (NLMS)**

---

## 📎 Reference Layout (Same as Image)
- Initialization 在最上方  
- Computation 接續說明  
- 三個主要公式垂直排列  
- 數學符號完全一致  

---
