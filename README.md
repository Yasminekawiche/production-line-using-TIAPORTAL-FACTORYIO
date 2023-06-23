# FACTORY :
The selected industry is the plastic boxes and glass bowls industry, and the production domain is the manufacturing of plastic boxes and glass bowls. The raw material is moldable plastic. The finished products are plastic boxes and glass bowls.

There are three workstations: molding for boxes, assembly of boxes, and labeling of boxes and glass bowls.

- Molding of boxes:
The first step is molding, where the moldable plastic is conveyed to the first workstation using a conveyor.
At the first workstation, a machine injects the moldable plastic into molds to obtain the first part of the box.
The workstation's capacity would be 1 piece/30s. The production rate would be one molding cycle every 30 seconds.

- Assembly of boxes:
The second workstation is the assembly of boxes. The assembly workstation is responsible for assembling the two parts of the box using an automated assembly machine. The boxes should be stackable and shock-resistant, with a failure rate of less than 1%.
The workstation's capacity would be 1 box/10 seconds.

- Labeling of boxes and glass bowls:
The third labeling workstation is responsible for labeling the finished products (assembled plastic boxes and glass bowls).
The workstation's capacity would be 1 finished product/10 seconds.
Once the assembled plastic boxes and labeled glass bowls are ready, they are conveyed to the output stock using a conveyor.
The output stock contains the finished products ready to be organized by employees and shipped to customers.

The production line organization includes:
- Input and output stocks.
- Three workstations (plastic molding, assembly of box parts, labeling of semi-finished products).
- Handling equipment (conveyors).
- Production flows from the input stock to workstations, then to the output stock.

Each workstation is equipped with a specific machine designed to perform a specific task:
1. Plastic molding machine.
2. Assembly machine.
3. Labeling machine.
The machines are controlled by automated systems to ensure precise and efficient operation.

Conveyance methods:
- For moldable plastic: a conveyor would be used to transport the melted plastic to the first molding workstation.
- For the first part of the box: after the molding process, the piece will be conveyed to the second assembly workstation using another specific conveyor.
- For the second part of the box: the pre-assembled piece will be conveyed to the second assembly workstation using another specific conveyor.
- For assembled boxes: the boxes will be conveyed to the third labeling workstation using a specific conveyor.
- For glass bowls: a conveyor would be used to transport the glass bowls to the third labeling workstation.

Input stock:
- Moldable plastic
- Glass bowls

Output stock:
- Labeled assembled boxes
- Labeled glass bowls

Let's consider two finished products: AEB (Assembled and Labeled Boxes) and GLB (Labeled Glass Bowls), with the following raw materials: RM1 (moldable plastic), RM2 (second part of the box), RM3 (glass bowls), and RM4 (labels), and two semi-finished products: SF11 (molded piece) and SF12 (assembled box).

The product transformation flow is as follows:
For AEB: RM1 → SF11 (molded piece) → SF12 (assembled box) → AEB
For GLB: RM2 → GLB

Human-Machine Interface:

● The HMI could include a touchscreen display to show real-time information about the status of the production line.

● The touchscreen display contains an emergency stop button, the switcher (switches between DCY and FCY), 3 tiles in red, green, and orange that indicate, respectively, whether the emergency button is pressed, the production line is running normally, or the FCY button is pressed. There are also two numerical indicators showing the quantity of the two produced products.

● The automatic mode allows the production line to operate autonomously without human intervention, using sensors and actuators to detect and adjust production parameters such as conveyor speed. This mode is used when the raw material is loaded into the input stock, the system is ready to operate without human intervention, and the DCY mode is enabled. If DCY is still active, this cycle repeats. Activating FCY mode stops the raw material loading, which means the current cycle completes normally, and no new cycle starts.

● For system shutdown, it can be automatically performed using an emergency stop button (AU) from any state, cutting off the power supply to all machines simultaneously and causing a complete system stop.

PROGRAMS : 
---------------------------------------------------------------------------------
- TIAPORTAL V16
- Factory IO
- PLCSIM

GUIDE : 
-----------------------------------------------------------------------------------
To run the simulation, follow these steps:

- Open the TiaPortalV16 program on your computer.
- Once the program is launched, locate and run the simulation. The PLCSim will 
start automatically, simulating the behavior of the programmable logic controller.
- Next, open the Factory IO software. This application provides a virtual environment for simulating industrial processes and equipment.
- Within Factory IO, you will find an interface known as the IHM (Interface Homme Machine) or Human-Machine Interface. Open the IHM to gain control over the simulated factory and its components.
- From the IHM, you can send commands and instructions to control various aspects of the factory's operations, such as activating/deactivating machinery, adjusting settings, or initiating processes.

By following these steps, you will be able to run the simulation and utilize the IHM to command and interact with the virtual factory environment.
