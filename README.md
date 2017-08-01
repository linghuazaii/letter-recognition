# Letter Recognition

### Features
These features are mentioned in [[resource/letter-recognition.pdf]](https://github.com/linghuazaii/letter-recognition/blob/master/resource/letter-recognition.pdf)  
The image rectangle is called `Box` and the smallest rectangle containing the letter is called `Rectangle` in the context. Pixels on black part of the Rectangle is marked as on, marked as off for the white part. Center point of the axes is the center of the Rectangle named as Center in the context.  
 - horizontal position (integer):  pixels from left of the Box to the center of the Rectangle.  
 - vertical position (integer): pixels from bottom of the Box to the center of the Rectangle.  
 - width (integer): in pixels, width of the Rectangle  
 - height (integer): in pixels, height of the Rectangle  
 - number of pixels(integer): total number of on pixels marked as on in the Rectangle
 - mean x of all on pixels (float): mean of horizontal position of all on pixels relative to the Center diveded by the width of the Rectangle. If this value is negative, the image is "left-heavy" as would be the case for the letter **L**  
 - mean y of all on pixels (float): mean of vertical position of all on pixels relative to the Center divided by the height. If this value is negative, the image is "bottom-heavy" as would be the case for the letter **G**, **Q**, etc.  
 - mean squared value of x (float): like mean x of all on pixels, but the distance is squared. If this value is large, the letter would be **W**, **M**, etc.  
 - mean squared value of y (float): like mean y of all on pixels, but the distance is squared.
 - mean x * y (float): mean of horizontal mutiply vertical position.
 - mean x^2 * y^2 (float): mean of horizontal squar times vertical squar.
 - mean number of edge from left to right (float): scan from left to right, edge here is left boundary or right boundary. calculate each vertically and the calculate the mean.
 - sum of y of edge above (integer): sum of vertical position for all edges measured above.
 - mean number of edge from bottom to top (float): scan from bottom to top, edge here is top boundary or bottom boundary. calculate the mean.
 - sum of x of edge above (integer): sum of horizontal positions for all edges measured above.
