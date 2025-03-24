### **1. Given Data:**  
- **Concrete Strength**: \( f'_{ck} = 21 \) MPa  
- **Steel Strength**: \( f_y = 300 \) MPa  
- **Reinforcement Area**: \( A_s = 1523 \) mm²  
- **Beam Dimensions**:  
  - **Height**: \( h = 600 \) mm  
  - **Width**: \( b = 300 \) mm  
  - **Effective Depth**: \( d = 500 \) mm  
- **Loads:**  
  - **Self-weight (Dead Load, \( D \))**:  
    - **Concrete Density**: \( \gamma_c = 25 \) kN/m³  
  - **Live Load**: \( L = 40 \) kN/m  
- **Factored Load:**  
  - Given by:  
    \[
    U = 1.4D + 1.7L
    \]

---

### **2. Load Calculation**  
#### **Dead Load (Self-weight of the beam)**  
\[
D = \gamma_c \times b \times h
\]
\[
D = 25 \times (0.3 \times 0.6) = 25 \times 0.18 = 4.5 \text{ kN/m}
\]

#### **Factored Load**  
\[
U = 1.4(4.5) + 1.7(40)
\]
\[
U = 6.3 + 68 = 74.3 \text{ kN/m}
\]

---

### **3. Maximum Moment Calculation**  
For a **simply supported beam** with a **uniformly distributed load**, the maximum **bending moment** is given by:  
\[
M_u = \frac{U L^2}{8}
\]
\[
M_u = \frac{(74.3) (4.0)^2}{8}
\]
\[
M_u = \frac{74.3 \times 16}{8} = \frac{1188.8}{8} = 148.6 \text{ kN}\cdot\text{m}
\]
\[
M_u = 148.6 \times 10^6 \text{ N}\cdot\text{mm}
\]

---

### **4. Check Steel Strength**  
The **ultimate moment capacity** of a singly reinforced beam is given by:  
\[
M_u = 0.87 f_y A_s (d - a/2)
\]
where **"a"** is the depth of the **equivalent stress block**, calculated as:  
\[
a = \frac{A_s f_y}{0.85 f'_{ck} b}
\]
\[
a = \frac{(1523 \times 300)}{0.85 \times 21 \times 300}
\]
\[
a = \frac{456900}{5355} = 85.3 \text{ mm}
\]

Now, substitute \( a \) into the moment equation:  
\[
M_u = 0.87 \times 300 \times 1523 \times (500 - 85.3/2)
\]

It looks like I encountered an issue running the calculation. Let me quickly compute it again for you.  

\[
a = \frac{1523 \times 300}{0.85 \times 21 \times 300} = \frac{456900}{5355} = 85.3 \text{ mm}
\]

Now,  
\[
M_u = 0.87 \times 300 \times 1523 \times (500 - 85.3/2)
\]
\[
M_u = 0.87 \times 300 \times 1523 \times (500 - 42.65)
\]
\[
M_u = 0.87 \times 300 \times 1523 \times 457.35
\]
\[
M_u = 181.75 \times 10^6 \text{ N·mm} = 181.75 \text{ kN·m}
\]

### **Final Check**  
- **Required Ultimate Moment**: **148.6 kN·m**  
- **Calculated Moment Capacity**: **181.75 kN·m**  

Since **181.75 kN·m** **≥** **148.6 kN·m**, the **beam is SAFE** ✅.
