# Artorius 
## A High-Performance CoreXY Platform Built for Precision and Speed

Artorius is a dedicated, enthusiast-grade coreXY 3D printer designed around achieving reliability, quality, and speed while cleverly utilizing repurposed industrial components, including BIQU B1 parts. This project represents an ongoing commitment to pushing the boundaries of open-source additive manufacturing.

***

### Project Background & Design Philosophy

The journey started in the spring of 2024. Initially, I began this project because my existing BIQU B1 unit struggled with speed and consistency; the goal was fundamentally to bring it up to a next generation standard. However, after the first physical iteration, the objective shifted: I realized the true aim was to build a machine that could operate at speeds and maintain a quality level comparable to modern commercial printers, such as the Bambulab P1S.

My design process was highly iterative, taking deep inspiration from established community projects like the E3NG, Voron Trident/2.4, Annex K3, Mercury One, and VZBot. The E3NG served as foundational support for the frame design, although I later determined that using two smooth rods as front support compromised ideal rigidity. Meanwhile, the principles observed in the Voron, VZBot, and Annex K3 informed my approach to wiring and aesthetics; specifically, adopting a side-mounted electronics setup (inspired by an Annex K3 user mod) provided a clean and aesthetically pleasing solution. Furthermore, designs like Mercury One inspired the motor mounting system, leading to the current configuration featuring two bearing stacks positioned paraboloically around the belts, with the motor situated behind them. Throughout every design phase, I focused on CADing only the parts intended for printing, relying on community-sourced reference geometry for all aluminum extrusions, electronics mounts, and hardware components.

### System Evolution & Core Improvements

The development of Artorius has required several major revisions to achieve its current state of reliability.
*   **Initial Prototype:** This first version successfully demonstrated high speeds but was fundamentally a rough prototype; it lacked proper electronics housing, clean cable management, or specialized filament handling (like reverse bowden setup). Changing filament and managing the path proved challenging due to minor inconsistencies in the reference geometries used for measurement. While functional, its reliability was poor, and performance lagged behind expectations.
*   **Current High-Power Revision:** The second iteration addressed these flaws by implementing a significantly improved frame. Here, the gantry and coreXY motion components were designed not just as mounts but as integral parts of the system structure itself. A key technical advancement included incorporating **motion-absorbing TPU inserts**, which effectively reduced noticeable rocking motion in the print bed while simultaneously improving rod fit and compensating for minor variations in linear rod machining lengths.

### Key Technical Systems & Components

To meet modern demands for speed and stability, the current build features several high-performance upgrades:

*   **Power System:** The system has been upgraded to run on a dedicated **48V power supply**, providing the necessary power headroom for increased speeds and accelerations.
*   **Hotend Performance:** We integrated the Mellow Heatercore 4 hotend, which, after testing, can reliably maintain print deposition rates of up to *30 mm^3/s* during regular PLA printing conditions ($473\text{K}$).
*   **Electronics Integration:** The electronics are mounted within a dedicated housing that supports key components: the Manta M8p motherboard, an external MOSFET for bed control, a USB-CAN board for toolhead connection, the 24V PSU, and the new 48V PSU. Structural integrity is further ensured by providing **double shear support** on motor shafts to prevent flexing when belts are over-tensioned.

### Future Roadmap

Artorius remains an evolving project. My immediate plans involve several critical additions designed to enhance both safety and functionality:
*   The construction of a protective enclosure for the entire system.
*   Adding dedicated cooling fans for all primary motors.
*   Developing self-designed components, including a sophisticated extruder assembly and modernized features like automated filament swapping cutters.

***
*Artorius is an example of continuous, hands-on engineering; each update is a step toward building the most refined, reliable coreXY printing platform possible.*
