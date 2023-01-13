<img src="https://user-images.githubusercontent.com/72500344/210864557-4078754f-86c1-4e7c-b291-73223bdf4e4d.png" alt="logo" width="200"/>

# Optimized reconstruction of large-scale 3D building models 

*Command-Line Interface (CLI) application for efficient and optimized reconstruction of large-scale 3D building models using GeoFlow.*

GeoFlow is a software tool that can be used to automatically reconstruct 3D building models from point clouds, with a high level of detail. It is a powerful tool for creating detailed and accurate 3D models of buildings and can be used in a variety of applications. The software is fully automated, making it easy to use and efficient for large-scale projects.

Our program is based on GeoFlow and makes use of it to perform 3D reconstruction of buildings. The process is inspired by the 3D BAG project, which is an up-to-date dataset containing detailed 3D building models of the Netherlands, based on the official BAG data and national AHN point cloud. The optimization of the reconstruction process is achieved by indexing and tiling of the input data which reduces the processing time and resources needed to generate large-scale 3D building models. The indexing and tiling of both, 3D point cloud and 2D footprints, allows for more efficient processing and handling of the 3D reconstruction workflow.

<img src="https://user-images.githubusercontent.com/72500344/212364590-b7fd444d-ec26-4a8b-bda9-fd4e1669bc6e.png" alt="Workflow of 3D Reconstruction" width="500"/>

## Installation

The easiest way to install <code>Optim3D</code> on Windows is to use the binary package on the [Release page](). In case you can not use the Windows installer, or if you are using a different operating system, you can build everything from source.

**NOTE:** It is important to note that in order to use our program for 3D reconstruction of buildings, GeoFlow-bundle must be installed. It is a necessary requirement for the program to function properly and perform the 3D reconstruction.

## Usage of the CLI
After installation, you have a small program called <code>optim3d</code>. Use <code>optim3d --help</code> to see the detailed help:

```
  
```
## Supported CityJSON versions

The application expects that your file is using the latest version [CityJSON schema](https://www.cityjson.org/specs/1.1.3/). If your file uses an earlier version, you can upgrade it with the upgrade operator of [cjio, CityJSON/io](https://github.com/cityjson/cjio): <code>cjio old.json upgrade save newfile.city.json</code>

Alternatively, any CityGML file can be automatically converted to CityJSON with the open-source project [citygml-tools](https://github.com/citygml4j/citygml-tools).

## About Optim3D

This software was developped by Anass Yarroudh, a Research Engineer in the [Geomatics Unit of the University of Liege](http://geomatics.ulg.ac.be/fr/home.php).

For more detailed information please contact us via <ayarroudh@uliege.be>, we are pleased to send you the necessary information.
