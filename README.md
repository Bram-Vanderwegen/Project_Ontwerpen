# Project_Ontwerpen
This is my "Project Ontwerpen" project: a boost converter
![Altium_Schema_01](https://user-images.githubusercontent.com/79916566/110454792-f8720000-80c7-11eb-948d-1893035dc609.png)
As previously said this is a DC/DC boost converter. This circuit transforms a DC voltage to a higher DC voltage. At first current flows through an inductor by switching a mosfet on, this way a magnetic field is formed around the inductor. When the mosfet is closed the current stops flowing and the magnetic field collapses because there is no path anymore through the mosfet the current searches for another one and discharges through the load. Because the inductor tries to discharge as fast as possible the voltage rises considerably. This cycle is repeated rapidly and as result a constant higher voltage is created. The mosfet is driven by a microcontroller tht also reads voltage values across multiple resistors so that the voltage can be monitored and the right duty-cyle can be given to the mosfet. The microcontroller has an LCD-screen connected aswell where it displays the current values. There are also two buttons which can be used to set a constant voltage or limit the current.