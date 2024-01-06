# Fusion 360 Design Project
## **Step 1: Build Design and New Component**

### **1.1 (Bench Vise Assembly)**

This assembly consisting of Four components, here are the components

1.  Base

2.  Vice Jaw

3.  Jaw Screw

4.  Screw Bar

First create a new design by going to file select new design.

![](vertopal_bd95cf7762df4f4ab8388baa9bdf37f3/media/image1.jpg)

Go to documents setting and change the units to millimeter.

### **1.2 Assemble Section (New Component)**

-   In assemble section create a new component and give it a name Base.

![](vertopal_bd95cf7762df4f4ab8388baa9bdf37f3/media/image2.jpeg)

## **Step 2: Design 3D Model**

### **2.1 Solid (Create)**

-   In create section create a new sketch on the front plane with
    required dimensions.

![](vertopal_bd95cf7762df4f4ab8388baa9bdf37f3/media/image3.jpeg)

-   After Create Sketch click on Finish Sketch and then Use Extrude
    Command

![](vertopal_bd95cf7762df4f4ab8388baa9bdf37f3/media/image4.png)

![](vertopal_bd95cf7762df4f4ab8388baa9bdf37f3/media/image5.png)

### **2.2 Construct Section (Tangent) & Modify (Fillet)**

-   We have used tangent tool to tangent the Circles which we created
    with circle tool in Create Section.

![tangent](image6.2.png)

-   And we have used fillet feature which is present in Modify Section.

![](image6.1.png)

-   Now we use line command from create section and then after giving
    dimensions, we use vertical/horizontal tool from Constraints
    Section.

![Alt text](<Screenshot (249).png>)

![Alt text](<Screenshot (250).png>)

### **2.3 Inspect Section**

-   We use inspect Section to measure the distance between 2 points or
    to measure the angle between 2 points.

![](vertopal_bd95cf7762df4f4ab8388baa9bdf37f3/media/image8.jpeg)

### **2.4 Remaining Components**

-   We have designed **Vice Jaw, Jaw Screw** and **Screw Bar**
    respectively.

![](vertopal_bd95cf7762df4f4ab8388baa9bdf37f3/media/image9.png)


![](vertopal_bd95cf7762df4f4ab8388baa9bdf37f3/media/image10.png)


![](vertopal_bd95cf7762df4f4ab8388baa9bdf37f3/media/image11.png)


### **2.5 Assemble**

-   After designing all components, we used joint command, Just go to assemble and click on joint command.

![Alt text](image12.1-1.png)

- Now select the Components to join as component 1 and component 2.

![Alt text](image12.2.png)

- After that set the position of the component on the base where it should be located.

![Alt text](image12.6.png)

- Then go to motion and select type for this i selected slider type.

![Alt text](image12.7.png)

- And Then also select the slide axis (X-Axis)

![Alt text](image12.8.png)

- After that give the minimum and maximum joint motion limits and check preview, then click OK.

![Alt text](image12.4.png)

- In the same way join all the components with the use of joint command in assemble section.

![](vertopal_bd95cf7762df4f4ab8388baa9bdf37f3/media/image12.png)


### **2.7 Video of Design History**

<video width=100% height=56.25% controls>
  <source src="Videos/Video1.mp4" type="video/mp4">
</video>

## **Step 3: Test Contact Set/Motion Link and GIF of Working Condition**

- To set the motion link of the design model click on assemble section and then click on the motion link.

![Alt text](<Screenshot (443).png>)

- Now select those joints in which you want to create motion link.

![Alt text](<Screenshot (439).png>)

- After selecting the joint we set 10mm distance covers on every 360 degree rotation. It means if we rotate our screw bar 360 degree then our Vice Jaw covers 10mm distance.
  
![Alt text](<Screenshot (440).png>)

- Now right click on slidebar or revolute and then click on animate joint relationships to check the motion link.

![Alt text](<Screenshot (442).png>)

<br>
<img style="float: center;" width=100% src="AC/CAD/GIF Working.gif">
<br>

## **3.1: Motion of Components (gif)**

<br>
<img style="float: center;" width=100% src="AC/CAD/1.gif">
<br>

<br>
<img style="float: center;" width=100% src="AC/CAD/GIF 10.gif">
<br>

<br>
<img style="float: center;" width=100% src="AC/CAD/3.gif">
<br>

<br>
<img style="float: center;" width=100% src="AC/CAD/GIF Working.gif">
<br>

### **3D Model Live**

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e29812ef6a85811ad?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## **Step 4: Install and Use Plugin**


   - First of all in Fusion 360 go to Utilities and then go to Add-Ins,
    make sure you are connected to the internet.

