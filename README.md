Batman LED Chaser - Custom Hardware Build

Project Description
For this project, I stepped away from my usual full-stack software development to build a custom piece of physical hardware. This is a classic "Knight Rider" style LED chaser circuit, but instead of using a standard rectangular circuit board, I designed a custom PCB shaped exactly like the Batman logo. The brains of the board use an NE555 timer chip to create a steady electrical heartbeat, and a CD4017 decade counter to distribute that pulse across 10 LEDs spread out along the bat wings.

Steps Taken to Build It

Designing the Logic: I started in EasyEDA by laying out the schematic. I wired the NE555 timer, the CD4017 counter, and all the passive components together to make sure the backend logic was sound before worrying about the physical layout.

The Custom Outline: For the physical board layout, I imported a solid black Batman logo silhouette to use as a background stencil. I then used the board outline tool to manually trace the shape, creating a custom cut-path for the factory.

Component Placement: I arranged the two main IC chips in the center of the bat, and distributed the 10 LEDs symmetrically across the left and right wings.

Copper Routing: Once the components were placed inside the custom shape, I ran the auto-router to generate the physical top and bottom copper traces, connecting everything together without shorting out.

Manufacturing: I finalized the design files and sent them directly to JLCPCB for physical fabrication.

Process Pictures
<img width="844" height="593" alt="Screen Shot 2026-04-18 at 16 44 00" src="https://github.com/user-attachments/assets/dd2665b0-0358-43bb-9ea0-890422db921a" />


Bill of Materials (Parts List)

1x NE555P Timer IC

1x CD4017BCN Decade Counter IC

10x Standard Through-Hole LEDs

1x 1k Ohm Resistor

1x 470 Ohm Resistor

1x 50k Ohm Potentiometer (to dial in the speed of the LEDs)

1x 1uF Electrolytic Capacitor

1x 10nF Ceramic Capacitor

Standard Male Header Pins (for Power, Ground, and a Clock debug pin)

1x Custom Batman Printed Circuit Board
