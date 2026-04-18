Batman LED Chaser 🦇
A custom-designed, Batman-shaped PCB that sequences 10 LEDs in a "Knight Rider" style light chase.

Project Description
This project was a deep dive into custom hardware design. Using an NE555 Timer as a clock and a CD4017 Decade Counter as the sequencer, I designed a schematic to handle the logic and then a custom PCB layout shaped like the Batman logo to house the physical components.

Steps to Reproduce
Schematic Design: Mapped out the electrical logic in EasyEDA, wiring the timer, counter, LEDs, and passive components.

PCB Layout: Imported a Batman logo silhouette as a reference stencil, traced the BoardOutline to create the custom shape, and arranged the components.

Routing: Used the Auto-Router to calculate and place the physical copper traces between components.

Manufacturing: Exported the Gerber files and ordered the boards through JLCPCB.

Bill of Materials (LCSC Part Codes)
CD4017BCN: CD4017BCN (Main Counter IC)

C46749: 555 Timer IC

C492401: Power Header

C81276: Debug Header

C62934: Electrolytic Capacitor

C249157: Ceramic Capacitor

C713997: 1k ohm Resistor

C58592: 470 ohm Resistor

C118912: Potentiometer (Speed Control)

C2895480: Normal LED (Quantity: 10)

Project Media
Schematic: <img width="727" height="505" alt="soft" src="https://github.com/user-attachments/assets/887b5271-18eb-4724-bf07-2edf5f8ae818" />


PCB Layout: <img width="847" height="592" alt="hard" src="https://github.com/user-attachments/assets/3aeb9c32-a956-45d8-9448-59033123becd" />