![](\../../image/image1.png)

   - Then you see the option of Fusion 360 App Store, Click on it

![](\../../image/image2.png)

-  Now Select your required Plugin and download it.

![](\../../image/image3.png)

-  After download install the Plugin.

![](\../../image/image4.png)

-  Now again go to Utilities and then in Add-Ins ( Scripts and Add-Ins)
    and go to Add-Ins and select the Plugin you Installed and Use it.

![](\../../image/image5.png)

![](\../../image/image6.png)

-  And then Click on Run. As i Installed FM Gear so to use this I have
    to go to Create Option and Select FM Gear.

![](\../../image/image7.png)

-  Then Give your dimensions and Click on OK. It will Run and Create
    Your Design.

![](\../../image/image8.png)

![](\../../image/image9.png)![](\../../image/image10.png)

## **Step 5: Engineering Drawing (Vice Jaw)**

![Vice Jaw](<Vice Jaw.jpg>)

### **How to Design Drawing**

- To design drawing go to Design button in left corner and click on drawing from design as mentioned below.

![Alt text](<d 1-1.png>)

- In create drawing box click on select option in contents so that you can choose specific component of your design.

![Alt text](<d 2-1.png>)

- Then select the components from your design and choose the sheet size.

![Alt text](<d 3-1.png>)

- Now change the scale for your component as required.

![Alt text](d4-1.png)

- Now fix the position of the component on the sheet and go to projected view option to show your design in different views.

![Alt text](d5-1.png)

- Then click on main component and drag it to get different views.

![Alt text](d6-1.png)

![Alt text](d7-1.png)

- Then go to dimensions section and click on dimension or you can also do this by clicking D Key on your Keyboard directly.

![Alt text](d8-1.png)

- Now give the dimensions of your component.

![Alt text](d9-1.png)

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e21b141afc4ec8fc9?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## **Step 6: Design Practices**

### **6.1 Design by Arslan Ali**

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e29812ef6a85811ad?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### **6.2 Design by Shahar Yar**
#### **6.2.1: Cam and Follower Assembly**
**Working of Model**

<br>
<img style="float: center;" width=100% src="AC/CAD/Shahar Yar GIF 1.gif">
<br>

**Components of Cam and Follower Assembly**

<br>
<img style="float: center;" width=100% src="AC/CAD/Shaharyar 2.gif">
<br>

**Engineering Drawing of Cam**

![Cam](Cam.jpg)

#### **6.2.2: Hexagonal Nut**

![Hexagonal Nut](<Shaharyar img.png>)

**Engineering Drawing**

![Drawing](<Hexagonal Nut Drawing v1_page-0001 (1).jpg>)

### **6.3 Design by Daniel Kassa**
#### **6.3.1: Ball Bearing**

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e3bff8897a75b82bc?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### **6.4 Design by Sana**

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e5299e15e67c6c785?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### **6.5 Design by Sahle Hagos**

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e42e30dc2aab69ca6?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### **6.6 Design by Ahmed Tejan**

<iframe src="https://myhub.autodesk360.com/ue28cacf9/shares/public/SH512d4QTec90decfa6e294a15da7ed4a49d?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## **Step 7: Simple Parameter Design Practice**

- First of all go to Modify section and click on change parameters.

![Alt text](p1.png)

- Then click on this Add Button to add parameters.

![Alt text](p2.png)

- Now type the name for your parameter and give the expression or value and click ok. In this way you can add parameters.

![Alt text](p3.png)

- These are the parameters that i added to use it for my design.

![Alt text](p4.png)

- Now i selected the plane and use circle command to make my design.

![Alt text](p5.png)

![Alt text](p6.png)

- Now give the dimension by using parameter feature.

![Alt text](p7.png)

- I have added these 2 circles with the use of parameters and in this design second circle is linked with first one. If we change the expression or value of first one the dimension of the second circle will also be changed.

![Alt text](p8.png)

- Now i have used extrude command in create section.

![Alt text](p9.png)

![Alt text](p10.png)

- As i said earlier if we change the expression of our first parameter then the second one will also be changed because i used [Firstglad - Number] in expression of the second one.

![Alt text](p11.png)

- So as i changed 70mm into 50 then the secondglad which is 54mm changed to 34mm automatically.

![Alt text](p12.png)

- Now our final design also changed as we changed the parameters.

![Alt text](p13.png)

![Alt text](p14.png)

### **Use of Parameters in Our Design Model**

