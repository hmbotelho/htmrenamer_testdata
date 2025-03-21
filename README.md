# htmrenamer: test data
*Raw and renamed high-throughput microscopy datasets for the [htmrenamer](https://github.com/hmbotelho/htmrenamer) R package.*





## Table of Contents
* [1. Overview](#overview)
* [2. Leica datasets](#leica)
    * [2.1. Leica MatrixScreener software](#leica-matrixscreener)
    * [2.2. Leica Navigator software](#leica-navigator)
* [3. Zeiss datasets](#zeiss)
* [3. Olympus datasets](#olympus)





## <a name="overview">1. Overview</a>

This repository contains high-throughput mircroscopy datasets acquired with different microscope systems. Each dataset contains the following:  

1. A collection of `TIFF` or `OME-TIFF` images exported by the microscope controller software; 
2. A text [microscope infile](https://github.com/hmbotelho/htmrenamer/blob/master/README.md#3-generating-well-descriptors) which describes the well contents; 
3. Raw images renamed with the [htmrenamer](https://github.com/hmbotelho/htmrenamer) package without file compression; 
4. Raw images renamed with the [htmrenamer](https://github.com/hmbotelho/htmrenamer) package with lossless file (deflate). 

Images are provided as individual files or `zip` archives.  
These datasets are used to perform [unit testing](https://github.com/hmbotelho/htmrenamer/tree/master/tests/testthat) on the [htmrenamer](https://github.com/hmbotelho/htmrenamer) R package.





## <a name="leica">2. Leica datasets</a>


### <a name="leica-matrixscreener">2.1. MatrixScreener software</a>

| #                                              | Microscope | Software version   | Carrier type           | Size (MB) | Images per carrier | Wells | Subpositions (P) | Time points (T) | Slices (Z) | Channels (C) |
|------------------------------------------------|:----------:|:------------------:|:----------------------:|:---------:|:------------------:|:-----:|:----------------:|:---------------:|:----------:|:------------:|
| **[01](./leica_matrixscreener/01_DMI6000_PC)** | DMI 6000B  | LAS-AF 1.1.0.12420 | 96 well plate (8×12)   | 22.7      | 108                | 4     | 9                | 1               | 1          | 3            |
| **[02](./leica_matrixscreener/02_DMI6000_PC)** | DMI 6000B  | LAS X 3.1.0.15537  | 384 well plate (16×24) | 53.9      | 288                | 24    | 4                | 1               | 1          | 3            |
| **[03](./leica_matrixscreener/03_DMI6000_TC)** | DMI 6000B  | LAS-AF 1.1.0.12420 | 96 well plate (8×12)   | 59.4      | 368                | 8     | 1                | 23              | 1          | 2            |
| **[04](./leica_matrixscreener/04_DMI6000_TC)** | DMI 6000B  | LAS X 3.1.0.15537  | 96 well plate (8×12)   | 13.8      | 98                 | 7     | 1                | 7               | 1          | 2            |
| **[05](./leica_matrixscreener/05_DMI6000_TC)** | DMI 6000B  | LAS X 3.1.0.15537  | 96 well plate (8×12)   | 19.3      | 140                | 10    | 1                | 7               | 1          | 2            |
| **[06](./leica_matrixscreener/06_SP8_TC)**     | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 22.3      | 126                | 9     | 1                | 7               | 1          | 2            |
| **[07](./leica_matrixscreener/07_SP8_TC)**     | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 57.8      | 336                | 24    | 1                | 7               | 1          | 2            |


### <a name="leica-navigator">2.2. Navigator software</a>

| #                                                 | Microscope | Software version   | Carrier type           | Size (MB) | Images per carrier | Wells | Subpositions (P) | Time points (T) | Slices (Z) | Channels (C) | Export options                     |
|---------------------------------------------------|:----------:|:------------------:|:----------------------:|:---------:|:------------------:|:-----:|:----------------:|:---------------:|:----------:|:------------:|------------------------------------|
| **[01](./leica_navigator/01_PZC)**                | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 2.2       | 40                 | 1     | 4                | 1               | 5          | 2            | None                               |
| **[02](./leica_navigator/02_PTZC)**               | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 543       | 11520              | 96    | 4                | 3               | 5          | 2            | None                               |
| **[03](./leica_navigator/03_PZC)**                | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 72.8      | 320                | 8     | 4                | 1               | 5          | 2            | None                               |
| **[04](./leica_navigator/04_ZC)**                 | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 55.2      | 960                | 96    | 1                | 1               | 5          | 2            | None                               |
| **[05](./leica_navigator/05_C)**                  | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 22.7      | 192                | 96    | 1                | 1               | 1          | 2            | None                               |
| **[06](./leica_navigator/06_TZC)**                | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 135       | 2880               | 96    | 1                | 3               | 5          | 2            | None                               |
| **[07](./leica_navigator/07_TC)**                 | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 38.9      | 576                | 96    | 1                | 3               | 1          | 2            | None                               |
| **[08](./leica_navigator/08_nothing)**            | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 2.2       | 40                 | 1     | 4                | 1               | 5          | 2            | None                               |
| **[09](./leica_navigator/09_overl)**              | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 1.67      | 20                 | 1     | 4                | 1               | 5          | 2            | Overlay                            |
| **[10](./leica_navigator/10_comp)**               | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 1.64      | 40                 | 1     | 4                | 1               | 5          | 2            | Compress                           |
| **[11](./leica_navigator/11_comp_overl)**         | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 1.53      | 20                 | 1     | 4                | 1               | 5          | 2            | Compress + Overlay                 |
| **[12](./leica_navigator/12_dir)**                | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 2.21      | 40                 | 1     | 4                | 1               | 5          | 2            | Folders                            |
| **[13](./leica_navigator/13_dir_comp)**           | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 1.66      | 40                 | 1     | 4                | 1               | 5          | 2            | Folders + Compress                 |
| **[14](./leica_navigator/14_dir_comp_overl)**     | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 1.55      | 20                 | 1     | 4                | 1               | 5          | 2            | Folders + Compress + Overlay       |
| **[15](./leica_navigator/15_raw)**                | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 1.42      | 40                 | 1     | 4                | 1               | 5          | 2            | Raw                                |
| **[16](./leica_navigator/16_raw_dir)**            | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 1.44      | 40                 | 1     | 4                | 1               | 5          | 3            | Raw + Folders                      |
| **[17](./leica_navigator/17_raw_dir_overl)**      | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 1.69      | 20                 | 1     | 4                | 1               | 5          | 2            | Raw + Folders + Overlay            |
| **[18](./leica_navigator/18_raw_dir_comp)**       | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 1.38      | 40                 | 1     | 4                | 1               | 5          | 2            | Raw + Folders + Compress           |
| **[19](./leica_navigator/19_raw_dir_overl_comp)** | SP8        | LAS X 3.5.5.19976  | 96 well plate (8×12)   | 1.55      | 20                 | 1     | 4                | 1               | 5          | 2            | Raw + Folders + Overlay + Compress |





## <a name="zeiss">3. Zeiss datasets</a>
| #                      | Microscope   | Software version            | Carrier type           | Size (MB) | Images per carrier | Wells | Subpositions (P) | Time points (T) | Slices (Z) | Channels (C) |
|------------------------|:------------:|:---------------------------:|:----------------------:|:---------:|:------------------:|:-----:|:----------------:|:---------------:|:----------:|:------------:|
| **[01](./zeiss/01_T)** | Zeiss LSM800 | ZEN 2.5 Lite (blue edition) | 96 well plate (8×12)   | 16.7      | 21                 | 3     | 1                | 7               | 1          | 1            |





## <a name="olympus">3. Olympus datasets</a>
| #                         | Microscope     | Software version            | Carrier type           | Size (MB) | Images per carrier | Wells | Subpositions (P) | Time points (T) | Slices (Z) | Channels (C) |
|---------------------------|:--------------:|:---------------------------:|:----------------------:|:---------:|:------------------:|:-----:|:----------------:|:---------------:|:----------:|:------------:|
| **[01](./olympus/01_TC)** | Olympus FV1000 |                             | 96 well plate (8×12)   | 49.3      | 18                 | 2     | 1                | 9               | 1          | 2            |
