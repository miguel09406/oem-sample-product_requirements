OEM sample PRD (Product Requirement Document)
=============================================

Project I-O-T (OEM-Partner Automation System Processor)

OEM P/N: OEM-SAMP

Home Automation Control System - A Complete AV System Controller with HTML and iPAD Control


Overview
--------

OEM-Partner's OEM-SAMP is a complete Automation System that offers control of video, audio, lighting, and other systems using OEM-Partner components. It features a HTML5 Web User Interface that is optimized for iPad, iPod, iPhone, Android, and similar tablets and smart-phones as the display and control interface.

-	The OEM-SAMP system is unique in that it is designed to run on a home or business network, rather than as a stand-alone controller with dedicated cabling, making it ideal for retrofit or distributed system designs. 
-	The system consists of a hardware component and a software component.  The hardware component is the OEM-Partner's OEM-SAMP (Linux Automation System). The software is the OEM-Partner's OEM-SAMP.
-	The control program, or “Daemon”, runs on a small fan-less low-power Linux processor (OEM-Partner's OEM-SAMP). The processor simply plugs into an Ethernet connection. It uses an 18V DC power supply, or can be powered over Ethernet 	(PoE) with the Alix POE1a2 passive POE Adapter. It has no other active connections.
-	The OEM-SAMP processor also runs “Command Servers”, which contains the interface drivers for the controlled devices, and the Device Library.  
-	The Device Library contains IR, LAN and RS-232 codes for each audio or video component that the system can control, along with button layouts, button names, etc.  
-	The OEM-SAMP processor also contains an optional Z-Wave interface for control of lighting and other appliances.
-	The OEM-SAMP system communicates with the OEM-Partner's THING and Mini-THING control interfaces via the Ethernet Network, providing direct control via IR, RS-232 and Trigger outputs. The THING device(s) may be located next to the 	devices that are being controlled, and multiple THING's or Mini-THING's devices may be deployed in distributed A/V systems.
-	The OEM-SAMP system also communicates directly with OEM-Partner's IP products over the Network.
-	OEM-SAMP features a high-level user-friendly configuration interface, allowing quick and simple system setup without requiring extensive programming or installer training, making it ideal for OEM-Partner’s world-wide network of 	installers.
-	OEM-SAMP does not require Internet access for configuration or use. All files are contained within the OEM-SAMP processor.




General Concept
---------------

All components of the Product shall be hosted in the same hardware and it should be configurable without Internet access.
The OEM-Partner's THING IR learner will store the IR codes in specific locations as specified in the OEM-SAMP system configuration menu. The client should learn the HEX code in the defined pattern of the addressed device.

Serial codes can, for the first step, only be retrieved from the fixed OEM-SAMP Library. The first version of the OEM-SAMP will only offer fixed templates (e.g. TV, Disc-Player, etc.). The product is designed to allow the end-user to configure the system themselves, and all advanced editing capabilities (e.g. .CSV files, etc.) will be locked.

A Wizard or a Step-by-Step guide will prevent the end user from missing any important steps needed to make the Product work properly.



Product Version 1:
------------------

The first Product should have the following basic specifications and shall allow upgrades and increases in functionality, via the Internet or through a USB port. 
The below listed characteristics are necessary for the Product launch.

-	The Product allows IR control of devices (e.g. TV, Cable Box, Receiver, and Disc Player) via the OEM-Partner's THING, Mini-THING, (or ev. other 3rd-Party Gateways, such as Global Cache, IRTrans, and/or Moxa) The devices can be 	learned within a fixed template through the IR receiver in the THING, or downloaded from the Library in the OEM-SAMP.
-	The Product allows control of RS-232 serial devices (e.g. Matrix, Amplifier, Video-Processor, etc.) This control is limited to OEM-Partner's products only. These supported devices must be pulled from a Library in the Product. 	(This feature requires that nomos system AG receives all the Products for prior testing and implementation in the Library).
-   	The Product can be configured via a simple “editor tool” (standalone software or via HTML5). The functionality of the “editor tool” will be kept simple and provides only basic functions. The graphic library provides fixed GUI 	templates consisting of basic sliders, buttons and text fields. The “editor tool” shall remain upgradable for further increments.
-   	The Product shall be remote controlled via a browser. Only specific Web browsers (to be specified) will be supported.
-   	The Product shall be delivered with “discovery” software to recognize and find the IP address of the Controller once it is plugged into the local Network. This will allow the configuration of the Product on the Controller.
-   	The LINUX Hardware will be evaluated by nomos system AG for its compiling abilities and purchased by OEM-Partner directly.
 
 
 
Product Version 2:
------------------

The second product revision shall have the following basic specifications and shall allow upgrades and increase in functionality according to feedback gathered in the market. The features listed below, as a minimum, will be included in the second revision of the Product. Many of these features will be included in the TRADESHOW-Release-Date demo system. All systems shall be upgraded to the Version 2 revision at no cost when it is released.

-   Support for Z-Wave Gateway will be integrated into the Product. Once the specific gateway is selected and specified, nomos system AG will implement basic functions of the Gateway into the Product. The goal shall be to configure the 	controllability (e.g. of a dimmer or an I/O module) through the “Editor tool”.
-	AppleTV 2 “semi bi-directional” integration
-	“Macro” functions
-	“Power Memory” may not be implemented in version 2. It will be on the feature list for the future.
-	iOS App to allow faster and more seamless operation and feedback from iPad, iPod, and other iOS devices.



Z-Wave Gateway:
---------------

The Z-Wave Gateway may be either an internal board mounted in the OEM-Partner enclosure with an external antenna, or may be an external USB “stick” with an integrated antenna.
The internal design will be more elegant, but may require additional time and costs for compliance testing and certification, while the external USB device should already be certified, and should lower costs and reduce time-to-market.



Editor tool (standalone Software or via HTML5):
-----------------------------------------------

We designed the Editor tool as a simple configurator (standalone software or via HTML5). The philosophy is to pre-produce fixed GUI-Templates and then just assign the command pattern for that device. With that philosophy we can pre-define and explain to the client how to setup and integrate his system, the biggest challenge is to avoid variables.

From our experience we learned that all systems are going back to 3 simple basics - Multi-room, Two-Channel and Multi-Channel – all system variations have the same roots of these known elements.



Hardware (EXT-LAST) Interface:
------------------------------

The OEM-Partner's OEM-SAMP Linux Processor shall incorporate the XILA 3D2 processor board from Board Manufacturer. The LINUX Hardware will be evaluated by nomos system AG for its compiling abilities and purchased by OEM-Partner directly. The enclosure will be purchased from OEM-Partner and may choose to design an enclosure for the board.

Board Manufacturer XILA boards are small form factor system boards optimized for wireless routing and network security applications.


Features:
---------

-	AMD Geode LX CPU, 433 MHz (LX700) or 500 MHz (LX800) 5x86 CPU,
-	256 KB cache (64K data + 64K instruction + 128K L2)
-	1 to 3 Ethernet channels (Via VT6105M, 10 / 100 Mbit/s)
-	1 or 2 miniPCI sockets for 802.11 wireless cards and other expansion
-	1 miniPCI Express socket for GSM / UMTS cards (XILA.6)
-	128 or 256 MB DDR SDRAM, 64 bit wide for high memory bandwidth
-	512 KB flash for Board Manufacturer “tinyBIOS”
-	CompactFlash + optional 44-pin IDE header for user’s operating system and application
-	7 to 18V (absolute maximum) DC supply through DC jack or passive power over Ethernet
-	1 serial port (DB-9 male, RXD / TXD only)
-	2 USB 2.0 ports (optional)
-	Header for LPC bus (use for flash recovery or I/O expansion)


OEM options:
------------

The following options can be configured for larger orders:

-	DRAM size (128 MB, 256 MB)
-	CPU speed (LX700 / LX800 / LX900)
-	Delete I/O not required by customer
-	CMOS level serial port (RXD / TXD only)
-	Optional RTC battery


Compact Flash Cards:
--------------------

The following requirements need to be fulfilled for the internal CF Card:

-	NAND Technology
-	Industrial Usability / Certification
-	Minimum 4GB memory


Part numbers:

-	xila3d2 = 1 LAN / 2 miniPCI / LX800 / 256 MB / USB


Specifications: 	

-	CPU: 500 MHz AMD Geode LX800
-	DRAM: 256 MB DDR DRAM 
-	Storage: CompactFlash socket 
-	Power: DC jack or passive POE, min. 7V to max. 20V 
-	Three LEDs 
-	Expansion: 2 miniPCI slots, LPC bus 
-	Connectivity: 1 Ethernet channel (Via VT6105M 10/100)
-	I/O: RS-232 DB-9 serial port, dual USB 
-	Firmware: tinyBIOS
-	Configuration 1 LAN / 2 miniPCI
-	Power Consumption- about 2.5 to 3.5W at Linux idle, peak about 5W (without miniPCI cards and USB devices.)
-	18V DC / 15W power supply. 
-	Center pin = positive, sleeve = ground, 2.1 mm diameter.
-	Temperature range: 0 to 50°C.
-	Dimensions: 100 x 160 mm (3.93” x 6.3”)


Connections (User-Accessible):	

-	(1) Ethernet Port
-	(2) USB Serial Ports
-	(1) External Power connector (may be powered via PoE)

	
Note:
Depending on the enclosure used, the bottom side miniPCI socket will not support radio cards with higher profile MMCX connectors.

Manufacturer:
Board Manufacturer GmbH, Kuala Lumpur, Malaysia

Origin:
Taiwan



XILA 3D2 Federal Communications Commission Statement:
-----------------------------------------------------

-	This device complies with Part 15 of the FCC Rules. Operation is subject to the following two conditions: 
-	(1) this device may not cause harmful interference, and 
-	(2) this device must accept any interference received, including interference that may cause undesired operation.
-	This equipment has been tested and found to comply with the limits for a Class B digital device, pursuant to Part 15 of the FCC Rules. These limits are designed to provide reasonable protection against harmful interference in a 	residential installation. This equipment generates, uses, and can radiate radio energy. If this equipment is not installed and used in accordance with the manufacturer’s instructions, it may cause harmful interference to radio 	communications. 

-	However, there is no guarantee that interference will not occur in a particular installation. If this equipment does cause harmful interference to radio or television reception, which can be determined by turning the equipment off 	and on, the user is encouraged to correct the interference by one or more of the following measures:
-	Reorient or relocate the receiving antenna.
-	Increase the separation between the equipment and receiver.
-	Connect the equipment to an outlet on a circuit different from that to which the receiver is connected.
-	Consult the dealer or an experienced radio/TV technician for help.
-	This board is designed for installation in a shielded enclosure (metal or plastic with conductive coating). Shielded cables are required on LAN and serial ports to assure compliance with FCC regulations.
-	A copy of the test report will be provided on request.


CE Declaration of Conformity:

-	We, Board Manufacturer GmbH, declare that XILA.2, XILA.3 and XILA.6 series boards, when installed in Board Manufacturer GmbH metal enclosures. (case1c1 / case1c2 / box2c), are in conformance with:
-	EN 61000-6-3 (2005) (emissions, residential and industrial)
-	EN 61000-6-2 (ESD, susceptibility, residential and industrial)
-	The unit under test is in conformity with the standards mentioned above. A copy of the test report will be provided on request.


XILA system board 5 5/5/2010 Compliance information:

-	For FCC, XILA has been tested as a CPU board, installed in an enclosure, with the top cover removed. No further testing should be required if the board is used with other FCC tested modular components. Please see http://www.fcc.gov/oet/ for more details. The responsible party for FCC is the importer.
-	Testing for CE mark must be done at the level of the complete product, possibly including the wireless cards. Please contact Board Manufacturer GmbH for assistance and documentation.
-	For satisfactory resistance to electrostatic discharge events (ESD), the XILA board should be grounded (e.g. through the mounting holes, or the serial port connector). The USB port on XILA.2B / XILA.3B boards is sensitive to ESD events, spurious over-current events may be detected in this version.



Desired Control Features:
-------------------------

-	iOS / Android UI Control
-	Re-labelable buttons
-	Metadata / cover art page
-	Favorite Channel button pages
-	Configuration download and off-line project editing
-	Use internal accelerometer for auto turn-on/off
-	Store IR, RS-232, CEC, URL commands in local banks
-	Configure TCP/IP settings
-	Configure RS-232 settings for each port: baud rate, flow control, parity, etc.
-	Action scheduler to trigger action(s)
-	Schedule programs with a name, description and unique Action ID.
-	Timer: start time, schedule (weekdays, weekends, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday)
-	Firmware field upgrades. Upload FW file thru web UI.
-	Upload/Download learned/programmed commands as a text file
-	Upload IR, RS-232, CEC command files from 3rd party databases
-	System wide reset: Delete all actions, programs, and internal settings.
-	Learn IR remotes
-	Event Engine: Allow the scripts to follow state of another trigger.



Compliance:
-----------

-	FCC, UL (power supply), CE, EMC, RoHS, Energy Star



Packaging (OEM-Partner Giftbox):
--------------------------------

-	(1) OEM-SAMP Audio/Video Control System
-	(1) power supply (18V / 1.2A)
-	(1) Software License
-	(1) User’s Manual



OEM-SAMP Processor Enclosure:
-----------------------------

-	Size: 113 x 163 x 30 mm (4.45 x 6.42” x 1.18”)
-	Material: Aluminium
-	Fan-less design
-	Color: TBD (OEM-Partner Design: 4.35 x 6.42 x 1.18)

