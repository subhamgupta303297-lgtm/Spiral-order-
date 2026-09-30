# Java & Data Structures Practice 🚀

A structured collection of Core Java implementations, algorithm practice problems, and Data Structures solutions developed during my engineering journey.

---

## 📂 Repository Structure

- `01-Basics/` - Control statements, loops, methods, Scanner input handling.
- `02-Arrays-1D/` - Min/Max search, array reversals, linear search, sub-arrays.
- `03-Arrays-2D/` - Matrix traversal, Matrix Transpose, Spiral Order Matrix.
- `04-OOP-Concepts/` - Classes, Objects, Inheritance, and Encapsulation.

---

## 🧩 Key Problems Solved

1. **Spiral Matrix Traversal (`SpiralOrder.java`):**
   - Traversing $N \times M$ 2D matrices in boundary layers using four boundary pointers (`rowStart`, `rowEnd`, `colStart`, `colEnd`).
2. **Matrix Transpose (`MatrixTranspose.java`):**
   - Converting rows into columns with index inversion $T[j][i] = M[i][j]$.
3. **Array Extremes (`FindMinMax.java`):**
   - Tracking minimum and maximum values cleanly using `Integer.MIN_VALUE` and `Integer.MAX_VALUE`.

---

## ⚙️ How to Compile and Run

Clone the repository and compile using standard JDK commands:

```bash
# Clone the repository
git clone [https://github.com/your-username/Java-DSA-Solutions.git](https://github.com/your-username/Java-DSA-Solutions.git)

# Navigate to folder
cd Java-DSA-Solutions

# Compile and run any program
javac SpiralOrder.java
java SpiralOrder
