# K2PRO
Adaptive Mesh for Creality K2PRO using Orca Slicer

Default is 5x5 mesh for small models also you can change printer.cfg for 7x7 and 9x9 manual with save config.
For now i cant find the solution to change nesh size automaticly.

========================================================================

⚙️ bed_mesh Configuration (Important)

Due to PRTouch spiral probing, the mesh must meet these rules:
probe_count must be:

NxN
odd numbers only
Minimum 5×5

Recommended configuration
[bed_mesh]
speed: 100
mesh_min: 5,5
mesh_max: 295,295
probe_count: 5,5
mesh_pps: 2,2
algorithm: bicubic
bicubic_tension: 0.2
horizontal_move_z: 5

⚠️ 3×3 and even grids (4×4, 6×6) are not supported.

========================================================================

z_offset from orca

▶️ START_PRINT Usage for z offset config

The START_PRINT macro supports the following parameters:

Parameter	Description
Z_OFFSET	Runtime Z-offset (e.g. -0.04)

example:

START_PRINT EXTRUDER_TEMP=[nozzle_temperature_initial_layer] BED_TEMP=[bed_temperature_initial_layer_single] Z_OFFSET=-0.05
========================================================================



<img width="1914" height="813" alt="image" src="https://github.com/user-attachments/assets/a8494f2f-e087-4d02-a46c-0d414dd642e6" />

