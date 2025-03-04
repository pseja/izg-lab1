# Color Space Reduction

Author: Lukáš Pšeja

xlogin: xpsejal00

## Assignment
1. Convert a color image to grayscale (0.5 points)
2. Convert to black-and-white using thresholding (0.75 points)
3. Convert to black-and-white using random modulation thresholding or any order-based dithering method (0.5 points)
4. Convert to black-and-white using error diffusion or the Floyd-Steinberg algorithm (0.75 points)
5. Convert to black-and-white using tone-dependent error diffusion (0.5 points)

## Setup
To compile this application, you'll need GCC 7.0.0+ and CMake 3.12.0+.
With Ubuntu, you'll also need to install [libsdl2](https://packages.ubuntu.com/en/source/focal/libsdl2).

```sh
git clone git@github.com:pseja/izg-lab1.git
git submodule update --init --recursive
mkdir build
cd build/
cmake ..
make
./izg_lab_01
```

## Usage
| **Key/Button**   | **Action**                                                                                                                     |
|------------------|--------------------------------------------------------------------------------------------------------------------------------|
| Left Mouse Click | Prints the value of the selected pixel to the console.                                                                         |
| L                | Loads a test gradient image.                                                                                                   |
| K                | Loads a test image of an automobile.                                                                                           |
| S                | Saves the current window as a BMP file in `/data/out.bmp`.                                                                     |
| G                | Converts the image to grayscale.                                                                                               |
| R                | Converts the image to black-and-white using random dithering algorithm.                                                        |
| T                | Converts the image to black-and-white using thresholding.                                                                      |
| M, B, C          | Converts the image to black-and-white using random modulation, ordered Bayer dithering, or clustered-dot dithering algorithms. |
| E, F             | Converts the image to black-and-white using error diffusion or Floyd-Steinberg algorithm.                                      |
| W                | Converts the image to black-and-white using tone-dependent error diffusion.                                                    |
