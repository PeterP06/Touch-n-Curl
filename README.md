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
|---------------|------------------|----------|----------|----------|---------------|------------------|------------------|
| <img width="60" height="60" alt="rules" src="https://github.com/user-attachments/assets/edaac219-1d70-40a7-92ec-9b2132992b9c" />|
 <img width="60" height="60" alt="ribbon" src="https://github.com/user-attachments/assets/1899e7ca-bb1f-4781-8c79-f766af3fc4c3" />|
 <img width="60" height="60" alt="flatten" src="https://github.com/user-attachments/assets/c38c7353-054d-419e-83a9-bdedd852603b" />｜
 <img width="60" height="60" alt="raw_unit" src="https://github.com/user-attachments/assets/e35ac313-32f7-4529-b680-26bf845db4fe" />｜
 <img width="300" height="300" alt="side_cut" src="https://github.com/user-attachments/assets/8495b2de-aea2-4480-9446-7a22ea3d9ad1" />｜
 <img width="60" height="60" alt="unit_cut" src="https://github.com/user-attachments/assets/bb19142c-9c30-4013-9c4e-de8630e1f8db" />｜
 <img width="60" height="60" alt="featured_unit" src="https://github.com/user-attachments/assets/922243f8-c4a6-4a60-9aef-f0958e69ece4" />｜ - ｜
 






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
