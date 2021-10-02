# Training VSD---Physical-Verification-using-SKY130

## Contents:
- Day 1 - Introduction to SkyWater SKY130
- Day 2 
## Notes and Useful Links

- Documentation https://skywater-pdk--136.org.readthedocs.build
- PDK Library and Files https://github.com/google/skywater-pdk
- Community (Slack) https://join.skywater.tools
- open_pdks http://opencircuitdesign.com/open_pdks // https://github.com/RTimothyEdwards/open_pdks
- openlane https://github.com/efabless/openlane

## Tools
- Layout https://opencircuitdesign.com/magic https://www.klayout.de
- Schematic Editor: Xschem
- Spice Simulator: ngspice
- LVS tool: netgen

## Inverter Schematic
- Creating schematic for an inverter using Xschem tool.
- Useful shortcuts:
	- insert "add a new component"
	- c "copy"
	- m "move"
	- w "draw wire"
	- q "instance properties"  
![lab01_sch_01](https://user-images.githubusercontent.com/16929397/135584193-b8cbf605-de4a-4153-b16b-c1ec0ac7e20a.JPG)

## Inverter Test Bench

Input Voltage source waveform syntax
![lab01_sch_tb_01](https://user-images.githubusercontent.com/16929397/135584661-992d925c-a72a-448c-a846-f37578b35887.JPG)

### Testbench Environment 
![lab01_sch_tb_03](https://user-images.githubusercontent.com/16929397/135586429-ffd8a93b-f60c-43a9-8815-e82517badb19.JPG)

## Simulation Results
![lab01_sch_tb_04](https://user-images.githubusercontent.com/16929397/135586368-d0666c35-5d3d-46df-93c3-bae2f089116e.JPG)



## Inverter Layout
Using magic to draw inverter layout

magic shortcuts:
- i "select instance"
- s "select pins"
- what command to show instance info
- ctrl+p after selecting instance "instance properties"

## Lab2
# part 1
- Creating a new workspace 
- Open magic and read sky130 library gds
![lab02_v01_01](https://user-images.githubusercontent.com/16929397/135720178-941c2c8d-44ab-4cd9-8473-e8ff9173564c.png)
- list available cells
![lab02_v01_02](https://user-images.githubusercontent.com/16929397/135720222-eeceb18f-9a5d-4751-b0a4-52e97f58d460.png)
- Open a stdcell view using --> options --> Cell Manager
![lab02_v01_03](https://user-images.githubusercontent.com/16929397/135720257-f8182d04-3f09-4ee2-bcf6-590f5e0680d4.png)
![lab02_v01_04](https://user-images.githubusercontent.com/16929397/135720301-e198b10a-5f61-456e-9e7d-586c8778296e.png)
- List available styles
![lab02_v01_00](https://user-images.githubusercontent.com/16929397/135720100-e531a006-a4a7-4b41-8f48-dfa1324dab68.png)
- Switch between different available styles
![lab02_v01_06](https://user-images.githubusercontent.com/16929397/135720327-d919197a-0e18-41a3-8bb7-3f1f6921997a.png)

# part 2
In this part we explore the effect of LEF/SPICE on adding metadata info to GDS.

- Displaying port info
![lab02_v02_01](https://user-images.githubusercontent.com/16929397/135722350-f6fb02f1-ae79-4a46-bb97-eb235abb98ac.png)
- Reading LEF and report port info changes
![lab02_v02_02](https://user-images.githubusercontent.com/16929397/135722380-a8793c49-bb96-4d7f-96c1-b7486aa90924.png)
- Reading SPICE and report port info changes
![lab02_v02_03](https://user-images.githubusercontent.com/16929397/135722388-b719e459-7513-44c8-a398-f948b9c44fbe.png)
![lab02_v02_04](https://user-images.githubusercontent.com/16929397/135722396-b7a4eb52-f712-4686-bbc1-88ce20c7dd73.png)

