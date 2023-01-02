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

Flip flops
- Set and reset are synchronous and take effect on the next clock cycle.
- Preset and clear are asynchronous and take effect _immediately_.

References
- Decade counter schematic: https://en.wikipedia.org/wiki/Counter_(digital)#Decade_counter
- 7400 series: https://en.wikipedia.org/wiki/List_of_7400-series_integrated_circuits
- Digital clock from scratch: https://medium.com/@erikvanzijst/a-digital-quartz-clock-from-scratch-a80ec5e427
  - Logic is easy, producing a clock signal from scratch is hard
