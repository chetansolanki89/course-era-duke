# course-era-duke
Programming Foundations with JavaScript, HTML and CSS

Try experimenting with the DukeLearnToProgram (DLTP) JavaScript programming environment to get comfortable with beginning to write JavaScript!
Here is a link to the environment: http://www.dukelearntoprogram.com/course1/example/index.php

<b>Program 1:</b>
Write a JavaScript program that modifies an image by putting three vertical stripes on it - a red stripe on the left one third, a green stripe in the middle, and a blue stripe on the right one third.
For example, if your program ran on Drew’s picture shown on the left, the resulting image would have red, green and blue vertical stripes as shown in the image on the right.

Program 2:
Write a JavaScript function named swapRedGreen with one parameter pixel (representing a single pixel). This function should swap the red and green values of the pixel. For example, if you have a pixel with red = 255, green = 100, blue = 150, after calling swapRedGreen on that pixel its new RGB values would be red = 100, green = 255, blue = 150.

Program 3:
Write code to change the Duke blue devil (the image below on the left) to be yellow.

Program 4:
Write the green screen algorithm you saw in the lecture of the course.

Program 5:
Your friend is trying to write a program that draws a square 200 pixels by 200 pixels and that looks like this square with colors red (red value 255), green (green value 255), blue (blue value 255) and magenta (red value 255 and blue value 255). All other RGB values are set to 0.

Your friend has written code to try to solve this problem, however their code has a bug, and produces this image:

Here is their code:<br>
    &emsp;var img = new SimpleImage(200,200);<br>
    &emsp;for (var px of img.values()){<br>
    &emsp;&emsp;    var x = px.getX();<br>
    &emsp;&emsp;    var y = px.getY();<br>
    &emsp;&emsp;    if (x < img.getWidth()/2){<br>
    &emsp;&emsp;&emsp;        px.setRed(255);<br>
    &emsp;&emsp;    }<br>
    &emsp;&emsp;    if (y>img.getHeight()/2){<br>
    &emsp;&emsp;&emsp;        px.setBlue(255);<br>
    &emsp;&emsp;     }<br>
    &emsp;&emsp;     else {<br>
    &emsp;&emsp;&emsp;         px.setGreen(255);<br>
    &emsp;&emsp;     }<br>
    &emsp;}<br>
    &emsp;print (img);<br>
Your task is to find and fix the bug. Use what you have learned about applying the scientific method to debugging: gather information, apply your knowledge about images and programming, form a hypothesis, test your hypothesis, and finally, change the code to fix the problem.

Program 6:
Write a function named setBlack that has one parameter pixel (representing a single pixel) and returns pixel with its red, green, and blue components changed so that the pixel’s color is black.
Now you will write another function named addBorder. This function will add a black border to an image, such as in the following example:
![](images/)
On the left, we have the original image, and on the right, we have modified the image by giving it a black border that is 10 pixels thick. Note that the image size of the image with the border is the same as the original image because the border is not added around the outside of the original image, instead it covers up some of the original image

If you are struggling writing your for loop, review the For Loops video. The method values will be critical to writing your loop. Be sure to review the documentation to understand how this method works: http://www.dukelearntoprogram.com/course1/doc/
