## Objective
This project showcases a series of CMOS digital circuit designs implemented as part of the Low Power Digital Integrated Circuits (ELE734) course. The work focuses on the full CMOS design flow, including schematic design, verification through simulation, physical layout creation, and post-layout analysis using Cadence. Through these labs I implemented digital building blocks such as **NAND, NOR, and a 1-bit full adder**, while exploring how transistor sizing, parasitic effects, and layout design influence timing performance and power characteristics.

---

## Lab 1 — NMOS & PMOS Transistor Layouts

The first step of the project involved designing the fundamental building blocks of CMOS logic: the NMOS and PMOS transistors. Using Cadence Virtuoso, transistor layouts were created following CMOS design rules to ensure correct diffusion regions, gate placement, and well structures. This exercise introduced the physical design constraints that influence real silicon implementation.

<img width="432" height="390" alt="Image" src="https://github.com/user-attachments/assets/f26ae7c3-a009-41e2-a29a-19f7c7a8d71b" /> 
<img width="508" height="364" alt="Image" src="https://github.com/user-attachments/assets/63fca308-deed-492a-b82f-38da5a241ada" /><br>

**Figure 1: NMOS & PMOS Transistor Layout**

---

## Lab 2 — CMOS Inverter

With the individual transistors validated, the next step was designing a CMOS inverter. The schematic connects the PMOS and NMOS transistors in a complementary configuration to create the simplest CMOS logic gate. A testbench was then used to simulate the inverter and verify correct switching behaviour.

<img width="288" height="159" alt="Image" src="https://github.com/user-attachments/assets/9bc6df0a-981a-4c8e-ab9e-6a4c7a1f1140" />
<img width="350" height="164" alt="Image" src="https://github.com/user-attachments/assets/78f82b20-dcea-42b5-87c2-6a969ca13b3c" /><br>

**Figure 2: CMOS Inverter Schematic & Testbench**  

The inverter was then translated into a physical layout while maintaining proper transistor placement and routing. Layout verification ensured the design followed fabrication design rules and preserved the schematic connectivity.

<img width="373" height="388" alt="Image" src="https://github.com/user-attachments/assets/00b72a4d-7930-42f8-b246-fda3746b10ed" /> <br>
**Figure 3: CMOS Inverter Layout**

---

## Lab 3 — NAND & NOR Gates

After validating the inverter, more complex combinational logic gates were implemented. This lab focused on designing CMOS NAND and NOR gates by arranging PMOS and NMOS transistors in series and parallel configurations. The schematics below represent the logical implementations of these gates.

<img width="467" height="360" alt="Image" src="https://github.com/user-attachments/assets/1f8eea8b-13d0-4142-b1f6-0fbe529c31eb" /> 
<img width="488" height="375" alt="Image" src="https://github.com/user-attachments/assets/a68e6444-6e0d-496c-86f4-0e1bf014b636" /> <br>

**Figure 4: CMOS NAND & NOR Gate Schematic**  

*Note: the NAND schematic technically looks like an AND gate because I forgot to include the small inversion bubble at the output — a classic schematic oversight — but the transistor configuration correctly implements a NAND.*

The layouts below show the physical implementations of the NAND and NOR gates, demonstrating how series and parallel transistor networks translate into silicon layout structures.

<img width="222" height="539" alt="Image" src="https://github.com/user-attachments/assets/80da90f6-ed19-4c77-937d-1b994393065d" />
<img width="245" height="624" alt="Image" src="https://github.com/user-attachments/assets/583243c5-35d9-4f09-bb56-8012f7f08b6f" /> <br>
**Figure 5: CMOS NAND & NOR Gate Layout**  

---

## Lab 4 — 1-Bit Full Adder

The final lab integrated multiple CMOS logic gates to implement a 1-bit full adder. This circuit performs binary addition using three inputs (A, B, and Carry-In) and produces Sum and Carry-Out outputs. Designing the full adder required combining previously developed logic gates while ensuring proper transistor connectivity and layout verification.

<img width="593" height="326" alt="Image" src="https://github.com/user-attachments/assets/d22025dd-a5be-4940-a0a7-e4af55a3ceec" /> <br>
**Figure 6: 1-Bit Full Adder Schematic**

The schematic was then translated into a physical layout, ensuring the design satisfied CMOS design rules while maintaining connectivity and functional correctness.

<img width="620" height="421" alt="Image" src="https://github.com/user-attachments/assets/17243014-6617-4669-8443-b42375d5d6dd" /> <br>
**Figure 7: 1-Bit Full Adder Layout**
