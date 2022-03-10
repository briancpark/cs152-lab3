# Lab 3 Logs


## Simualtion commands to run
```sh
cd ${LAB3ROOT}/sims/verilator
make CONFIG=CS152BaselineBoomConfig
make CONFIG=CS152BaselineBoomConfig run-bmark-tests
cd output/chipyard.TestHarness.CS152BaselineBoomConfig
```


One-liner
```sh
cd ${LAB3ROOT}/sims/verilator && make CONFIG=CS152BaselineBoomConfig -j && make CONFIG=CS152BaselineBoomConfig run-bmark-tests -j
```


```
mcycle = 16638
minstret = 2417
mcycle = 37908
minstret = 6170

matmul(cid, nc, 16, input1_data, input2_data, results_data); barrier(nc): 219501 cycles, 53.5 cycles/iter, 8.3 CPI

vvadd(cid, nc, 1000, input1_data, input2_data, results_data); barrier(nc): 53959 cycles, 53.9 cycles/iter, 5.3 CPI

vvadd(cid, nc, 1000, results_data, input2_data, results_data); barrier(nc): 51043 cycles, 51.0 cycles/iter, 5.0 CPI
C0: reg block 4x5x6, cache block 24x25x24
C0: 24688 instructions
C0: 60579 cycles
C0: 28800 flops
C0: 475 Mflops @ 1 GHz
mcycle = 209125
minstret = 34851
Microseconds for one run through Dhrystone: 2618
Dhrystones per Second:                      381
mcycle = 1309273
minstret = 196029
mcycle = 725758
minstret = 127368

  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/median.riscv.out  Completed after 135642 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/multiply.riscv.out        Completed after 408878 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/qsort.riscv.out  Completed after 1682042 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/towers.riscv.out  Completed after 126190 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/vvadd.riscv.out  Completed after 123480 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/dhrystone.riscv.out       Completed after 1515030 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/mt-matmul.riscv.out       Completed after 339767 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/mm.riscv.out     Completed after 917451 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/spmv.riscv.out   Completed after 859110 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/mt-vvadd.riscv.out        Completed after 604033 cycles
```


```
mcycle = 16638
minstret = 2417
mcycle = 23018
minstret = 4156
mcycle = 37908
minstret = 6170

matmul(cid, nc, 16, input1_data, input2_data, results_data); barrier(nc): 219501 cycles, 53.5 cycles/iter, 8.3 CPI
mcycle = 175341
minstret = 24101

vvadd(cid, nc, 1000, input1_data, input2_data, results_data); barrier(nc): 53959 cycles, 53.9 cycles/iter, 5.3 CPI

vvadd(cid, nc, 1000, results_data, input2_data, results_data); barrier(nc): 51043 cycles, 51.0 cycles/iter, 5.0 CPI
C0: reg block 4x5x6, cache block 24x25x24
C0: 24688 instructions
C0: 60579 cycles
C0: 28800 flops
C0: 475 Mflops @ 1 GHz
mcycle = 209125
minstret = 34851
Microseconds for one run through Dhrystone: 2618
Dhrystones per Second:                      381
mcycle = 1309273
minstret = 196029
mcycle = 725758
minstret = 127368

  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/median.riscv.out  Completed after 135642 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/multiply.riscv.out        Completed after 408878 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/qsort.riscv.out  Completed after 1682042 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/towers.riscv.out  Completed after 126190 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/vvadd.riscv.out  Completed after 123480 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/dhrystone.riscv.out       Completed after 1515030 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/mt-matmul.riscv.out       Completed after 339767 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/mm.riscv.out     Completed after 917451 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/spmv.riscv.out   Completed after 859110 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/mt-vvadd.riscv.out        Completed after 604033 cycles
```


mcycle = 16638
minstret = 2417
mcycle = 37908
minstret = 6170
mcycle = 23018
minstret = 4156

matmul(cid, nc, 16, input1_data, input2_data, results_data); barrier(nc): 219501 cycles, 53.5 cycles/iter, 8.3 CPI

mcycle = 175341
minstret = 24101
vvadd(cid, nc, 1000, input1_data, input2_data, results_data); barrier(nc): 53959 cycles, 53.9 cycles/iter, 5.3 CPI

vvadd(cid, nc, 1000, results_data, input2_data, results_data); barrier(nc): 51043 cycles, 51.0 cycles/iter, 5.0 CPI
C0: reg block 4x5x6, cache block 24x25x24
C0: 24688 instructions
C0: 60579 cycles
C0: 28800 flops
C0: 475 Mflops @ 1 GHz
mcycle = 209125
minstret = 34851
Microseconds for one run through Dhrystone: 2618
Dhrystones per Second:                      381
mcycle = 1309273
minstret = 196029
mcycle = 725758
minstret = 127368

  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/median.riscv.out  Completed after 135642 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/multiply.riscv.out        Completed after 408878 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/qsort.riscv.out  Completed after 1682042 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/towers.riscv.out  Completed after 126190 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/vvadd.riscv.out  Completed after 123480 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/dhrystone.riscv.out       Completed after 1515030 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/mt-matmul.riscv.out       Completed after 339767 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/mm.riscv.out     Completed after 917451 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/spmv.riscv.out   Completed after 859110 cycles
  [ PASSED ] /scratch/cs152-aaf/lab3/sims/verilator/output/chipyard.TestHarness.CS152BaselineBoomConfig/mt-vvadd.riscv.out        Completed after 604033 cycles