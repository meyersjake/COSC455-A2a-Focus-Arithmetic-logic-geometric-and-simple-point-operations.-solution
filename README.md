# COSC455-A2a-Focus-Arithmetic-logic-geometric-and-simple-point-operations.-solution

Download Here: [COSC455 A2a Focus: Arithmetic/logic, geometric, and simple point operations. solution](https://jarviscodinghub.com/assignment/a2a-focus-arithmetic-logic-geometric-and-simple-point-operations-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

For all questions, you need to include code to check whether the input image is grayscale. If it is not,
convert it first to grayscale then process it as required in each question.
1. [5 points] Write a Matlab function that corrects the brightness of a given image. The function should
take as arguments an image, a number between 0 and 100 (amount of brightness correction,
expressed in percentage terms), and a third parameter indicating whether the correction is intended
to brighten or darken the image. It should return a corrected grayscale image. [adapted from the
suggested textbook by Marques Q6.11]
2. [10 points] Many photo editors provide tools is to fix perspective errors when photographing large
buildings, e.g. the building in the left image below. PhotoShop for example provides this tool under
the name “Perspective Wrap” (e.g. see here). For this assignment, you need to (a) briefly explain the
science behind these tools, and (b) write a Matlab program that fixes the perspective of any given
image. Use ‘prespectiveCorrect.jpg’ for testing. The result should be similar to the right image below.
Your Matlab program should do the following:
 The program starts by displaying an image to the user using imshow.
 It then reads the (x,y) of four mouse clicks on the input image (use ginput). For simplicity,
assume the user must do the clicks in the order shown below. The image should be geometrically
transformed so that the four points form a rectangle in output image (i.e.points (1),(2) are aligned
horizontally, points (1),(3) vertically, points (2),(4) vertically, and points (3),(4) horizontally).
 Every time the user clicks a point, a small rectangle is drawn on the image to remind the user of
the position of that point (e.g. see the small red rectangles in the image below).
Marking guide:
+2 for theoretical explanation
+1 for showing the image and
reading the points
+4 for fixing the perspective
+1 for drawing the little
squares
+2 for simplicity and logical
correctness.
3. [8 points] You learned different transformation functions that map input intensities r to output
intensities s. The example below shows the mapping of a narrow range of dark pixels [r1,r2] to a
much wider range of intensities, improving the contrast of the input pixels.
Write a Matlab function intensityStretch that changes the contrast of a given image based the
linear mapping function shown below.
Your function should takes five arguments: the input image, two values for the input range of
intensities [r1,r2], and two values for the output range [s1,s2]. The function must check the input
intensity values and ensure that:
 r1 ≥ min intensity of I.
 r2 ≤ max intensity of I.
 s1 ≥ 0.
 s2 ≤ 255
Test your function with the code below. The output should be similar to the following images.
I = imread(‘baby_faceHiddent.png’);
I2 = intensityStretch(I,2,50,2,200);
imshow(I), figure, imshow(I2);
Marking guide:
+2 for validating the
input
+4 for the mapping
function
+2 for logical flow
and correctness
Submission Instructions
For each question, write a separate Matlab program or function. If you are required to explain
things, write your answer as a comment in your Matlab code. Submit everything as one zip file to
Blackboard Connect. Note that you can resubmit an assignment, but the new submission
overwrites the old submission and receives a new timestamp.
Input intensity level, r
Output intensity level, s
255
255
0
r1 r2
s1 s2



