# Introduction to Neural Networks

## Table of Contents

* [3.1 Introduction](#3.1-intorduction)
* [3.2 Classification Problems 1](#3.2-classification-problems-1)
* [3.3 Classification Problems 2](#3.3-classification-problems-2)
* [3.4 Linear Boundaries](#3.4-linear-boundaries)
* [3.5 Higher Dimensions](#3.5-higher-dimensions)
---

## 3.1 Introduction

* ### **What is Deep Learning?, What is it used for?**
    - #### Deep Learning is subfield of machine learning concerned with algorithms inspired by the structure and function of the brain called Artificail Neural Networks.
    - #### It has many applications such as:
        - beating Humans in games such as Go or jeopardy
        - Detecting spam in emails
        - forcasting stock prices
        - recognizig images in pictures
        - diagnosing illnesses sometimes with more percision than doctors
        - self-driving cars

<img src="imgs/5.png" align="right" width=150>

* ### **Neural Networks**
    - It vaguely mimic the process of how the brain operates, with neurons that fire bits of information.

## 3.2 Classification Problems 1

**When we have a system for acceptance of students at a university and most people who get 9 in test and 8 in grades more likely to get accepted but who get 3 in test and 4 in grades are more likely not to be accepted, so If we have a student who gets 7 in test and 6 in grades, will he be accepted or not?**

<p align="center">
    <img src="imgs/1.png" width=500>
</p>

## 3.3 Classification Problems 2

**we could say from the data above that the student will be accepted because he falls at the area of accepted students. We can clarify it more by setting a line which seperates the students who got accepted or not accepted like below**

<p align="center">
    <img src="imgs/6.png" width=500>
</p>

<br>

## 3.4 Linear Boundaries

<p align="center">
    <img src="imgs/7.png" width=500>
</p>

<img src="imgs/3.png" align="right" width=150>

<br>
<br>

**that line which has been drawn it has an equation <a href="https://www.codecogs.com/eqnedit.php?latex=2x_{1}&space;&plus;&space;x_{2}&space;-&space;18&space;=&space;0" target="_blank"><img src="https://latex.codecogs.com/png.latex?2x_{1}&space;&plus;&space;x_{2}&space;-&space;18&space;=&space;0" title="2x_{1} + x_{2} - 18 = 0" /></a> which mean to accept or reject a student we should see the equation result <a href="https://www.codecogs.com/eqnedit.php?latex=2*test&space;&plus;&space;grades&space;-&space;18&space;=&space;0" target="_blank"><img src="https://latex.codecogs.com/png.latex?2*test&space;&plus;&space;grades&space;-&space;18&space;=&space;0" title="2*test + grades - 18 = 0" /></a> and the result if it > 0 the student will be accepted and if it < 0 the student will be rejected**

<br>
<br>
<br>
<br>

<img src="imgs/4.png" align="right" width=150>

<br>
<br>

**In more general case the equation of the boundary line will be <a href="https://www.codecogs.com/eqnedit.php?latex=w_{1}x_{1}&space;&plus;&space;w_{2}x_{2}&space;&plus;&space;b&space;=&space;0" target="_blank"><img src="https://latex.codecogs.com/png.latex?w_{1}x_{1}&space;&plus;&space;w_{2}x_{2}&space;&plus;&space;b&space;=&space;0" title="w_{1}x_{1} + w_{2}x_{2} + b = 0" /></a> and to summarize it more, we will have <a href="https://www.codecogs.com/eqnedit.php?latex=WX&space;&plus;&space;b&space;=&space;0" target="_blank"><img src="https://latex.codecogs.com/png.latex?WX&space;&plus;&space;b&space;=&space;0" title="WX + b = 0" /></a> which <a href="https://www.codecogs.com/eqnedit.php?latex=W" target="_blank"><img src="https://latex.codecogs.com/png.latex?W" title="W" /></a> is a vector of <a href="https://www.codecogs.com/eqnedit.php?latex=w_{1},&space;w_{2}" target="_blank"><img src="https://latex.codecogs.com/png.latex?w_{1},&space;w_{2}" title="w_{1}, w_{2}" /></a> and <a href="https://www.codecogs.com/eqnedit.php?latex=X" target="_blank"><img src="https://latex.codecogs.com/png.latex?X" title="X" /></a> is a vector of <a href="https://www.codecogs.com/eqnedit.php?latex=x_{1},&space;x_{2}" target="_blank"><img src="https://latex.codecogs.com/png.latex?x_{1},&space;x_{2}" title="x_{1}, x_{2}" /></a> and  <a href="https://www.codecogs.com/eqnedit.php?latex=y" target="_blank"><img src="https://latex.codecogs.com/png.latex?y" title="y" /></a> is a label of 0 or 1. The prediction variable <a href="https://www.codecogs.com/eqnedit.php?latex=y\hat{}" target="_blank"><img src="https://latex.codecogs.com/png.latex?\hat{y}" title="y\hat{}" /></a> which will be 1 if <a href="https://www.codecogs.com/eqnedit.php?latex=WX&space;&plus;&space;b&space;\geq&space;0" target="_blank"><img src="https://latex.codecogs.com/png.latex?WX&space;&plus;&space;b&space;\geq&space;0" title="WX + b \geq 0" /></a> which will be above the line and will be 0 if <a href="https://www.codecogs.com/eqnedit.php?latex=WX&space;&plus;&space;b&space;<&space;0" target="_blank"><img src="https://latex.codecogs.com/png.latex?WX&space;&plus;&space;b&space;<&space;0" title="WX + b < 0" /></a> which will be below the line.**

<br>

## 3.5 Higher Dimensions

**If we have 3 columns instead of 2, we won't be working in 2 dimensions, we will be working in three dimensions**

<p align="center">
    <img src="imgs/8.png" width=500>
</p>

<img src="imgs/9.png" align="right" width=150>

<br>

**The Equation for that plane will be <a href="https://www.codecogs.com/eqnedit.php?latex=w_{1}x_{1}&space;&plus;&space;w_{2}x_{2}&space;&plus;&space;w_{3}x_{3}&space;&plus;&space;b&space;=&space;0" target="_blank"><img src="https://latex.codecogs.com/png.latex?w_{1}x_{1}&space;&plus;&space;w_{2}x_{2}&space;&plus;&space;w_{3}x_{3}&space;&plus;&space;b&space;=&space;0" title="w_{1}x_{1} + w_{2}x_{2} + w_{3}x_{3} + b = 0" /></a> but it still could be abreviated with <a href="https://www.codecogs.com/eqnedit.php?latex=WX&space;&plus;&space;b&space;=&space;0" target="_blank"><img src="https://latex.codecogs.com/png.latex?WX&space;&plus;&space;b&space;=&space;0" title="WX + b = 0" /></a> but instead the vector <a href="https://www.codecogs.com/eqnedit.php?latex=\vec{W}" target="_blank"><img src="https://latex.codecogs.com/png.latex?\vec{W}" title="\vec{W}" /></a> will include <a href="https://www.codecogs.com/eqnedit.php?latex=w_{1},&space;w_{2},&space;w_{3}" target="_blank"><img src="https://latex.codecogs.com/png.latex?w_{1},&space;w_{2},&space;w_{3}" title="w_{1}, w_{2}, w_{3}" /></a> and the vector <a href="https://www.codecogs.com/eqnedit.php?latex=\vec{X}" target="_blank"><img src="https://latex.codecogs.com/png.latex?\vec{X}" title="\vec{X}" /></a> will include <a href="https://www.codecogs.com/eqnedit.php?latex=x_{1},&space;x_{2},&space;x_{3}" target="_blank"><img src="https://latex.codecogs.com/png.latex?x_{1},&space;x_{2},&space;x_{3}" title="x_{1}, x_{2}, x_{3}" /></a> and the predction will still <a href="https://www.codecogs.com/eqnedit.php?latex=\hat{y}\begin{cases}&space;&&space;1&space;\text{&space;if&space;}&space;WX&space;&plus;&space;b&space;\geq&space;0&space;\\&space;&&space;0&space;\text{&space;if&space;}&space;WX&space;&plus;&space;b&space;<&space;0&space;\end{cases}" target="_blank"><img src="https://latex.codecogs.com/png.latex?\hat{y}\begin{cases}&space;&&space;1&space;\text{&space;if&space;}&space;WX&space;&plus;&space;b&space;\geq&space;0&space;\\&space;&&space;0&space;\text{&space;if&space;}&space;WX&space;&plus;&space;b&space;<&space;0&space;\end{cases}" title="\hat{y}\begin{cases} & 1 \text{ if } WX + b \geq 0 \\ & 0 \text{ if } WX + b < 0 \end{cases}" /></a>**

<br>

<img src="imgs/10.png" width=150 align="right">

**But what if we have n dimensional space <a href="https://www.codecogs.com/eqnedit.php?latex=x_{1},&space;x_{2},....,&space;x_{n}" target="_blank"><img src="https://latex.codecogs.com/png.latex?x_{1},&space;x_{2},....,&space;x_{n}" title="x_{1}, x_{2},...., x_{n}" /></a>, We will have n dimensional hyperplane and the equation will be <a href="https://www.codecogs.com/eqnedit.php?latex=w_{1}x_{1}&space;&plus;&space;w_{2}x_{2}&space;&plus;&space;w_{3}x_{3}&space;&plus;&space;b&space;=&space;0" target="_blank"><img src="https://latex.codecogs.com/png.latex?w_{1}x_{1}&space;&plus;&space;w_{2}x_{2}&space;&plus;&space;w_{n}x_{n}&space;&plus;&space;b&space;=&space;0" title="w_{1}x_{1} + w_{2}x_{2} + w_{n}x_{n} + b = 0" /></a> but it still could be abreviated with <a href="https://www.codecogs.com/eqnedit.php?latex=WX&space;&plus;&space;b&space;=&space;0" target="_blank"><img src="https://latex.codecogs.com/png.latex?WX&space;&plus;&space;b&space;=&space;0" title="WX + b = 0" /></a> but instead the vector <a href="https://www.codecogs.com/eqnedit.php?latex=\vec{W}" target="_blank"><img src="https://latex.codecogs.com/png.latex?\vec{W}" title="\vec{W}" /></a> will include <a href="https://www.codecogs.com/eqnedit.php?latex=w_{1},&space;w_{2},....,&space;w_{n}" target="_blank"><img src="https://latex.codecogs.com/png.latex?w_{1},&space;w_{2},....,&space;w_{n}" title="w_{1}, w_{2},...., w_{n}" /></a> and the vector <a href="https://www.codecogs.com/eqnedit.php?latex=\vec{X}" target="_blank"><img src="https://latex.codecogs.com/png.latex?\vec{X}" title="\vec{X}" /></a> will include <a href="https://www.codecogs.com/eqnedit.php?latex=x_{1},&space;x_{2},....,&space;x_{n}" target="_blank"><img src="https://latex.codecogs.com/png.latex?x_{1},&space;x_{2},....,&space;x_{n}" title="x_{1}, x_{2},...., x_{n}" /></a> and the predction will still <a href="https://www.codecogs.com/eqnedit.php?latex=\hat{y}\begin{cases}&space;&&space;1&space;\text{&space;if&space;}&space;WX&space;&plus;&space;b&space;\geq&space;0&space;\\&space;&&space;0&space;\text{&space;if&space;}&space;WX&space;&plus;&space;b&space;<&space;0&space;\end{cases}" target="_blank"><img src="https://latex.codecogs.com/png.latex?\hat{y}\begin{cases}&space;&&space;1&space;\text{&space;if&space;}&space;WX&space;&plus;&space;b&space;\geq&space;0&space;\\&space;&&space;0&space;\text{&space;if&space;}&space;WX&space;&plus;&space;b&space;<&space;0&space;\end{cases}" title="\hat{y}\begin{cases} & 1 \text{ if } WX + b \geq 0 \\ & 0 \text{ if } WX + b < 0 \end{cases}" /></a>**