# Seven Hole Probe Calibration

Full description with code, [here](https://github.com/arielya/SevenHoleProbe/blob/master/Seven_Hole_Probe_Calibration.ipynb)


This document explains, in practice, how to calibrate a seven-hole probe, and the general handling of different coordinate systems in a wind tunnel. The seven-hole probe is an application used to indicate the velocity vector in the current point of the probe. It gives as an output the velocity magnitude and two angles. From these results, the three components of the velocity vector can be estimated. The probe estimate is calculated through correlating the pressures and a polynomial. The polynomial coefficients should be found, or in other words, should be calibrated for the specific probe.

For the calibration, the probe gets as an input two angles in a certain reference system and three pressure coefficients. The pressure coefficient estimation is quite simple and will be discussed in the first part of this document. During the calibration process, the probe is set in a known angle relative to the upstream. The angle of the probe relative to the flow is set by two servo motors. The estimation of the angles is more complicated as it needs the angle to be in the probe reference system, which is not equal to the servo motor system angles. The transformation to the probe system depends on the servo motor system, and it will be explained for two different systems.

The seven-hole probe is a great example of the coordinate transformation between two different reference systems and to the global wind tunnel coordinate system. This document has been written in this format with the code, in order to explain not only the theory but also the practical applications.


Tags: aerodynamic, sensor, pitot, calibration, seven-hole, speed-sensor 
