Parts distributors 
- Elenco
- Jameco
- Digikey

Integrated circuits
- Dual inline packaging.
- Pinouts to make sense of inputs and outputs.
- TTL vs CMOS. CMOS more sensitive, more expensive, lower power. I have TTL ICs.

TTL family
- 5 volts.
- 7400 NAND
- 7402 NOR
- 7408 AND
- 7432 OR
- 7486 XOR
- 74266 XNOR
- 7447 BCD (binary-coded decimal) to 7seg
- 7474 D flip-flop
- 7475 Bistable latch (don't remember what this is?)
- 74148 Decimal to BCD encoder
- 7476 JK flip-flop. Two flip-flops wired together in a master-slave (unfortunate naming...) configuration
- 7490 decade counter. Saves you the trouble of wiring four JK flip flops sequentially.
- 75690 8-bit counter
- 74283 4-bit full adder

Flip flops
- Set and reset are synchronous and take effect on the next clock cycle.
- Preset and clear are asynchronous and take effect _immediately_.
- Edge triggered vs level triggered. The former seem to be preferred.

References
- Decade counter schematic: https://en.wikipedia.org/wiki/Counter_(digital)#Decade_counter
- 7400 series: https://en.wikipedia.org/wiki/List_of_7400-series_integrated_circuits
- Digital clock from scratch: https://medium.com/@erikvanzijst/a-digital-quartz-clock-from-scratch-a80ec5e427

Design notes for a digital clock displaying hours, minutse, and seconds in binary:
- 5 LEDs for 24 hours, 6 LEDs for 60 minutes, and 6 LEDs for 60 seconds means I'm using 17 LEDs total
- Place them in three rows
- Use an 8-bit counter with clear logic for hours, minutes, seconds, respectively?
- Switch for toggling between two modes: letting the clock run (default) and letting the user configure it
- Two push buttons: one for incrementing the hour and another for incrementing the minute
  - These should do nothing if the user is not configuring the time
- Use adders to increment the state? Or will the user pushing the button function as a clock signal?
