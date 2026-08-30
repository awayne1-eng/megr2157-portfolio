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
![image alt](https://github.com/awayne1-eng/megr2157-portfolio/blob/4929f2e28cad054dde24a707421acc34c3e9e191/IMG_0952.jpeg)

Therefore, I was able to move on and start calculating the internal axial forces for the truss members connected to joints B, C, D, and A by isolating each node and executing a static equilibrium analysis. Analyzing the joints individually is necessary to determine the exact structural demand on each member, which allows me to classify whether they are acting in tension or compression, so that the correct material dimensions can be selected later to prevent buckling or yielding. The analysis was done sequentially by starting at Joint B, where there were only two unknown forces. I applied the horizontal and vertical equilibrium equations using my pre-calculated trigonometric multipliers to solve for the diagonal components. I then carried the solved member forces forward as known inputs to help isolate the remaining unknowns at Joint C, Joint D, and Joint A, which ultimately revealed that member DF functions as a zero-force element under this loading configuration.
Now, the previous step helped me find the remaining internal member force calculations by isolating Point E and Point F on the top chord of the truss structure. Analyzing these two were necessary because they helped find the load carried by member FE and to serve as equilibrium check to verify that the internal forces balance perfectly across the entire system. This step was completed by substituting the known member forces into the horizontal equilibrium equation at Joint E to isolate and solve for the compression force in member FE, followed by a vertical balance at Joint F which confirmed that member DF from earlier, carries zero load.
![image alt](https://github.com/awayne1-eng/megr2157-portfolio/blob/fadc273aa0387af5624fb88443eb89ce6e5106d2/IMG_0953.jpeg)
![image alt](https://github.com/awayne1-eng/megr2157-portfolio/blob/fd3b3ae4399ced6a8adf62f41a062bc999b888fe/IMG_0954.jpeg)

## Internal Forces (Symbollically and Numerically)
This step compiles the calculated internal member forces into two separate summary tables categorized by symbols such as positive or negative, and then by the true numerical values. Splitting this data into clear reference tables is important because it provides an organized view of the structural system, making it easier to identify critical design points. Member DE is a good example as it carries the largest tensile load for me at 26.67kN, which is required for selecting the appropriate member cross-sections in the final design phase. So, this summary was completed by putting together the previously solved joint forces, applying a sign convention where tension is (+) and compression is (-). Lastly, it also highlighted the maximum loaded members to ensure clear legibility for material optimization. 
![image alt](https://github.com/awayne1-eng/megr2157-portfolio/blob/662968201920abffa8660f61b7077295ad79bd1e/IMG_0955.jpeg)
![image alt](https://github.com/awayne1-eng/megr2157-portfolio/blob/49a50a9c354f1f3e089b9b6164be52a419c2c43f/IMG_0956.jpeg)

## Material Sizing/Cross-Sectional Area and Weight Approximation
I began this process by providing the knowns and unknowns, deriving the formulas to find the minimum required cross-sectional area using a safety factor of 3.5, and set up the math to estimate the total weight of the truss. I needed to do this to move from just calculating abstract forces to figuring out actual physical sizing, so the members don't yield under the maximum load, while also setting up a way to find the overall weight once a specific material density is picked. I started by writing down all the individual lengths to get a total truss length of 3.7m and used the maximum force of 26.67kN to set up my allowable stress equation. After this, I cross-multiplied and rearranged things to get a formula for the minimum area on its own. Since I needed to match standard US units, I converted the max force from kN to kips and changed the total length over to inches(145.67in). This let me simplify the area breakdown down to 20.98 over S_y in^2. I was then able to establish the final weight equation.
![image alt](
## Analyze


## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

