# Spiral Matrix Traversal in Java 🌀

A robust implementation of clockwise spiral order traversal for an $N \times M$ 2D matrix in Java.

---

## 📌 Problem Overview
Given a matrix of $N$ rows and $M$ columns, print all elements of the matrix in clockwise spiral order, starting from the top-left cell $(0, 0)$ and spiraling inwards toward the center.

---

## 💡 Algorithm & Approach

The solution utilizes **four boundary pointers** to traverse layer by layer:
1. `rowStart` (initialized to `0`)
2. `rowEnd` (initialized to `N - 1`)
3. `colStart` (initialized to `0`)
4. `colEnd` (initialized to `M - 1`)

### Traversal Steps:
- **Left to Right:** Traverse from `colStart` to `colEnd` along `rowStart`, then increment `rowStart`.
- **Top to Bottom:** Traverse from `rowStart` to `rowEnd` along `colEnd`, then decrement `colEnd`.
- **Right to Left:** Check boundary condition (`rowStart <= rowEnd`), traverse from `colEnd` down to `colStart` along `rowEnd`, then decrement `rowEnd`.
- **Bottom to Top:** Check boundary condition (`colStart <= colEnd`), traverse from `rowEnd` down to `rowStart` along `colStart`, then increment `colStart`.

---

## ⚙️ Edge-Case Handling & Debugging

- **Negative Index Prevention:** Added explicit boundary safety guards (`if (rowStart <= rowEnd)` and `if (colStart <= colEnd)`) to eliminate `ArrayIndexOutOfBoundsException: Index -1`.
- **Non-Square Matrices:** Seamlessly handles rectangular grids ($N \neq M$) without duplicate element visits.

---

## 🚀 How to Run

```bash
javac SpiralOrder.java
java SpiralOrder
