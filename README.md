# batman-blink-board
# Batman LED Chaser 🦇 (My First Custom PCB)

Yoo so this is my first ever custom hardware project. Im usually a software guy (MERN stack, mostly React stuff like when I built NextWatch) so jumpin into raw hardware was wild. But I finally figured it out. 

Basically this is a "Knight Rider" style LED chaser, but instead of a boring square board, the LEDs run across a custom Batman shaped PCB. 

## How it works (The Brains)
I learned that hardware is basically just full stack dev but with electricity. 
* **The NE555P Timer:** This is the heartbeat. It just pulses power on and off based on the resistors and capacitors attached to it. Its like the setInterval function in JS.
* **The CD4017 Decade Counter:** This chip listens to the 555 timer's heartbeat. Everytime it hears a beat, it shifts power to the next LED in the sequence (0 through 9). 

## The Tools I used
Everything was designed in **EasyEDA** (standard version, runnin right in the browser). 

**Phase 1: The Schematic (The Backend)**
First I had to draw the schematic. This is purely theoretical—like mapping out API routes or database schemas. Just putting down the symbols for the 555, the 4017, the 10 LEDs, and wiring them together so the logic works. Tbh wiring the manual traces in the schematic was the most annoying part lol cus u have to make sure every wire connects to the right pin or it shorts out.

**Phase 2: The PCB Layout (The Frontend)**
Once the logic was done, I moved to the actual physical PCB design. 
I deleted the default boring square board outline. Then I found a solid black Batman logo PNG on google, imported it as a `Document` layer in EasyEDA to use as a stencil, and literally traced it using the `BoardOutline` tool to make a custom cut-path for the factory router. 

Dragged all the LEDs onto the bat wings, and then used the Auto-Router tool to let the computer figure out how to lay down all the physical copper traces without them crossing.

## Manufacturing
I sent the final files directly to **JLCPCB**. They are the factory that actually bakes the fiberglass and cuts the Batman shape out. Used a new user coupon so a batch of 5 boards was super cheap. 

Just waiting on the mail now so I can actually solder the physical chips onto the board. Ill probably take some sick macro shots of the finished soldering with the 6D Mark I when it gets here. 

If ur trying to learn hardware, def recommend starting with a 555 timer circuit like this. Its a classic for a reason!
