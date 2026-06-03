# Walkthrough-in-a-Point-Cloud-in-Unity

This repository contains the source code and supporting scripts developed as part of a Master's thesis at KU Leuven (Geomatics). The research focuses on the real-time visualization of large point clouds in Unity and the creation of interactive walkthroughs through scanned environments.

## Application

The developed application allows users to:

* Load and visualize large point clouds at runtime using PLY files.
* Define walkthrough routes using control points and interpolation methods.
* Adjust visualization and navigation settings in real time.
* Generate smooth camera walkthroughs through scanned environments.
* Export walkthroughs as MP4 videos.

The complete application package, including the executable, supporting files, and example data used during the thesis, is available through the following download link:

https://kuleuven-my.sharepoint.com/:f:/g/personal/ruben_verlinden_student_kuleuven_be/IgA5mEUNPYgRT5TQ3cG-JkkwAf0-uL-XI_vsRxo0y2MiAdQ?e=46qz0F

## Repository contents

This repository contains both the code of the final application and a collection of scripts that were developed during the research process. Some of these scripts are used directly in the application, while others were created for benchmarking, testing, data preparation, or evaluating alternative point cloud visualization techniques. They are included for completeness and reproducibility of the thesis results.

### Main application scripts

* **RuntimePLYLoader.cs**
  Loads binary PLY point clouds at runtime and converts them into Unity data structures.

* **SmoothRoute.cs**
  Generates smooth camera movement along a user-defined walkthrough route.

* **TourBuilder.cs**
  Handles the user interaction, route creation, settings, and overall application workflow.

### Rendering scripts

* **PointCloudRenderer.cs**
  Responsible for rendering point cloud data inside Unity.

* **VoxelRenderer.cs**
  Experimental renderer used during the evaluation of alternative visualization methods.

### Benchmark scripts

* **BenchmarkSecondeVOORKEUR_1%.cs**
  Benchmarking script used to measure FPS performance and stability of the different visualization techniques evaluated in the thesis.

### Data preparation scripts

* **Converteer.ipynb**
  Jupyter Notebook used to transform georeferenced point clouds to a coordinate system suitable for Unity.

* **kolommen_filter.ipynb**
  Filters and preprocesses point cloud text files for compatibility with specific visualization methods.

## Thesis context

The scripts in this repository were developed during the research and implementation phases of the Master's thesis. Therefore, not every file is necessarily used in the final application. Several scripts were created to test, compare, and benchmark different point cloud visualization approaches within Unity.

## Author

**Ruben Verlinden**
Master of Science in Engineering Technology – Geomatics
KU Leuven
