# Touch-n-Curl

## About Touch-n-Curl

Touch-n-Curl is a design and construction system for rapidly prototyping 3D skeletal curved structures, covering scales from millimeters to meters, by printing 2D zipper assemblies with interlocking mechanisms using conventional 3D printers. This parametric design tool is developed to support this inverse design workflow, instantly generating 2D zippers and offering a preview of the 3D skeletal assembly.

This program is based on Rhino&Grasshoper and exist as a plug-in of Grasshopper. Its input is a skeleton form(curve only for now) and output is zipper pair for 3D-printing. For further information, please refer to our paper:

## Installation

### Prerequisites

- A computer compatible with Python 3.8 or higher
- Rhino 8 with Grasshopper (Grasshopper is included by default when installing Rhino)
- Wombat (A plugin for Grasshopper)
  - For Windows or Mac with Intel chips users: Drag the [example file](./Example.gh) into Rhino and follow the on-screen instructions `OR` download from [Food4Rhino](https://www.food4rhino.com/en/app/wombatgh)
  - For Mac with Silicon chips users: Download from [Food4Rhino](https://www.food4rhino.com/en/app/wombatgh) and move the downloaded folder to a path similar to `/Users/YOUR_USER_NAME./Library/Application Support/McNeel/Rhinoceros/packages/8.0`

### Configuration

1. Download [cluster files](./Touch-n-Curl%20Clusters) 
2. Move the folder into a path similar to `/Users/YOUR_USER_NAME./Library/Application Support/McNeel/Rhinoceros/8.0/Plug-ins/Grasshopper/UserObjects`(for Windows users： `C:\Users\YOUR_USER_NAME\AppData\Roaming\Grasshopper\UserObjects` ).
3. Restart Rhino and enjoy.

## Getting Start

There are currently 8 components to generate a zipper pair from a curve named `Rule Generation`, `Raw Unit`, `Flatten`, `Base Cut`, `Unit cut`, `Ribbon`, `Featured Unit`, `Zipper Rearrange`. Each of them is comprised of a input list, a cluster of batteries, an output list and an icon. The icons are listed in the following table:


| Rule Generate | Ribbon | Flatten | Raw Unit | Base Cut | Unit Cut | Featured Unit | Zipper Rearrange |
|------------------|------------------|------------------|------------------|------------------|------------------|------------------|------------------|
| Data 1   | Data 2   |

### Rule Generation

**Input**: This Component have 5 inputs and the informations are listed below:
- Curve: The input space curve
- Alpha: One of the two angles that decide the direction of the first rule
- Beta: Another angle for direction
- i: The multiplier of the overall scale of units
- Curve_Scale: The multiplier of the scale of input curve

**Output**: This components have 4 outputs and the informations are listed below:
- Rules: Rules calculated sequential according to the initial rule direction determined by Alpha and Beta
- Points: Points for dividing the space curve
- B_vec: Binormal vector at each point
- T_vec: Tangent vector at each point

**

## Communication

## Acknowledgement

## License