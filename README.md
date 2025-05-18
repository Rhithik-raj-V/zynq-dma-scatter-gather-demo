#  Xilinx Scatter-Gather DMA Walkthrough

🔧 **In-depth walkthrough of Scatter-Gather (SG) mode AXI DMA on Xilinx Zynq, featuring annotated C code and register-level configuration.**

This repository showcases my understanding of SG DMA operation in a Xilinx Zynq system. I reverse-engineered and documented the setup, configuration, and internal workings of the DMA engine based on a bare-metal C implementation and Vivado block design.

---

##  Documentation

- **File:** `DOCUMENTATION OF DMA IN SCATTER GATHER MODE PART 2.pdf`  
- **What it covers:**
  - Zynq block design overview with AXI DMA in SG mode
  - Memory map and buffer descriptor layout
  - Step-by-step analysis of each DMA-related function
  - Explanation of register operations (CR, SR, CDESC, TDESC, etc.)
  - TX and RX BD ring creation, initialization, and usage
  - Practical use of API functions:  
    `XAxiDma_CfgInitialize`, `XAxiDma_BdRingCreate`, `XAxiDma_BdRingStart`, `XAxiDma_BdRingClone`, etc.

This is a hands-on technical guide—not a copy of Xilinx documentation—intended to help FPGA engineers understand the logic behind DMA SG mode at both API and hardware levels.

---

##  Technologies Used

- **Platform:** Xilinx Zynq (tested with ZedBoard)
- **Tools:** Vivado, Vitis/SDK
- **Language:** C (bare-metal)
- **Interfaces:** AXI DMA, AXI-Stream FIFO

---

##  Use Case

This repo is especially helpful for:
- FPGA engineers learning DMA architecture
- Embedded developers debugging AXI DMA in SG mode
- Anyone needing a guided teardown of Xilinx's DMA driver structure

---

##  Motivation

I built this documentation to deepen my understanding of low-level data transfer mechanisms in FPGA systems. Rather than just using pre-made IPs, this was my effort to analyze how the code actually works under the hood—every function, structure, and register bit.

This is part of my learning portfolio, as referenced in my resume.

---

 **If you found this insightful, feel free to star the repo or share it with others working on similar systems!**
