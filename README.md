# SCHEMATIC ENTRY AND CIRCUIT SIMULATION OF A CMOS INVERTER, TWO INPUT NAND GATE, TWO INPUT NOR GATE

# AIM:
To simulate the design of CMOS inverter, NAND, NOR from schematic using cadence.

# APPARATUS REQUIRED:
cadence

# PROCEDURE:

## Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
          i)	tcsh
          ii)	source /home/install/cshrc
          iii)	virtuoso 
## Procedure for Schematic simulation using Cadence
1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
          i)	Create a New Library
          ii)	Create Schematic Cell view.
          iii)	Create the Symbol for schematic Cell view.
          iv)	Create the test Cell view.
          v)	Analog simulation by spectre
## Procedure for Creating New Library.
a)	File –New – Library
b)	Name : Give name for ur library Ex: VLSILAB , Enable Attach to an existing technology library, Click OK
c)	Attach the library to the technology library gpdk045.Click OK
## Create Schematic Cell view.
a)	Go to 1st window i.e virtuoso(CIW)
b)	File-New-Cell view
c)	Setup the new file form, Library: Select the one you a created. Cell : Give the experiment name Ex: Inverter View: Schematic
d)	Type: Schematic press OK
e)	Add the required components from the libraries and make the connections.
f)	Go to instance fixed menu or use shortcut key “I” from keypad to go instances Click on browse. This opens the library browser ow select the appropriate library for components like Gpdk045,nmos, pmos
g)	Analog library	Vdd, Gnd, Vcc, Vpulse, Vsin
h)	Make the connections by using fixed narrow wire key
i)	Click Check and Save button


## Creating the Symbol for schematic Cell view
a.	In the schematic window, execute
          Crate – Cell view – From Cell view
          The cell view from cell view window appears
          Check Lib Name, Cell Name, From View name must be schematic Press ok
b.	Now Symbol generation form appears. Click Ok If No changes required
c.	A new window with with default symbol is created.
d.	Edit the symbol if you want to give actual symbol shape else continue.
          i.	Execute Create-Cell view-from cell view
          ii.	Library Name and Cell Name must be same which you have used for schematic. Press OK
          iii.	Check for the position of pin side.Prss OK
          iv.	Edit for the shape by Create-Shape-Choose required options to edit.
## Creating the new test cell view

a)	Go to CIW window, Execute File-New-Cell view
b)	Setup the new file form
Library: Select the one you a created.
          Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
          View: Schematic
          Type: Schematic  press OK
## Analog simulation by SPECTRE.
a.	In test cell view window
i.	Launch – ADE L(Analog Design Environment)
b.	Execute Setup—Simulation/directory/Host A new window opens
c.	Set the simulation window to spectre and click ok
d.	Execute Setup-Model Library. Anew window opens, Check of gpdk.scs as lib and section type as stat then press OK.
e.	Execute Analysis – Choose. A window opens.
f.	Select the type and set the specifications and press OK
g.	Execute Output s—to be plotted – Select on Schematic
h.	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
i.	Execute Simulation -- Net list and Run

# INVERTER SCHEMATIC:

![image](https://github.com/Princyagnes/VLSI-LAB-EXP-6/assets/115100663/0b6c7198-06d8-4238-855a-b6fcc1285af2)

# SPECIFICATIONS:

# Vpulse
    V1 = 0	       
    V2 = 1
    td = 0,tr=tf=1 n, ton= 100n ,T=200n

Vdc = 1

# SIMULATION SETTINGS:
# Setup for transient analysis:
  1. Stop time = 400n
     
# Setup for D.C analysis:
1. Component to be selected in schematic is for d.c analysis
2. Start = -1 Stop = -1 resp.
   
# EXPECTED WAVEFORM:

# TRANSIENT ANALYSIS:

![image](https://github.com/Princyagnes/VLSI-LAB-EXP-6/assets/115100663/a326e7a2-0a68-4e3a-b1d3-101dec661ca0)

# DC ANALYSIS:

![image](https://github.com/Princyagnes/VLSI-LAB-EXP-6/assets/115100663/823b19d9-e491-429b-982a-863a89f1355e)

# NAND SCHEMATIC:

![image](https://github.com/Princyagnes/VLSI-LAB-EXP-6/assets/115100663/95256cba-580d-4738-9107-e884deb11c06)

![image](https://github.com/Princyagnes/VLSI-LAB-EXP-6/assets/115100663/cd72d5a8-e81d-4789-9126-086bd4dd5056)

# SPECIFICATIONS:

# Vpulse:

Va1 = 0 Va2 = 1 tr=tf=50ps, period=20ns pulse with = 10ns
Vb1 = 0 Vb2 = 1 tr=tf=50ps, period=40ns pulse with = 20ns
Vdc = 1

# EXPECTED WAVEFORM:
 # TRANSIENT ANALYSIS:

 ![image](https://github.com/Princyagnes/VLSI-LAB-EXP-6/assets/115100663/f482980d-d6d2-43a3-9b16-98d0d414e805)

# NOR SCHEMATIC:

![image](https://github.com/Princyagnes/VLSI-LAB-EXP-6/assets/115100663/7efcd2de-e225-470f-b425-ebaa7d1b7372)

![image](https://github.com/Princyagnes/VLSI-LAB-EXP-6/assets/115100663/d8cd8679-58b7-4fc8-826c-c56c23e8f9a3)

# SPECIFICATIONS:

# Vpulse:

Va1 = 0 Va2 = 1 tr=tf=50ps, period=20ns pulse with = 10ns
Vb1 = 0 Vb2 = 1 tr=tf=50ps, period=40ns pulse with = 20ns
Vdc = 1

# EXPECTED WAVEFORM:
 # TRANSIENT ANALYSIS:

 ![image](https://github.com/Princyagnes/VLSI-LAB-EXP-6/assets/115100663/6df8b432-a6a1-44f2-845f-7a9562b71a99)

# RESULT:

Thus, the design,simulation and verification of the CMOS inverter,NAND,NOR from schematic using cadence was successfully completed.
