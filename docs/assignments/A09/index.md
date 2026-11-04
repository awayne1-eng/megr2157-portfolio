# A9 – Pulleys

## Objective
This project moves away from the CAD design portion of the course and focuses more on the mathematical design of a pulley system. The pulleys must be spaced between 4–6 inches apart, operate at a rotational speed of 1,000–2,000 RPM, and maintain a belt tension of 4–6 lbf. We also have specific material requirements to follow and must use a safety factor of 3. The main goal of this project is to apply engineering calculations to determine the proper dimensions and values while making sure everything falls within the required limits. Throughout the process, we also need to show our calculations, explain our design decisions, and document any challenges or problems that come up along the way.

## Pulley Design
For the pulley design, I decided to use a 5-inch center distance, an operating speed of 1,500 RPM, and a static belt tension of 5 lbf. Both pulleys have a diameter of 3 inches, and I used the given yield strength of 471 psi for the polyurethane belt with a safety factor of 3. I started by drawing the free-body diagram and using the belt tension equations to calculate the tight-side and loose-side forces, which came out to 7.78 lbf and 2.22 lbf. From there, I used the normal stress equation to determine the minimum cross-sectional area and belt diameter needed to prevent failure. I calculated a minimum belt diameter of approximately 0.250 inches and a belt length of 19.425 inches. Based on these calculations, I selected a 1/4-inch round belt with a length of approximately 19 1/4 inches.
![My Image](IMG_1367.jpeg)

## Shaft Work
For the shaft design, I selected 1060 hardened steel and used its yield strength of 94,000 psi. I used the tight-side and loose-side belt forces from the previous section to determine the torque being applied to the shaft, which came out to 8.34 lb-in. After drawing the free-body diagram, I calculated the allowable shear stress using the material's yield strength and the required safety factor of 3. I then used the torsion equation to solve for the minimum shaft diameter. My calculations gave me a minimum diameter of approximately 0.140 inches, so I decided to use a 1/4-inch shaft to provide additional strength and meet the design requirements.
![My Image](IMG_1368.jpeg)

## Bearing Work
For the journal bearing, I used the combined belt forces to determine a net load of 10 lbf acting on the shaft. I selected a bearing length of 0.5 inches and used the 0.250-inch shaft diameter from my previous calculations. I first calculated the projected bearing area and used it to determine the bearing pressure, which came out to 80 psi. Next, I calculated the shaft's surface velocity using the 1,500 RPM operating speed, giving me approximately 98.17 ft/min. I multiplied the pressure by the velocity to determine a PV value of 7,854 psi-ft/min. Based on these calculations, I selected dry graphite as my bearing material because it is a potential option for dry-running applications.
![My Image](IMG_1369.jpeg)

## Frame Design
For the frame design, I decided to use 6061-T6 aluminum because it provides a lightweight support structure for the pulley system. I designed the frame with an overall length of 7 inches, a width of 1 inch, and a thickness of 0.25 inches, with the mounting holes spaced 5 inches apart. I used the 10 lbf loading condition to calculate the normal stress, which came out to 40 psi. I also calculated the moment of inertia and used Euler's buckling equation to determine the critical buckling load of approximately 5,140 lbf. After comparing this value to the applied load, I calculated a buckling safety factor of 514, which is well above the required safety factor of 3. Based on these results, the frame dimensions should provide sufficient resistance to buckling under the applied load.
![My Image](IMG_1370.jpeg)


## Decide


## Communicate

