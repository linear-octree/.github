# linear-octree

This organization hosts tools for processing and classifying LiDAR point cloud data using linear octree data structures.

## Repositories

### octree-mpi

A C++ implementation of a rule-based classifier for LiDAR point cloud data. It processes `.las` files and automatically classifies points into ground, vegetation, and building categories. The implementation relies on linear octree structures for spatial indexing and uses MPI to enable parallel execution across multiple processors.

Dependencies: Eigen, Armadillo, LASlib.

Build system: Make and CMake.

Original project: https://gitlab.citius.usc.es/lidar/rule-based-classifier

### laslib

A lightweight C++ library for reading and writing LAS files, including format version 1.4, which is not supported by the original liblas. It provides a `LASReader` class for loading point cloud headers and points from a file, and a `LASWriter` class for serializing point clouds back to disk.

Build system: CMake.
