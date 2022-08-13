-- WIP!

**Turbines** are multi-block power generators that run on steam. The steam can be sourced from an active [reactor]() that boils water, or from a [heat exchanger](). In operation, the steam is condensed into water which can be fed back into the source or it can be voided.

TODO: insert part with turbine max size

## Required Components

**Turbine Casings** make up the frame and walls of the turbine.

**Turbine Fluid Ports** are used to insert steam and extract water. They provide a UI to set input or output status.

**Power Taps** are used to extract power.

**Rotor Bearings** are located at each end of the shaft of the turbine. Exactly 2 are required.

**Rotor Shafts** form the shaft of your turbine that spans end to end and connects to the rotor bearings.

**Rotor Blades** make the rotor spin by converting the thermal energy from the steam into angular momentum of the shaft.

## Optional Components

**Turbine Terminals** are the control panels of the turbine. A turbine multi-block will form without a terminal, but you can't do much without it.

**Turbine Glass** functions identically to casings, but may only be used on walls. It allows you to see inside of the turbine.

**Computer Ports** allow for control of various turbine functions via Lua scripting. This requires a computers mod such as [CC: Tweaked](https://www.curseforge.com/minecraft/mc-mods/cc-tweaked) to be installed.

## Construction
A Turbine is a cuboid multi-block structure, just like the reactor. The edges must be made of Turbine Casings, but the faces can be Turbine Glass or any of the other listed block components such as Fluid Ports and Terminals.

The turbine requires a rotor shaft which consists of Rotor Shafts and spans end to end in a straight line, touching two opposing faces. The shaft must connect to exactly two Rotor Bearings.

### Rotor Blades
Rotor Blades can be placed on any of the four sides of a Rotor Shaft and must not be disconnected from the shaft. The placement of the blades can be asymetric and this will not impact the turbine's performance.

### Coils
**Coils** turn the kinetic energy of the rotor into RF/FE. Coils consist simply of metal or metal-like blocks, placed around a Rotor Shaft component. It is not necessary to form complete rings around the shaft, and it is not necessary for coil blocks to be connected; they can be farther out from the center (see design section)

Note that you may *not* have more than one section of coils or blades. For example, it is not possible to have a section of coils in the middle of a turbine, and two sections of blades surrounding it. It is also not possible to have both coil blocks and rotor blades on one Rotor Shaft component.

## Design
Several factors influence the steam intake, power production and efficiency of the turbine.

### Coil structure
The material, number and positioning of the coil blocks determine the amount of power that will be produced and the minimum amount of blades needed for optimal operation.
- Doubling the number of coils essentially doubles the power produced and the drag on the rotor.
- The farther away a coil block is from the shaft, the less effect it has on the turbine (less power, less drag). This is summarized in the following diagram. TODO: insert diagram

  This fact leads to the conclusion that it is most resource efficient to have coils of the smallest ring size.
- Each allowed coil material has three values associated with it:
  - **Extraction rate** 
  - **Efficiency**
  - **Bonus**

  You can view the allowed materials and their stats on the [Coil stats]() page.

### Blade structure
The number of blades determines the steam intake of the turbine and how much steam the turbine can handle for certain RPM.




## Operation and control

A turbine spinning at 1800 RPM produces roughly twice the power of a turbine spinning at 900 RPM.



