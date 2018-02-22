# Magnetometer-calibration
Mag calibration and 3d point cloud visualisation
This code is for simplification whole process of magnitometer calibration.
1. Parser data from txt file. String data is ignored, so data could be in format like "x=.., y=.., z=..".
Lines which are not contains measurements ignored.
2. Point cloud visualization together with ideal sphere.
3. Axis non-orthogonality fixing and visualization.
4. Ellipsoid to sphere compression matrix and displacement vector calculation. Visualization of calibrated data as well.
5. Constructing of end user c-code lines like:
  xcal = a11*x+a12*y+a13*z
            ...
  zcal =    ...      a33*z
