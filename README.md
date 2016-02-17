# McStas_3DND

Alberto Cereser, 15 February 2016

In this repository you can find the files I used to simulate a ToF 3DND experiment at beamline BL18, J-PARC, using [McStas](http://www.mcstas.org/). The BL18 setup is described by [`BL18_pxtal_BOTH.instr`](https://github.com/albusdemens/McStas_3DND/blob/master/BL18_pxtal_BOTH.instr); to speed up the computational time, the simulation can be performed with only the near- or the far-field detectors mounted (relative instrument files: [`BL18_pxtal_MCP.instr`](https://github.com/albusdemens/McStas_3DND/blob/master/BL18_pxtal_MCP.instr) and [`BL18_pxtal_FF.instr`](https://github.com/albusdemens/McStas_3DND/blob/master/BL18_pxtal_FF.instr)). To improve the code readibility, the description of the far-field detectors is in a separate file, [`detector_arms.instr`](https://github.com/albusdemens/McStas_3DND/blob/master/detector_arms.instr).

The J-PARC source is described by [`source_BL18.txt`](https://github.com/albusdemens/McStas_3DND/blob/master/source_BL18.txt).

As a sample, we consider an Iron cylinder consisting of 20 regions with random orientation. [`default.map_101x101_rectified`](https://github.com/albusdemens/McStas_3DND/blob/master/default.map_101x101_rectified) is a voxellized map of the sample, with the voxel orientations defined by [`default.orts`](https://github.com/albusdemens/McStas_3DND/blob/master/default.orts). The reflections for Iron are listed in [`Fe.lau`](https://github.com/albusdemens/McStas_3DND/blob/master/Fe.lau).

To save the output data using the same format of the detetcors at J-PARC, E. Knudsen developed the new modules [`FITS_monitor_new.comp`](https://github.com/albusdemens/McStas_3DND/blob/master/FITS_monitor_new.comp) and [`HDB_monitor_new.comp`](https://github.com/albusdemens/McStas_3DND/blob/master/HDB_monitor_new.comp). 
