# **Three Address Code (TAC) Generation for 3D Array using SDTS**  

## **📌 Project Overview**  
This project implements **Three Address Code (TAC) generation** for assignments involving **3D arrays**, using **Syntax Directed Translation Scheme (SDTS)**. It follows **Row-Major Order** to compute memory addresses and generates TAC accordingly.  

### **🔹 Key Features**  
- Tokenizes the input code using a **Lexer**.  
- Parses array indices and **computes addresses dynamically**.  
- Generates **optimized Three Address Code (TAC)** for array assignments.  
- Ensures correct syntax handling with proper error checking.  
- Fully executable in **Google Colab or any Python environment**.  

---

## **🚀 Steps to Execute**  

### **1️⃣ Run the Code in Google Colab**
Copy-paste the code into a **Google Colab** notebook and execute it.  

### **2️⃣ Input Code Example**
```python
code = "A[i][j][k] = B;"
```
- This assigns **B** to the **3D array A[i][j][k]**.  

### **3️⃣ Output (Generated TAC)**
```
Three Address Code (TAC) Generated:

t1 = i * 100
t2 = j * 10
t3 = t1 + t2
t4 = t3 + k
t5 = t4 * 4
t6 = &A + t5
MEM[t6] = B
```
- This shows the **computed memory address** and the final assignment.

---

## **🛠️ How This Works?**
1. **Lexical Analysis (Lexer)**  
   - Breaks the input into **tokens** (variables, operators, brackets, etc.).  
2. **Parsing & Address Calculation**  
   - Computes the **Row-Major Address** for `A[i][j][k]`.  
3. **Three Address Code (TAC) Generation**  
   - Converts expressions into **low-level intermediate code**.  
4. **Displays TAC Output**  
   - Shows step-by-step execution of memory address calculations.  

---

## **📌 Example Use Cases**  
✅ **Compiler Design Projects** 🎓  
✅ **Understanding TAC for Multi-Dimensional Arrays**  
✅ **Building a Mini Compiler with 3D Array Support**  

---

## **📩 Future Enhancements**  
- ✅ Extend support for **expressions on RHS** (e.g., `A[i][j][k] = B + C;`).  
- ✅ Optimize **register allocation** for better performance.  
- ✅ Implement a **GUI-based compiler simulator**.  

---

## **🤝 Contribution**  
Feel free to **modify and extend** this project! 🎉 If you have any suggestions or improvements, let me know! 🚀  
