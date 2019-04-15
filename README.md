# ninjaCap Support

This repository provides information about the ninjaCap 3D-printed headcaps for fNIRS measurements, including instructions for providing probe designs and additional relevant information. If you have an issue or feature suggestion, [create a new issue](https://github.com/neuluce/ninjaCap-support/issues/new).

The 3D-printed headcaps are currently in a limited beta test, with probe holders for TechEn fibers. 

## Probe Configuration

To print a ninjaCap, you must provide NeuLuce with your probe configuration as an [AtlasViewer file](https://homer-fnirs.org/). The following instructions cover key steps in the process:

1. Register the atlas to the desired head size (under "Tools", select "Register Atlas to Head Size"). The head size will determine the size of the ninjaCap. The ninjaCap is flexible, and will be printed slightly smaller than the desired dimension to ensure consistent probe contact. See the table at the end of the document for scaling measurements.

   ![AtlasViewer: Register Atlas to Head Size](https://github.com/neuluce/ninjaCap-support/raw/master/av-head-size.png)

2. Add your probes and register them to the head surface. (Consult AtlasViewer documentation for more information on this process.)

3. Save your viewer state (under "File", select "Save Viewer State"). An "AtlasViewer.mat" file will be saved in the current working directory (usually the AtlasViewer directory or Atlas directory) containing all the information needed to print the cap.

   ![AtlasViewer: Save Viewer State](https://github.com/neuluce/ninjaCap-support/raw/master/av-save.png)

4. Send both the original probe file ("your-probe-design.SD") and the generated "AtlasViewer.mat" file to NeuLuce for printing.

## Scaling

When scaling, AtlasViewer requires providing two measurements in addition to the head circumference. If you only know the head circumference, use the table below to find recommended parameters for the corresponding Iz to Nz and RPA to LPA measurements.

| Head Circumference (cm) | Iz to Nz (cm) | RPA to LPA (cm) |
| ----------------------- | ------------- | --------------- |
| 50                      | 32.5          | 31.43           |
| 52                      | 33.8          | 32.68           |
| 54                      | 35.1          | 33.94           |
| 56                      | 36.4          | 35.2            |
| 58                      | 37.7          | 36.45           |
| 60                      | 39            | 37.71           |
| 62                      | 40.3          | 38.97           |
| 64                      | 41.6          | 40.23           |

