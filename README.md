# Particle-counter-V1
PIN_Diode based radiation particle counter with differential sensing

This is a beta/gamma particle detector designed with differential sensing of the PIN diode signal, to establish some rejection of common-mode EMI. Transimpedance amplifiers with high gain are very similar to an oscilloscope probe amplifier: high impedance and very sensitive to external interference. By sensing symmetrically across both sides of the diodes, common-mode rejection of 40dB can be achieved. In batches of 1% resistor and 5% capacitor tolerances, matching can be achieved of 0.1% for R and 1% for C. This will yield 40dB CMRR.

This design is intended for remote sensing for balloon flights or similar weight-sensitive applications: assembled weight is 3.3g. As such, the added weight (and difficulty) of shielding is avoided, or reduced, by incorporating common-mode rejection.

Notes:
For U1 and U3, good opamps are: OPA-2376, AD8692 or TLV2772. U2 is an MCP602.
A charge pump voltage doubler is needed to increase the reverse bias across the PIN diodes: this enlarges the diode depletion region, which is where particle detection takes place. The reverse bias makes AC coupling to the opamps necessary.

Do not exceed 5.5V Vcc.

Steve
