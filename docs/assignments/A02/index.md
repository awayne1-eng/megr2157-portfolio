# A2 – Truss Stress Analysis

## Objective
For this assignment, I was asked to create a 3D truss with specific given requirements/constraints. This image was what the requirements/constraints consist of.
![image alt](https://github.com/awayne1-eng/megr2157-portfolio/blob/232e4556cc62db65a405d64fb7881e212720c3ce/IMG_0948.jpeg)

In the image layout of the soon to be truss, I am given that point A is a pin and point B is a roller. I am also given the lengths of both a and b, where a=0.4m and b=0.3m. I was also able to choose the value of the external forces. ranging anywhere from 20-30kN. I ended up choosing 24kN for this assignment. I need to design a lightweight truss, containing A500 steel, or something of similar relevance.
![image alt](https://github.com/awayne1-eng/megr2157-portfolio/blob/e0b9a8b0bd65b205871df8e1eedbb6b03e06afaf/IMG_0949.jpeg)

Since one of the main objectives is to make the truss lightweight, I want to try and minimize the number of beams connected to the truss. But I still need to ensure that the number of beams will be enough to support the truss, or it will not sustain itself. I ended up deciding that the best way to figure how to maximize the truss's full potential would be to use triangular geometry shape within the truss.
![image alt](https://github.com/awayne1-eng/megr2157-portfolio/blob/c463b8084c5134678a4cde1de6602b1f07f57cbf/IMG_0950.jpeg)

For this next step, I calculated the external reaction forces at supports A and B by applying the static equilibrium equations to the entire truss under my selected load of P=24kN. Determining these support reactions is a mandatory prerequisite because it balances the entire structure externally before you can move on to solve for the internal members at each joint. To end up solving this, I first summed up the moments of pin A to isolate and solve for the vertical reaction at roller B. I then applied the global force balance equations to determine the remaining reactions at pin A.
![image alt](https://github.com/awayne1-eng/megr2157-portfolio/blob/671c60ab0778c87944d42d64b3f2f2eb963251a5/IMG_0951.jpeg)

So, now I was able to establish a detailed sketch of my truss, containing joints A-F. The truss layout also defines the geometric lengths and trigonometric ratios for all the diagonal elements. Labeling each joint provides a proper layout required to set up for the method of joints portion, while pre-calculating the angle of components is essential for breaking down 2D inclined force vectors into simple horizontal and vertical parts. The nodes/joints were mapped sequentially across the top and bottom chords, and I used the Pythagorean Theorem and applied it to the 0.4m horizontal base and the 0.3m vertical height, to then establish a diagonal length of 0.5m. This helped yield the exact numbers for the horizontal force resolution, which ended up being cos(theta)=0.8 and then the vertical force resolution which was sin(theta)=0.6. I could have done inverse tangent, but this way was easier and more efficient.
![image alt](

## Analyze


## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

