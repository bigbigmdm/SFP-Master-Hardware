# SFP-Master-Hardware

**SFP-Master** is a free, cross-platform program for programming optical SFP modules. It allows you to read, write, and save SFP module data on a computer.
Software part of **SFP-Master** project is [here](https://github.com/bigbigmdm/SFP-Master). The description of the hardware is provided here.

![Cover image](img/sfp-master-1-1-2_cover.png)

The hardware part of SFP-Master can be assembling in two variants:
* [Adapter](#adapter) for very popular low cost CH341 programmer device.
* [SFP-Master device](#sfp-master-device)

## Adapter

![Adapter](img/adapter_h.png)
This adapter must be connected to the section of the CH341 programmer's ZIF socket marked with the "24xx" symbols. At the same time, the ZIF socket lever must fit into the oval cutout on the adapter board.

![Connection](img/connection.jpg)

### Schematic diagram

![Adapter schematic](img/sfp-adapter-sch.png)

Jumpers J1 to J3 (TxPWR, RxPWR, TxEN) must be installed initially. They are used to supply power to the SFP module. If you want to program a module with hardware write protection, remove one of the jumpers and try to program the module. If it fails, remove the other jumper and repeat the operation.

Bill of material:

| ID  |  Name                | Footprint | Designator          | Quantity |
|:---:| :---                 | :---      | :---                |  :---:   |
|  1  |  P1                  | H1        | HDR-TH_4P-P2.54-V-M |     1    |
|  2  |  P2                  | H2        | HDR-TH_4P-P2.54-V-M |     1    |
|  3  | XDZ254-1-02-Z-2.5-G1 | J1,J2,J3  | HDR-TH_2P-P2.54-V-M |     3    |
|  4  | SFP插座-20PINSFP 	   | P1        | CONN-SMD_SFP-20PIN  |     1    |
|  5  | 4.7kΩ	               | R1,R2,R3  |   R0805             |     3    |

### Printed circuit board

![PCB](img/sfp-adapter-pcb.png)

## SFP-master device

![Adapter](img/sfp-master-device.png)
