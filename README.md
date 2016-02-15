# McStas_3DND

Alberto Cereser, 15 February 2016

These are the files I used to simulate a ToF 3DND experiment at beamline BL18, J-PARC, using [McStas](http://www.mcstas.org/). The BL18 setup is described by BL18_pxtal_BOTH.instr; to optimize the simulatiuon time, data can be separately collected using only the near-field or the far-field detectors (relative instrument files: BL18_pxtal_MCP.instr and BL18_pxtal_FF.instr). 

The J-PARC source is described by source_BL18.txt.

As a sample, we consider an Iron cylinder consisting of 20 regions with random orientation. default.map_101x101_rectified is a voxellized map of the sample, with the voxel orientations defined by default.orts. The reflections for Iron are listed by Fe.lau.

To save the output data using the same format of the detetcors at J-PARC, E. Knudsen developed the new modules FITS_monitor_new.comp and HDB_monitor_new.comp. 
