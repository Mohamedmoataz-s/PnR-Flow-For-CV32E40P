Below is the **paragraph-style README** with **image descriptions placed immediately after each image**. You can paste directly into `README.md`:

---

This project implements a complete RTL-to-GDSII physical design flow for the open-source cv32e40p RISC-V processor core using professional Synopsys EDA tools. The goal is to transform Verilog RTL into a manufacturable GDSII layout following industry-standard VLSI backend methodologies.

Starting from RTL, the design is synthesized using Design Compiler to generate a gate-level netlist optimized for area, power, and timing. Static timing constraints (SDC) are applied to ensure proper frequency targets and design integrity before entering the physical design environment.

The physical design flow is realized in IC Compiler II (ICC2), beginning with floorplanning to define the core boundaries, routing channels, and I/O ring. A robust Power Delivery Network (PDN) is implemented using core rings and metal straps to guarantee stable power distribution across the chip.

Next, standard cells are placed using global and detailed placement, achieving balanced cell distribution and routability without congestion hotspots. Clock Tree Synthesis (CTS) is performed to create a low-skew clock network with balanced insertion delay. Following CTS, detailed routing connects all signals while resolving DRC violations and optimizing wire geometry.

Post-route optimization, extraction, and PrimeTime STA ensure setup and hold timing closure. Parasitic files (SPEF/SDF) are generated for accurate timing and signal integrity analysis. The flow concludes with the generation of final GDSII, DEF, and sign-off reports, representing a complete tape-out-ready ASIC layout.

This project demonstrates hands-on experience with key digital backend processes including timing closure, congestion debugging, routing optimization, and sign-off methodologies, offering valuable real-world VLSI implementation knowledge.
---

### 📸 Flow Outputs

#### 🧠 Design Browser

![hierarchy browser ](https://github.com/user-attachments/assets/050f97a8-a95e-4b07-8e35-0bcc9473461a)
*Shows RTL module hierarchy loaded into the design environment, confirming structural correctness.*

#### 🗂️ Design Hierarchy View

![design hierarchy ](https://github.com/user-attachments/assets/95964bc1-9545-486b-801a-ace43ac05d87)
*Displays top-level core structure and submodules used during synthesis and floorplan setup.*

#### 🧱 Floorplan

![floorplan](https://github.com/user-attachments/assets/c84fb8e5-50ca-406c-a33b-5bbd9b7217e2)
*Demonstrates core area boundaries, IO ring, placement rows, and routing channels.*

#### ⚡ Power Distribution Network

![powerplan](https://github.com/user-attachments/assets/d91393a1-e858-4acc-8323-ca89c64553fa)
*Illustrates power rings, metal straps, and a robust power grid across the core region.*

#### 📐 Placement Cell Density

![placment cell denisty](https://github.com/user-attachments/assets/1f8fe5db-cf87-47d4-890c-43327320fce4)
*Shows standard cell distribution across the chip with balanced placement and minimal congestion.*

#### 📌 Pin Density Map

![placment pin denisty](https://github.com/user-attachments/assets/d336db34-af69-4e7c-a1fd-1cf5617f9c6c)
*Indicates pin distribution and high-activity regions for routing optimization.*

#### 🕒 Clock Tree Synthesis (CTS)

![design CTS](https://github.com/user-attachments/assets/9d0ab2d2-bfde-4c33-b1f4-369405e75b0d)
*Shows CTS buffers and clock routes ensuring balanced clock skew and delay.*

#### 🛠 Routing & Chip Finishing

![Route and Chipfinishing](https://github.com/user-attachments/assets/e74b0db5-a108-4fd3-b37c-6a8db5b4b981)
*Displays full routing, ECO fixes, DRC cleanup, and ready-for-GDS layout state.*

