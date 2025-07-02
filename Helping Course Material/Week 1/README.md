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

IPC = Instruction Count / Total CPU Cycles = 1 / CPI


> Higher IPC means better instruction throughput per cycle.

---

### ✅ 5. Clock Rate & Cycle Time

**Definition**:  
- **Clock Rate**: Number of cycles per second (Hz).
- **Cycle Time**: Duration of a single clock cycle.

**Formulas**:  

Clock Rate = 1 / Cycle Time
Cycle Time = 1 / Clock Rate


> Faster clock rate = more operations per second, but architecture efficiency also matters.

---

### ✅ 6. Amdahl’s Law

**Definition**:  
Determines the maximum speedup possible from improving part of a system.

**Formula**:  

Speedup = 1 / [(1 - f) + (f / s)]


- `f` = fraction of the task affected by the improvement  
- `s` = speedup of the improved portion

**Example**:  
If 60% of a task is sped up 3×:

Speedup = 1 / (0.4 + 0.6/3) = 1 / 0.6 ≈ 1.67× overall speedup


> Highlights diminishing returns on optimization.

---

### ✅ 7. Benchmarks

**Definition**:  
Standardized tests to evaluate and compare system performance.

**Examples**:

| Benchmark    | Focus                        |
|--------------|------------------------------|
| SPEC CPU     | CPU and memory performance   |
| Geekbench    | General CPU/GPU workloads    |
| Linpack      | Floating-point performance   |
| PCMark       | Desktop application tasks    |

> Always choose benchmarks that resemble your actual workload.

---

## 📈 Summary Table

| Metric         | Formula                                      | Meaning                                |
|----------------|-----------------------------------------------|----------------------------------------|
| Execution Time | (Instructions × CPI) / Clock Rate             | Total runtime                          |
| CPI            | CPU Cycles / Instruction Count                | Efficiency of instruction execution    |
| IPC            | Instruction Count / CPU Cycles = 1 / CPI      | Instructions per clock cycle           |
| MIPS           | Instruction Count / (Execution Time × 10⁶)    | Rate of execution in millions/sec      |
| Cycle Time     | 1 / Clock Rate                                | Time taken for one cycle               |
| Amdahl’s Law   | 1 / [(1 - f) + f/s]                           | Projected speedup from optimization    |

---

## 🎯 Key Takeaways

- **Execution time** reflects user experience.
- **CPI/IPC** reveal how well the CPU utilizes cycles.
- **MIPS** gives basic throughput—but with limitations.
- **Amdahl’s Law** helps assess how much optimization is worth.
- **Benchmarks** provide real-world performance data.

---

## 📂 Additional Resources

- [Exercises](./exercises.md)  
- [Solutions](./solutions/)  
- [Tools Demo](./tools-demo/) – Examples using `perf`, `CPU-Z`, etc.

---

✅ **Next Topic Preview**:  
→ [Instruction-Level Parallelism (ILP)](../topic-02-ilp/README.md)

Ready to practice? Jump to [`exercises.md`](./exercises.md).
