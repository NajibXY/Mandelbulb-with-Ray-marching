# Experimenting-with-Mandelbulb

# C++ Game of Life Simulation with Raylib Library

## Author: [Najib El khadir](https://github.com/NajibXY)
## French Version //todo

## 1. Motivations

<img align="right" src="https://github.com/NajibXY/Game-Of-Life-using-CPP-and-Raylib/blob/master/gifs/main.gif">

Who doesn't love fractals ? </br>
As an exercice to learn more about the maths behind generating and displaying fractals. I worked on this example of Mandelbulb generation. Mandelbulb is a 3D fractal emerging from the experimentations to find a 3D canonical Mandelbrot set.

//todo
<img align="right" src="https://github.com/NajibXY/Game-Of-Life-using-CPP-and-Raylib/blob/master/gifs/main.gif">

</br> </br>

## 2. Technologies Used

- C++14, OpenMP
- Python, Conda, Numpy, Matplotlib

## 3. References



## 4. Implemented Features

- Grid randomization (Key R)
- Grid clearing (Key E)
- Acceleration and deceleration of simulation (Keys S, D & F)
- Pause/Resume simulation (Space Key)
- Play one step (Key G)
- Modify randomization rate (Keys K, L & J)  
![](https://github.com/NajibXY/Game-Of-Life-using-CPP-and-Raylib/blob/master/gifs/randomization.gif)

### Implemented Patterns and Oscillators

- It is also possible to manually activate and deactivate cells with mouse clicks.
  
- The following predefined patterns have been implemented (navigation for selecting shapes to draw is done with keys O & P):
  + The Dot (for customized shapes):  
      ![](https://github.com/NajibXY/Game-Of-Life-using-CPP-and-Raylib/blob/master/gifs/dot.gif)

  + The Glider: https://conwaylife.com/wiki/Glider  
      ![](https://github.com/NajibXY/Game-Of-Life-using-CPP-and-Raylib/blob/master/gifs/glider.gif)

  + The Blinker: https://conwaylife.com/wiki/Blinker  
      ![](https://github.com/NajibXY/Game-Of-Life-using-CPP-and-Raylib/blob/master/gifs/blinker.gif)

  + The Gosper Glider Gun: https://conwaylife.com/wiki/Gosper_glider_gun  
      ![](https://github.com/NajibXY/Game-Of-Life-using-CPP-and-Raylib/blob/master/gifs/glider-gun.gif)
    
  + The Pulsar: https://conwaylife.com/wiki/Pulsar  
      ![](https://github.com/NajibXY/Game-Of-Life-using-CPP-and-Raylib/blob/master/gifs/pulsar.gif)

## 5. Possible Improvements

- Customization of grid size
- Customization of initial grid with a seed file
- Memorization of steps and backward step-by-step playback
- Saving a run from initialization to stabilization
- Implementation of more oscillators and shapes
- Implementation of variations of the Game of Life (different rules, different dimensionality, and properties of space): https://conwaylife.com/wiki/Conway%27s_Game_of_Life#Variations_on_Life

## 6. Running the Project

- If you simply want to play with the simulation, you can download the .exe from the main repository: [game_of_life.exe](https://github.com/NajibXY/Game-Of-Life-using-CPP-and-Raylib/blob/master/game_of_life.exe)

## Compilation, Duplication, and Improvement of the Project
  
### Prerequisites

+ C++ installation (preferably 14)
+ Raylib for C++ installation: https://www.raylib.com/

### Steps

- Download or fork the project
- Open the project in VS Code via the main.code-workspace file
- Press F5 to compile and run
- From there, you can make any modifications you want to the project fork.
