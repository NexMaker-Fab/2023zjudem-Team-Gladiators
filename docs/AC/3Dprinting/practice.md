**3D printing practices**

- Digital 3D Model

1. **Cat standholder tool** From open source 3D modeling [Culs 3D](https://cults3d.com/en)
2. **Pipe holder** designed and assembled on fusion 360

- Material: PLA

|Filament Type |Super Power |Best Suited|Printing Temp|Heated Bed|
| :- | :- | :- | :- | :- |
|PLA|All natural and Biodegradable|<p>Prototypes</p><p>and products</p><p></p>|180- 210 <sup>o</sup>c|20-45 <sup>o</sup>c|


- **Slice software:** Flash print

A slicing program takes an STL or OBJ file and creates G-code, the code that instructs your 3D printer where to move the print head to, how fast to move it, and what path to follow.

- **Printer:** Flashforge Guider IIs

It is capable of delivering 3D print parts of industrial-grade accuracy and quality, usually used for model verification of structural prototypes or industrial designs.

**Steps**

<img src="image/step1.jpg" alt=""/>

**First trial:**  **Cat Standholder tool**

**Step 1.**  First make ready digital 3D model in STL or OBJ file by designing from scratch using computer-aided design software, scanning an object using 3d scanners  or download from open source websites. 

This standholder tool model is downloaded from open source [website Cults 3D](https://cults3d.com/en/3d-model/home/stand-holder-tool-for-iphone-ipad )

<img src="image/q0.jpg" alt=""/>

<img src="image/stl0.jpg" alt=""/>


**Step 2.** Use slice software to set printing parameter and slice

**First:** open the downloaded STL or OBJ file on FlashPrint software

<img src="image/s4.jpg" alt=""/>

**Second** : start slicing to set printing parameter

<img src="image/s5.jpg" alt=""/>

**Third:** Set printing parameter and slice 
<iframe width=100% height="430" src="image/pc.mp4" frameborder="0" allowfullscreen></iframe>
Set Parameters
<table><tr><th colspan="2" valign="top"><b>Parameters</b></th><th colspan="1" valign="top"><b>values</b></th></tr>
<tr><td colspan="2" valign="top">Machine Type</td><td colspan="1" valign="top">Guider II Series</td></tr>
<tr><td colspan="2" valign="top">Material Type</td><td colspan="1" valign="top">Flash forge- PLA</td></tr>
<tr><td colspan="2" valign="top">Nozzle Size</td><td colspan="1" valign="top">0.4 mm</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Temperature</td><td colspan="1" valign="top">Extruder temperature</td><td colspan="1" valign="top">210<sup>o</sup>c</td></tr>
<tr><td colspan="1" valign="top">Platform temperature</td><td colspan="1" valign="top">45<sup>o</sup>c</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">layer</td><td colspan="1" valign="top"><p>Layer height</p><p>(Thickness of one printed layer)</p></td><td colspan="1" valign="top">0.18mm</td></tr>
<tr><td colspan="1" valign="top"><p>First layer height</p><p>(This is the first layer of the model, which will affect the sticking performance between the model and platform)</p></td><td colspan="1" valign="top">0.27mm</td></tr>
<tr><td colspan="1" valign="top">Shells</td><td colspan="1" valign="top"><p>Shell count</p><p>(Number of paths superimposed for building the shell)</p></td><td colspan="1" valign="top">2</td></tr>
<tr><td colspan="1" rowspan="4" valign="top">Infill</td><td colspan="1" valign="top">Top solid layers</td><td colspan="1" valign="top">3</td></tr>
<tr><td colspan="1" valign="top">Bottom solid layers</td><td colspan="1" valign="top">3</td></tr>
<tr><td colspan="1" valign="top"><p>Fill density </p><p>(determines the interior solidity of the model)</p></td><td colspan="1" valign="top">15%</td></tr>
<tr><td colspan="1" valign="top"><p>Fill pattern </p><p>(The pattern of filling shape which effects printing duration.)</p></td><td colspan="1" valign="top">Hexagon</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Speed</td><td colspan="1" valign="top"><p>Print speed</p><p>(The moving speed of the extruder under printing status. Generally, the lower speed is, the better print you will get.)</p></td><td colspan="1" valign="top">60 mm/s</td></tr>
<tr><td colspan="1" valign="top"><p>Travel Speed</p><p>(the moving speed of the extruder under non-printing Status during work.)</p></td><td colspan="1" valign="top">80 mm/s</td></tr>
<tr><td colspan="1" valign="top">Cooling</td><td colspan="1" valign="top"><p>Cooling Fun control</p><p>(Cooling will increases the printing quality)</p></td><td colspan="1" valign="top">On when first layer printed</td></tr>
<tr><td colspan="1" valign="top">Platform adhesion</td><td colspan="1" valign="top"><p>Raft</p><p>(This function will help the model to stick well on the platform.)</p></td><td colspan="1" valign="top">yes</td></tr>
</table>

<img src="image/s7.jpg" alt=""/>

**Forth:** you can preview the slice and see the set printing parameters, estimated print time and estimated material required.

<img src="image/s8.jpg" alt=""/>

**Fifth:** Download the file on the printer directly using a USB cable or download the file on your flash disk and plug the flash disk directly on the printer

<img src="image/s9.jpg" alt=""/>

**Step-3**. Machine operation for printing

**First:** Check if there is enough material (PLA filament) to print out your model

<img src="image/s1011.jpg" alt=""/>

**Second:** Switch on the power and insert the flash drive containing the file

<img width=100% height="450" src="image/q12.jpg" alt=""/>

**Third:** print your model

<img src="image/s1314.jpg" alt=""/> 

<iframe width=100% height="450" src="image/vS3.mp4" frameborder="0" allowfullscreen></iframe>

<img src="image/s1516.jpg" alt=""/> 

**STEP 4.** Post processing
<br>This requires post processing only to remove the raft platform adhesion using metal scraper.

<img src="image/s1718.jpg" alt=""/> 

**Step 5.**  Testing the 3D object cat standholder tool

<img src="image/s1920.jpg" alt=""/>
<br>

**Second Trial:** **Pipe holder**

**Step 1.**  First make ready digital 3D model in STL or OBJ file by designing from scratch using computer-aided design software, scanning an object using 3D scanners  or download from open source websites.

For this pipe holder, we designed it from scratch using Fusion 360 software.
<br>
<br>
<img src="image/q.jpg" alt=""/>

<img src="image/s2.jpg" alt=""/>

<img src="image/stl.jpg" alt=""/>

**Step2:** Use slice software to set printing parameter and slice

<img src="image/q1.jpg" alt=""/>

**Note:** Remember to add support for models which have over hanging parts like this pipe holder

<img src="image/q2.jpg" alt=""/>

<iframe width=100% height="450" src="image/pp.mp4" frameborder="0" allowfullscreen></iframe>
Set parameters
<table><tr><th colspan="2" valign="top"><b>Parameters</b></th><th colspan="1" valign="top"><b>values</b></th></tr>
<tr><td colspan="2" valign="top">Machine Type</td><td colspan="1" valign="top">Guider II Series</td></tr>
<tr><td colspan="2" valign="top">Material Type</td><td colspan="1" valign="top">Flash forge -PLA</td></tr>
<tr><td colspan="2" valign="top">Nozzle Size</td><td colspan="1" valign="top">0.4 mm</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Temperature</td><td colspan="1" valign="top">Extruder temperature</td><td colspan="1" valign="top">210<sup>o</sup>c</td></tr>
<tr><td colspan="1" valign="top">Platform temperature</td><td colspan="1" valign="top">45<sup>o</sup>c</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">layer</td><td colspan="1" valign="top"><p>Layer height</p><p>(Thickness of one printed layer)</p></td><td colspan="1" valign="top">0.18mm</td></tr>
<tr><td colspan="1" valign="top"><p>First layer height</p><p>(This is the first layer of the model, which will affect the sticking performance between the model and platform)</p></td><td colspan="1" valign="top">0.27mm</td></tr>
<tr><td colspan="1" valign="top">Shells</td><td colspan="1" valign="top"><p>Shell count</p><p>(Number of paths superimposed for building the shell)</p></td><td colspan="1" valign="top">2</td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><p></p><p>Infill</p></td><td colspan="1" valign="top">Top solid layers</td><td colspan="1" valign="top">3</td></tr>
<tr><td colspan="1" valign="top">Bottom solid layers</td><td colspan="1" valign="top">3</td></tr>
<tr><td colspan="1" valign="top"><p>Fill density </p><p>(determines the interior solidity of the model)</p></td><td colspan="1" valign="top">15%</td></tr>
<tr><td colspan="1" valign="top"><p>Fill pattern </p><p>(The pattern of filling shape which effects printing duration.)</p></td><td colspan="1" valign="top">line</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Speed</td><td colspan="1" valign="top"><p>Print speed</p><p>(The moving speed of the extruder under printing status. Generally, the lower speed is, the better print you will get.)</p></td><td colspan="1" valign="top">60 mm/s</td></tr>
<tr><td colspan="1" valign="top"><p>Travel Speed</p><p>(the moving speed of the extruder under non-printing Status during work.)</p></td><td colspan="1" valign="top">80 mm/s</td></tr>
<tr><td colspan="1" valign="top">Cooling</td><td colspan="1" valign="top"><p>Cooling Fun control</p><p>(Cooling will increases the printing quality)</p></td><td colspan="1" valign="top">On when first layer printed</td></tr>
<tr><td colspan="1" valign="top">Support</td><td colspan="1" valign="top">When print suspended structure models, support is necessary</td><td colspan="1" valign="top">yes</td></tr>
<tr><td colspan="1" valign="top">Platform adhesion</td><td colspan="1" valign="top"><p>Raft</p><p>(This function will help the model to stick well on the platform.)</p></td><td colspan="1" valign="top">yes</td></tr>
</table>
This is how we preview the slice and download the gcode file
<br>
<img src="image/q3.jpg" alt=""/>

**Step 3.**  Printing
<br>
<iframe width=100% height="450" src="image/q8.mp4" frameborder="0" allowfullscreen></iframe>
<img src="image/q11.jpg" alt=""/>

**Step 4.** Post Processing

This model requires post processing to remove the support structures. This can be achieved by breaking the support structures from the build material using needle nose pliers and metal scraper.
<iframe width=100% height="450" src="image/q10.mp4" frameborder="0" allowfullscreen></iframe>
Here is the postprocessing result.
<br>
<img src="image/q5.jpg" alt=""/>
**Step 5.** Testing
<br>Here we can check the printed model with the designed one in the movement of its upper part as well as in assembling of M10 Nut.
<div style="display: flex; justify-content: space-between;">
  <div style="flex: 1; margin-right: 10px;">
    <iframe width="420" height="315" src="image/q4.mp4" frameborder="0" allowfullscreen></iframe>
  </div>
  <div style="flex: 1; margin-left: 10px;">
    <iframe width="420" height="315" src="image/q9.mp4" frameborder="0" allowfullscreen></iframe>
  </div>
</div>
