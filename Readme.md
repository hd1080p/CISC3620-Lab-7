# Lab 3: Animate a drawing

## Due date: Thurs. 2/23

As usual, 1 point extra credit will be awarded for completed assignment or pull request fixing error before Sat. 2/18

Extra credit will also be given for opening and especially answering issues on the original repository.

## Summary

The startup code for this lab applies a model transformation to a rectangle. Change the code to apply a model transformation made of a scale, translation, and rotation concatenated together in an appropriate order, which is continuously applied with changing parameters to create an animation.

## Getting started

Same as [last time](https://cisc3620.github.io/docs/submissions.html). 

1. Clone this repository to make a local copy on your machine.

2. Run cmake from the Build directory to generate a project file for your platform.

3. Compile and run.
   You should see a red triangle on a pink background.

## Modify

Open main.cpp for editing. 

* The model transformation matrix currently only scales the triangle; modify it to consist of a scale, rotation, and translation concatenated together.

* The model transformation matrix is currently sent to the shader on line 123. Move the command to inside the rendering loop so it will be updated on each draw.

* Also inside the rendering loop, modify the matrix to create an animation.

   * *The animation should not end* -- the shape should not translate off the screen, or grow beyond the size of the screen, or shrink into invisibility.

* You may want to modify the vertices to draw your shape from lab 2 or another more interesting shape. (*This is not required*)

## Submit

[Same as last time.](https://cisc3620.github.io/docs/submissions.html)

**In addition**, execute the program, save a clip of the animation that's created (using a screen recording tool such as Quicktime or CamStudio), and move the video into the top level of your repository.

Your add command will be (depending on your clip format)

```git add main.cpp animation.mp3```

I will look at the code you've changed in main and your generated animation.