- First go to Modify section and click on change parameters.

![](<pr 1.png>)

![](<pr 2.png>)

- Now here you will find your model parameters so you can change them directly from here.

![](<pr 3.png>)

- Here you will see your component parameters. So we selected base to change its lenght.

![](<pr 4.png>)

![](<pr 5.png>)

- After changing the dimensions click Ok.

![](<pr 6.png>)

![](<pr 7.png>)

- So you can change any of your design component parameters (also angle degree dimensions).

![](<pr 8.png>)

![](<pr 9.png>)

- Now here we will change the vice jaw dimensions.

![](<pr 10.png>)

![](<pr 11.png>)

- After changing dimensions click ok, then you will see the results.

![](<pr 12.jpg>)

- As we have changed the dimensions of vice jaw so now you can see the difference clearly. So in this way we can change our design parameters easily.

![](<pr 13.jpg>)


## **Step 8: Practice for Automated Modeling (New Model)**

- We choose Cam Shaft Assembly designed by Shahar Yar for automated Modeling.
  
  ![Alt text](<Screenshot (421).png>)

  - First of all for automated modeling go to Automate section and click on it.

  ![Alt text](<Screenshot (421)-1.png>)

- Now Select faces that you want to connect to create new body or component for your model.
- ![Alt text](<Screenshot (424).png>)

  - After selecting faces to connect now select bodies that you want to avoid and click on generate shapes.

![Alt text](<Screenshot (425).png>)

  - Now select any shape that you like and click on Ok.

![Alt text](<Screenshot (426).png>)

![Alt text](<Screenshot (427).png>)

- Now go to your new body that you have created and right click on it and select Isolate.

![Alt text](<Screenshot (428).png>)

![Alt text](<Screenshot (429).png>)

- Here is the final design by using automate feature of Fusion 360.

![Alt text](<Screenshot (430).png>)

![Alt text](<image (6).jpg>)

### **Working Condition of this design after Automated Modeling**

<video width=100% height=56.25% controls>
  <source src="Videos/Automated Modeling Part.mp4" type="video/mp4">
</video>

## **Step 9: Introduction of another CAD Software**
### **AutoCAD** 
AutoCAD is a popular computer-aided design (CAD) software developed by Autodesk. It has been an industry-standard for 2D and 3D design and drafting for many years. AutoCAD is used in various industries, including architecture, engineering, construction, manufacturing, and more. Its versatility, extensive user base, and compatibility with other software make it a valuable tool for professionals in these fields.

Here are some key details about AutoCAD:

**2D and 3D Design**

  AutoCAD is used for both 2D and 3D design. It's well-known for its 2D drafting capabilities, which allow you to create precise technical drawings, floor plans, schematics, and more. It also supports 3D modeling, enabling the creation of 3D models and visualizations.

**User Interface**

AutoCAD has a user-friendly interface with a familiar ribbon-style toolbar. It provides a wide range of tools and commands for drawing, editing, dimensioning, and annotating drawings.

**Parametric Design**

While not as robust as some other 3D CAD software like SolidWorks, AutoCAD offers some parametric modeling capabilities. You can create and control geometric relationships between objects.

**Libraries and Templates**

 AutoCAD provides libraries of pre-built objects, blocks, symbols, and templates, which can save time and maintain consistency in design projects.

**Customization**

 AutoCAD is highly customizable. Users can create custom commands, menus, and tool palettes to streamline their workflow. It also supports the development of custom AutoLISP and Visual Basic for Applications (VBA) scripts.

**Automation and Batch Processing**

AutoCAD allows you to automate repetitive tasks and batch-process multiple files using scripting and programming, which can significantly improve productivity.

**Collaboration**

AutoCAD offers cloud-based collaboration tools that allow teams to work on the same project simultaneously, even if they are located in different places.

**File Compatibility**

AutoCAD files are widely compatible with other CAD software and can import/export various file formats, making it easier to work with clients and collaborators who use different software.

**Industry Specialization**

AutoCAD has industry-specific versions, such as AutoCAD Architecture, AutoCAD Civil 3D, and AutoCAD Electrical, which include specialized tools and features tailored to specific fields like architecture, civil engineering, and electrical design.

**Mobile and Web Apps**

 Autodesk offers AutoCAD mobile and web apps, allowing users to view and edit AutoCAD drawings on smartphones, tablets, and web browsers, which can be useful for on-the-go access and collaboration.

**Education and Training:**

 AutoCAD is widely used in educational institutions, and Autodesk provides educational versions for students and teachers. There is a vast amount of training material and certification programs available.



