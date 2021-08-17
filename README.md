# Shoreline Detection

**Author:** Anna Spinosa

Contacts

Anna Spinosa (anna.spinosa@deltares.nl)

# Contents

(i) Required Python Packages

(ii) Input files

(iii) How to run the code

(iv) Outputs

(v) Publications

# (i) Required Python packages

(a) numpy

(b) scipy

(c) cv2

(d) gdal

(e) matplotlib

# (ii) Input files

The code accepts tiff files. To visualize tiff files please consider the software qGIS, a free and open source geographic information system (https://www.qgis.org/en/site/). In case of large files, please also consider to clip the raster with vector boundaries of the area of interest.

# (iii) How to run shoreline_detection.py

* python3 run_shoreline_detection.py

Inputs in the configs/sample_config.json:

(a) path_to_data: path to the dataset

(b) output_directory: name of the output directory to be created

(c) output_name_tif: name of the tif output file

(d) k: number of the neighborhors defining the size of the kernel implemented to reduce the speckling effect due to the constructive/destructive interferences of backscattered electromagnetic waves, and appearing as a salt–pepper noise in the image. The default size is 5.

# (iv) Outputs

Outputs are saved in a "outputs" folder. The folder "outputs" will contain a tiff file. The folder "outputs" will contain 2 subfolders:

(a) image

Here you will find

* shoreline.png

the resulting image.

(b) image geolocalized

Here you will find

* output_name_tif.tif

containing the geolocalized shoreline. Coordinates are taken from the input image.

Note: as the files.tif are > 25MB, we couldn't upload them in this github repository.

# (v) Publications

Spinosa, Anna, Alex Ziemba, Alessandra Saponieri, Leonardo Damiani, and Ghada El Serafy. "Remote sensing-based automatic detection of shoreline position: A case study in apulia region." Journal of Marine Science and Engineering 9, no. 6 (2021): 575.

Spinosa, Anna, Alex Ziemba, Alessandra Saponieri, Victor D. Navarro-Sanchez, Leonardo Damiani, and Ghada El Serafy. "Automatic Extraction of Shoreline from satellite images: a new approach." In 2018 IEEE International Workshop on Metrology for the Sea; Learning to Measure Sea Health Parameters (MetroSea), pp. 33-38. IEEE, 2018.
