# A3 – Parametric and FEA

## Parametric Design
For this assignment, I had to parametrically design a bar in CAD. For the load, I was given a choice anywhere from 300lb-500lb, and I chose 400lb. The max axial deflection was 0.009in. It was also stated that the bar be designed from Aluminum with a range of Young's Modulus from (8.5-11.5) X 10^6 psi. I chose an outer diameter of 7in and an inner diameter of 4in for my aluminum bar. I used the area equation for a hollow circular cross section to calculate my area of 25.92in^2. From these dimensions, I also was able to get the thickness which was 1.5in. 

For my calculations, I chose an applied force of 400lb, which is within the range required for the assignment. I used a modulus of elasticity of 8.8 x 10^6 psi and the maximum deflection of 0.009in. Using the direct tension elongation equation and my area of 25,92in^2, I solved for the bar length and got 5,132.16in.
![My Image](IMG_1013.jpeg)
## CAD Parameters
I entered my calculated values into SolidWorks as global variables so the dimensions of the bar would be controlled parametrically. i used an elastic modulus of 8.8 x 10^6 psi, a maximum deformation of 0.009in, a 400lb load, and outer and inner diameters of 7in and 4in. I then linked these values to my dimensions and used the equation L = (E)(Deformation)(Area)/(F), which gave me a bar length of 5,132.16in. This allowed SolidWorks to automatically generate the bar based on the values from my calculations.
![My Image](IMG_1014.jpeg)
![My Image](IMG_1015.jpeg)
![My Image](IMG_1016.jpeg)
## FEA/CAD Designs
I generated a von Mises stress map using the same 400lb load from my original calculations. The maximum stress from the FEA was about 1.164 x 10^5 N/m^2, which is much lower than the 40ksi strength of aluminum given in the assignment. This showed that my bar could safely handle the applied load without exceeding the material strength.
![My Image](IMG_1036.jpeg)
I created a displacement map to see how much the bar moved under the 400lb load. The simulation showed a maximum resultant displacement of about 3.188mm, or 0.1255in. The colors show how the displacement changes along the length of the bar. I am aware that I probably did this part wrong and I was trying to fix it but didn't know what to do.
![My Image](IMG_1037.jpeg)
I also viewed the deformed shape to see how SolidWorks represented the bar's movement. The deformation is shown at a scale of 4,417.15, so the bending shown on the screen is greatly exaggerated and is not the actual shape the bar would take. This view helped me visualize where the deformation took place.
![My Image](IMG_1038.jpeg)
Lastly, I checked the factor of safety using the maximum von Mises stress. SolidWorks calculated the lowest factor of safety as 236.802, which is much greater than 1. However, the assignment requires comparison to an aluminum strength of 40ksi, so I separately checked the FEA maximum stress against 40ksi. The maximum stress was still far below 40ksi, so the design passes the strength requirement.
![My Image](IMG_1039.jpeg)
## Design Reflection
From my parametric hand calculation, I used a maximum axial deflection of 0.009in as provided. I used 8.8 x 10^6 psi for my elasticity, a cross-sectional area of 25.92in^2, and a load of 400lb, which gave me a calculated bar length of 5,132.16in. My SolidWorks FEA gave a maximum displacement of 3.188mm. I converted this to inches, and it became 0.1255in. I then calculated the percent difference using 2(0.1255-0.009)/0.1255+0.009 x (100) to then get a total percentage difference of 173.2%.

There was a large difference between my hand calculated deflection of 0.009in and my FEA displacement of 0.1255in. One likely reason is the difference in the loading and boundary conditions between the two methods. My hand calculation assumes that the 400lb force acts directly along the axis of the bar, while my SolidWorks results showed the bar bending. This means the FEA was most likely including bending displacement in addition to axial deformation, which caused a much larger displacement. 

For the intended design, I would trust my hand calculated result more for the axial deflection because the assignment is specifically based on direct axial tension. The equation I used directly relates to the load, length, area, modulus of elasticity, and axial deformation. Before trusting the FEA displacement more, I would need to make sure that the 400lb force was applied completely along the axis of the bar so that bending was not included in the result.

## Pin Hole
For the pin hole, I assumed a hole with a diameter equal to about half of the flat bar width, giving d/W = 0.50. I used a stress concentration factor of approximately K_t = 4.25. Using my FEA stress of 1.164 x 10^5 N/m^2 as a conservative nominal stress away from the hole, I estimated the peak stress as 4.947 x 10^5 N/m^2, or about 0.0718ksi. Compared to the 40ksi aluminum strength given in the assignment, this gives a factor of safety of approximately 557, so the bar would still pass the safety requirement within the pin hole.
![My Image](IMG_1040.jpeg)

## Engineering Lessons Learned
During this assignment, I learned how to use parametric equations in SolidWorks to control dimensions and how to run an FEA to check displacement, stress, deformation, and factor of safety. One mistake I made was not realizing at first that my FEA setup was causing the bar to bend instead of showing only axial deformation, which made my FEA displacement much larger than my hand calculated value. I also had to correct how I interpreted the factor of safety because the material strength being used in SolidWorks was different from the 40ksi value given in the assignment. These mistakes helped me understand how important the load direction, boundary conditions, and material properties are when comparing hand calculations to FEA results.

## Modify Design Parameters
Before doing my new calculations, I guessed that the length of my bar would decrease if I increased the load and made the cross-sectional area smaller. For my modified design, I changed the load from 400lb to 450lb and changed my outer and inner diameters from 7in and 4in to 5in and 3in. I kept the same material and modulus of elasticity so I could compare the new design to my original one. After changing the parameters and calculating the new length, I found that my guess was correct because increasing the load and decreasing the cross-sectional area caused the required length of the bar to decrease. This helped me see how changing individual design parameters affects the overall dimension of the bar.

## CAD Model
[Download my SolidWorks Bar Model](../../../Part1-Bar-A3.SLDPRT)




