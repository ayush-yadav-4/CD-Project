
# Three Address Code Generator for 3D Array
## Deployment Link (Teat at) = https://ayush-yadav-4.github.io/CD-Project/
## 📌 Introduction
This project is a **Three Address Code (TAC) Generator** for accessing elements in a **3D array** using **Row-Major Order**.  
It takes user input (array indices, dimensions, element size, and base address) and generates the corresponding **TAC representation**.

## 📌 How It Works?
In **Row-Major Order**, the memory address of an element `A[i][j][k]` in a **3D array** is calculated using:

\[
Address = Base + ((i \times d_2 \times d_3) + (j \times d_3) + k) \times ElementSize
\]

Where:
- `i` is the first index (depth)
- `j` is the second index (row)
- `k` is the third index (column)
- `d2` is the number of rows in the 3D array
- `d3` is the number of columns in the 3D array
- `Base` is the starting memory address
- `ElementSize` is the size of a single element

The program follows these steps:
1. Takes user input for array properties.
2. Computes intermediate TAC statements.
3. Displays the generated **Three Address Code**.

---

## 📌 Input Guide
Here’s what each input represents and an example:

| **Input Field**  | **Description** | **Example Value** |
|-----------------|----------------|----------------|
| **Array Name** | Name of the 3D array | `A` |
| **i index** | First index (depth) | `2` |
| **j index** | Second index (row) | `1` |
| **k index** | Third index (column) | `3` |
| **Base Address** | Starting memory address (default: 1000) | `1000` |
| **Row Size (d₂)** | Number of rows in the 3D array | `4` |
| **Column Size (d₃)** | Number of columns per row | `5` |
| **Element Size** | Size of one element in bytes (default: 4) | `4` |

### Example Input:
