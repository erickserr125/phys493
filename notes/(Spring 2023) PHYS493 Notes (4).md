# Notes for last week's work (1/17 and 1/19)

I worked on understanding the circuit which uses the quadratic-photodiode to interpret results. 
The quadratic photodiode uses four signals separated by a thin cross to provide information about the light that enters the region (such as the shift).

Typically, the quadratic photodiode has its regions labelled as `A` `B` `C` `D` with `A` adjacent to `B` and `D`. Note that the signals `A,B,C,D`
are **current sources**. When these four regions receive a light signal,it is interpreted in three ways, the "X-DIFFERENCE," the "Y-DIFFERENCE," 
and "QUAD MODE." The circuit for the quadratic photodiode provides the X-DIFFERENCE and Y-DIFFERENCE, but we are charged with including 
"QUAD MODE." In general, the signals are interpreted as such.

* X-Difference: `A+D-(B+C)`
* Y-Difference: `(D+C)-(A+B)`
* Quad Mode: `(B+D)-(A+C)`

Using several transimpedance amplifiers, I created a signal circuit which outputs these currents in a superposition (which is converted to a voltage).

Finally, I began working on a PCB board design. with the help of Dr. Zhou, I found smaller, faster Ki-CAD files with a PCB footprint that I could use 
in place of the amplifiers and photodiode signal. 
