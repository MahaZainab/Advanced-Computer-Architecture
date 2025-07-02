# 📊 Topic 01: Performance Metrics & Fundamentals

This topic introduces and explains the essential metrics used to evaluate and optimize processor and system performance.

---

## 📘 Key Concepts in Detail

### ✅ 1. Execution Time (Response Time)

**Definition**:  
The total time a program takes to run from start to finish.

**Formula**:  

Execution Time = (Instruction Count × CPI) / Clock Rate


- **Instruction Count**: Number of instructions executed.
- **CPI**: Cycles per instruction.
- **Clock Rate**: Processor speed (e.g., 2 GHz = 2 × 10⁹ Hz).

> Lower execution time indicates better performance.

---

### ✅ 2. CPI – Cycles Per Instruction

**Definition**:  
Average number of clock cycles required to execute one instruction.

**Formula**:  

CPI = Total Clock Cycles / Instruction Count


> A lower CPI generally reflects a more efficient processor architecture.

---

### ✅ 3. MIPS – Million Instructions Per Second

**Definition**:  
Measures the number of instructions executed per second (in millions).

**Formula**:  

MIPS = Instruction Count / (Execution Time × 10^6)


> ⚠️ MIPS can be misleading across different architectures or programs with varying instruction complexity.

---

### ✅ 4. IPC – Instructions Per Cycle

**Definition**:  
Average number of instructions executed per CPU cycle.

**Formula**:  

