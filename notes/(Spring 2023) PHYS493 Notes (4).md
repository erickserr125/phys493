# Notes for last week's work (1/17 and 1/19)

I worked on understanding the circuit which uses the quadratic-photodiode to interpret results. The quadratic photodiode uses four signals separated by a thin cross to provide information about the light that enters the region (such as the shift).

Typically, the quadratic photodiode has its regions labelled as `A` `B` `C` `D` with `A` adjacent to `B` and `D`. The following figure shows how we use these signals for the output:

![Original Schematic](https://github.com/erickserr125/phys493/tree/main/notes/images/202301_week3_orig_schematic.jpg=250x500)


Note that the signals `A,B,C,D` are **current sources**. When these four regions receive a light signal,it is interpreted in three ways, the "X-DIFFERENCE," the "Y-DIFFERENCE," and "QUAD MODE." The circuit for the quadratic photodiode provides the X-DIFFERENCE and Y-DIFFERENCE (as seen above), but we are charged with including 
"QUAD MODE." In general, the signals are interpreted as such.

* X-Difference: `A+D-(B+C)`
* Y-Difference: `(D+C)-(A+B)`
* Quad Mode: `(B+D)-(A+C)`

The following figure below demonstrates the derivation for each of these modes:

![XY-Derivation](https://github.com/erickserr125/phys493/tree/main/notes/images/202301_week3_xy_derivation.jpg=250x500)

![Q-Mode Derivation](https://github.com/erickserr125/phys493/tree/main/notes/images/202301_week3_qmode_derivation.jpg=250x500)

Using several transimpedance amplifiers, I created a signal circuit which outputs these currents in a superposition (which is converted to a voltage).

Finally, I began working on a PCB board design. with the help of Dr. Zhou, I found smaller, faster Ki-CAD files with a PCB footprint that I could use 
in place of the amplifiers and photodiode signal. The following image shows my progress on the schematic in Ki-CAD:

![Quad-PD schematic image](https://github.com/erickserr125/phys493/tree/main/notes/images/202301_week3_quadpd_schematic.png=250x250)

