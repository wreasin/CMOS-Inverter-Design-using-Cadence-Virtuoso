# CMOS-Inverter-Design-using-Cadence-Virtuoso
### CMOS Inverter Design with Layout and Analysis using Cadence Virtuoso
---
<!-- Cadence Project (Transient & DC Response With Layout) -->

I’m thrilled to announce that, this is my first project on __Cadence Virtuoso__. I am design here a CMOS inverter with it's layout.

Here i have use __gpdk90n__ :-
1. pmos1v and nmos1v
2. For vdd i have use vdc (1.8v)
3. For input i have use vpulse
4. Here I am doing two types of Analysis :  
    i ) Transient Response  
    ii ) DC Response  
    N.B. I'm measuring here input & output as Voltage and Current (I) in Output & VDD node.
5. In Layout - Metals Used ( Metal1 ) and Poly Layer
6. The minimum width of metal utilized for routing is 0.012
7. DRC and LVS clean (there are no error)

___Before i explain my project in details let you know one thing !___

### What is CMOS Inverter?
Complementary-Metal -Oxide-Semiconductor (CMOS) is a type of metal–oxide–semiconductor field-effect-transistor (MOSFET) fabrication process that uses complementary and symmetrical pairs of p-type and n-type MOSFETs for logic functions. CMOS technology is used for constructing integrated circuit (IC) chips, including microprocessors, microcontrollers, memory chips and other digital logic circuits.   

CMOS inverter definition is a device that is used to generate logic functions is known as CMOS inverter and is the essential component in all integrated circuits. A CMOS inverter is a FET (field effect transistor), composed of a metal gate that lies on top of oxygen’s insulating layer on top of a semiconductor. These inverters are used in most electronic devices which are accountable for generating data n small circuits.

_An interesting obseration was made in the previous section, where we realised that neither NMOS nor PMOS can be used for design that can produce either values, HIGH and LOW. But another thing that is worth notice is how they complement each other. This is what gave rise to an idea of attaching them together. Since, PMOS is a Strong 1, we put it between VDD and Vout and NMOS being a STRONG 0, it is placed between Vout and GND. This way, either can act as a load to the other transistor, since both are never ON together (Are they?). The configuration looks like what we have below. This is referred to as Complimentary Metal Oxide Semiconductor(CMOS) Configuration and it also represents the simplest circuit known as the CMOS Inverter._

### The Project details of mine :
So I designed a Schematic of the CMOS Inverter, where the whole thing is based on gpdk 90n. I have use pmos for 1v and nmos for 1v. I also designed a symbol of it, so that we can utilise that for further schematic creation.  
![Scametic](https://github.com/wreasin/CMOS-Inverter-Design-using-Cadence-Virtuoso/blob/main/Image/Scametic.PNG?raw=true) 
![Symbol](https://github.com/wreasin/CMOS-Inverter-Design-using-Cadence-Virtuoso/blob/main/Image/Symbol.PNG?raw=true)
![Symbol_Scametic](https://github.com/wreasin/CMOS-Inverter-Design-using-Cadence-Virtuoso/blob/main/Image/Scametic_Diagram.PNG?raw=true)

#### DC and Transient Response :
_Here I am doing two types of Analysis - DC and Transient_.  
In DC and Transient Analysis i have measured input & output as Voltage, and Current (I) in Output & VDD node. The plots of _IN_ and _OUT_ shows the _voltages_, on the otherhand _VDD(I4)_ & _OUT(I4)_ shows the _current (I)_.
![output](https://github.com/wreasin/CMOS-Inverter-Design-using-Cadence-Virtuoso/blob/main/Image/All_Output.PNG?raw=true)
![output2](https://github.com/wreasin/CMOS-Inverter-Design-using-Cadence-Virtuoso/blob/main/Image/All_Output_2.PNG?raw=true)

#### Layout :
In Layout i have use  Metal1 and Poly Layer. I have use here X & Y snap spacing is 0.012m and also the minimum width of metal utilized for routing is 0.012.  
![Layout](https://github.com/wreasin/CMOS-Inverter-Design-using-Cadence-Virtuoso/blob/main/Image/Layout.PNG?raw=true)  

#### Design Rule Check (DRC)  
DRC is clean. There are no error in DRC.
![DRC](https://github.com/wreasin/CMOS-Inverter-Design-using-Cadence-Virtuoso/blob/main/Image/DRC%20Check.PNG?raw=true)  

#### Layout Versus Schematic (LVS)  
LVS is clean. There are no error in LVS.  
![LVS](https://github.com/wreasin/CMOS-Inverter-Design-using-Cadence-Virtuoso/blob/main/Image/InkedDVS%20Check.jpg?raw=true)
