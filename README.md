﻿# Experimenting-with-Mandelbulb

# C++ & Python Mandelbulb generation and rendering

## Author: [Najib El khadir](https://github.com/NajibXY)
## French Version //todo

## 1. Motivations

<img align="right" src="https://github.com/NajibXY/Mandelbulb-with-Ray-marching/blob/master/mandelbulb.gif">

Who doesn't love fractals ? </br>
As an exercice to learn more about the maths behind generating and rendering fractals. I worked on this example of Mandelbulb generation. Mandelbulb is a 3D fractal emerging from the experimentations to find a 3D canonical Mandelbrot set.
<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/2/21/Mandel_zoom_00_mandelbrot_set.jpg">
  <em>Mandelbrot set</em>
</p>

</br> </br>

## 2. Technologies Used

- C++14, OpenMP
- Python, Numpy, Matplotlib, FFMPEG, Conda (for my personal environment)

## 3. References

- [Distance Estimated 3D Fractals](http://blog.hvidtfeldts.net/index.php/2011/06/distance-estimated-3d-fractals-part-i/)
- [Understanding the View Matrix](https://www.3dgep.com/understanding-the-view-matrix/)
- [The Coding train's Mandelbulb Challenge](https://www.youtube.com/watch?v=NJCiUVGiNyA&ab_channel=TheCodingTrain)

## 4. Data generation

- The data points of the mandelbulb are pretty easy to generate, even thought it required to do some parallelisation with OpenMP in order to achieve a good enough execution time.
- But in order to be able to render the data, a ray marching method has been implemented, that involves lights and distances calculation, according to the movement of the camera, and requires to do some parallelization with OpenMP and a lot of 3D vector maths to achieve an acceptable execution time.
- It takes about 30 minutes to generate the data with an base exponent equal to 8.

### Compilating the generate_data.cpp file

- Requires C++ and G++ installed.
- Just run : g++ -Wall -Wextra -fopenmp generate_data.cpp -o generate_data.exe
- Running the .exe will generate the data in the /data/ folder.

## 5. Displaying the rendering data

### Set up your environment

- You'll need to set up a Python environment (in my case conda), to display the generated data with Matplotlib.
- For installing the requirements with conda you can just run : conda create --name <env> --file <this file>
- Or pip install -r requirements.txt if you use pip
- Then you will be able to run the 

### Run the python script

- python .\generate_video.py
</br>
- This will provide you with all the rendered PNGs of the data previously generated. Those are saved in the /images/ folder
- After generating the images, the script also generates a video compilating the results using FFMPEG in the same folder as the script.
<img align="left" src="https://github.com/NajibXY/Mandelbulb-with-Ray-marching/blob/master/example1.png">
<img align="right" src="https://github.com/NajibXY/Mandelbulb-with-Ray-marching/blob/master/example2.png">

## 5. Possible Improvements

- Faster data generation
- Using other formulas for the data generation
- Using other methods for rendering
- Using a C++ efficient library to generate the vizualisation along the data.
- Being able to tune the generation parameters.

