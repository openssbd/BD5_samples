Copyright (C) 2020 RIKEN

## Sample codes and tools for reading and writing BD5 file format
* This repository contains the sample source codes for reading and writing BD5 file formats using Python in Juypter notebook.
* The samples include codes using either the h5py or pytables packages.

## Sample codes in Juypter notebook:

### Sample codes writing BD5 object entities:
![BD5 object entities](BD5numpy_examples.png?raw=true)

* Writing out object entities, line, point, circle, sphere and face.
    * [BD5write_numpy](BD5write_numpy.ipynb) (uses h5py) with explanation
        * Writing line, face, sphere, point and circle objects as numpy array to BD5 files.
    * [BD5write_circle_details](BD5write_circle_details.ipynb) (uses pytables) with explanation
    * [BD5write_circle](BD5write_circle.ipynb) (uses pytables)
        * Reading in an image segmentation data stored in a TIFF image file, and write it as a circle in BD5 format. 
    * [BD5write_point](BD5write_point.ipynb) (uses pytables)
        * Reading in an image segmentation data stored in a TIFF image file, and write it as a point in BD5 format. 
    * [BD5write_line](BD5write_line.ipynb) (uses pytables)
        * Reading in an image segmentation data stored in a TIFF image file, and write it as a line in BD5 format. 

### Sample codes writing BD5 files using h5py
* [CSVread_BD5write](CSVread_BD5write.ipynb) (uses h5py) with explanation
    * Reading in a BD5 file and writing out a CSV file/Reading in CSV file and writing out a BD5 file     
* [BD5write_numpy](BD5write_numpy.ipynb) (uses h5py)
    * Writing line, face, sphere, point and circle numpy arrays to BD5 files
* [BD5append_trackinfo_point](BD5append_trackinfo_point.ipynb) (uses h5py) with explanation
    * Reading in a BD5 file with time series information. It tries to calculate and track the objects over two time points and then append the trackInfo information to a BD5 file. 
* [BD5read_count](BD5read_count.ipynb) (uses h5py)
    * Reading in an existing BD5 file and do some simple analysis by counting the number of nucleus vs time point and ploting out a prolification curve of C.elegans.
### Sample codes writing BD5 files using pytables
* [BD5write_circle_details](BD5write_circle_details.ipynb) (uses pytables) with explanation
* [BD5write_circle](BD5write_circle.ipynb) (uses pytables)
    * Reading in an image segmentation data stored in a TIFF image file, and write it as a circle in BD5 format.
* [BD5write_point](BD5write_point.ipynb) (uses pytables)
    * Reading in an image segmentation data stored in a TIFF image file, and write it as a point in BD5 format.
* [BD5write_line](BD5write_line.ipynb) (uses pytables)
    * Reading in an image segmentation data stored in a TIFF image file, and write it as a line in BD5 format.
* [BD5write_timeseries_point](BD5write_timeseries_point.ipynb) (uses pytables) with explanation 
    * Reading in two time series ROIs data stored in TIFF image files, and track the objects over the two time points and write that to a BD5 file. 

## BD5 manual
Detailed description can be found on the link below.
http://ssbd.qbic.riken.jp/bdml/bd5.html

## Reference
BD5: an open HDF5-based data format to represent quantitative biological dynamics data
Koji Kyoda, Kenneth H. L. Ho, Yukako Tohsato, Hiroya Itoga, Shuichi Onami
bioRxiv 2020.04.26.062976; doi: https://doi.org/10.1101/2020.04.26.062976
