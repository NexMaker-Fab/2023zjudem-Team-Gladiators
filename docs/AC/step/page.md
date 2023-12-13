## How To Develop the website

## A: Installing necessary Tools

` `We installed all the following tools to build the website

\- [Git](https://git-scm.com); It serves as a control system for tracking changes to the code base, collaborating, managing project versions, which allows us to clone, commit, and push changes to GitHub。

\- [Github](https://about.gitlab.com/);This is where our web page is hosted.

\- [Github desktop](https://www.gitbook.com/);Since it is a user-friendly GUI application, we use it to streamline our Git workflow, allowing us to easily clone, commit, and sync repositories.

\- [VScode](https://code.visualstudio.com/); We enhanced our web development workflow with this versatile and customizable tool.

\- [Nodejs](https://nodejs.org/en/);  Since the tool includes NPM, we used it to manage packages, interact with the command line, and integrate with VScode

\- [Markdown language](https://www.nexmaker.com/doc/1projectmanage/markdown.html); This language helps us format plain text by creating headings, lists, links, images, and emphasis.

## B: Set up the page

` `We visited the GitHub website (https://github.com) and registered a new account, login. 

 <br>
<img style="float: center;" width=100% src="image/login.jpg">
<br>
<br>
Once logged in, we click the "+" button in the upper right corner of the GitHub homepage and select "New Repository.
<br>
<br>
<img style="float: center;" width=100% src="image/plus.jpg">
<br>
<br>
Then we gave it a name (Team-Gladiators) being in the admin's account and selected whether it should be public or private. Then, after enabling the readme, click create repository.
<br>
<br>
<img style="float: center;" width=100% src="image/merge.jpg">
<br>
<br>
Then after, Go to setting located at the upper left side of Github homepage, then pages, go to main, enable root, save. 
<br>
<br>
<img style="float: center;" width=100% src="image/link.jpg">

## C: Local setup

### 1. Github Desktop

In GitHub Desktop, we go to Files and Clone Repository.
After selecting the repository to clone, We selected the directory to save the cloned repository. Then we click "Clone" to start the cloning process. Once the cloning is complete, we navigate to the location of the cloned repository.
<br>
<br>

<img style="float: center;" width=100% src="image/gi.jpg">

<br>
<img style="float: center;" width=100% src="image/clone.jpg">
<br>
<br>
We painted the VS code with red color to show that after installing vs code, we open it to start writing our documents.
<br>
<br>
<img style="float: center;" width=100% src="image/opn.jpg">

### 2. Vs Code Installation and Its Menus
<b>Download:</b>

Visit the official Visual Studio Code website at [visualstudio](https://code.visualstudio.com)
Click on the "Download" button, which will automatically detect your operating system and provide the appropriate download link.

<img style="float: center;" width=100% src="image/vs1.jpg">

<b>Installation:</b>
<br>Click the downloaded file to run the installer.Follow the instructions provided by the installer to complete the installation process. This typically involves accepting the license agreement, choosing the installation location, and selecting additional components or integrations if desired.
<br><b>Launching VS Code:</b>
<br>Once the installation is complete, you can launch VS Code from your desktop or start menu.
<br><b>User Interface Overview:</b>
<br>Visual Studio Code is a lightweight and customizable code editor. It features a clean and intuitive user interface. <br>Here are some key components:
<br><b>Menu Bar: </b> <br>Contains various menus for accessing different features and settings.
<br><b>Side Bar: </b>  <br>Provides quick access to file explorer, source control, extensions, and other views.
<br><b>Editor Area: </b> <br>The main work area where you write and edit code.
<br><b>Status Bar: </b> <br>Displays information such as line and column numbers, file encoding, and extension shortcuts.
<br><b>Extensions: </b> <br>VS Code has a vast ecosystem of extensions that provide additional functionality and language support. You can install extensions from the VS Code Marketplace.
<br><b>Language Support and Features:</b>
<br>VS Code supports a wide range of programming languages and offers numerous features to enhance your coding experience. These include syntax highlighting, code completion, debugging, version control integration, terminal access, and more.You can customize VS Code to suit your preferences by adjusting settings, installing themes, and configuring keybindings.
<br><b>Working with Projects: </b>
<br>You can open a project or individual files in VS Code by using the "File" menu or dragging and dropping them into the editor.VS Code provides various features for navigating, searching, and organizing your code within a project. After installling VS code, We opened our folder on the vs code to develop the website.

<br>
<img style="float: center;" width=100% src="image/vs.jpg">

<br>

### 3. Install Docsify

 In the VS code, We opened the terminal and New terminal.

 <br>
<img style="float: center;" width=100% src="image/term.jpg">

<br>

And by Writing "npm i docsify-cli -g" in the terminal and hit enter, we installed docsify.

<br>

<img style="float: center;" width=100% src="image/installingdocsify.jpg">
<br>

 We then initialize it by typing “docsify init./docs” in the terminal command and hit enter so that Docsify creates the necessary files and folders in the specified directory.

  <br>
<img style="float: center;" width=100% src="image/initialize.jpg">

  We then type "docsify serve docs" into the command terminal to instruct Docsify to serve the documentation site. We open it in the browser by clicking CTRL + "https://losthost:3000".

  <br>
<img style="float: center;" width=100% src="image/serve.png">

<br>

### 4. Set up the index.html

<br>

<img style="float: center;" width=100% src="image/des.jpg">
<br>

<b> 1. .nojekyll:</b>
<br>
<br>A file used by GitHub Pages to indicate that the site should not be processed as a Jekyll site.

<b> 2. index.html:</b>
<br>
<br>The main HTML file serving as the homepage of a website.
<br>
<br>
<b> 2. README.md:</b>
<br>
<br>A documentation file written in Markdown format, providing an overview and instructions for a project or repository.


    <!DOCTYPE html>
    <html lang="en" xmlns="http://www.w3.org/1999/html">
    <head>
    <meta charset="UTF-8">
    <title>Gladiators</title>
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="description" content="Description">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">
    <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify@4/lib/themes/vue.css">
    <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/sidebar.min.css" />
    <meta name="theme-color" content="#661a1d">
    <link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">
    <link rel="stylesheet" href="//unpkg.com/docsify/lib/themes/vue.css">
    <link rel="stylesheet" href="bootstrap-grid.min.css"/>

    <link rel="stylesheet" href="common-1.css"/>
        <link rel="stylesheet" href="style.css"/>
    <!-- Responsive-->
    </head>
    <div id="app"></div>

            <script>
        window.$docsify = {
        name: 'GLADIATORS',
        repo: '',

        loadSidebar: true, //prepare for sidebar
        loadNavbar: true, //prepare for navbar
        mergeNavbar: true,

        executeScript: true,
        homepage: 'home.md',
        search: 'auto', // default

        // complete configuration parameters
        search: {
            maxAge: 86400000, // Expiration time, the default one day
            paths: 'auto',
            placeholder: 'Search',
            noData: 'No Results!',
            // Headline depth, 1 - 6
            depth: 6,
            hideOtherSidebarContent: false, // whether or not to hide other sidebar content
        },

        copyCode: {
        buttonText: {
        '/'      : 'Copy to clipboard'
        },
        successText: {
        '/'      : 'Copied'
        }
    },



        subMaxLevel: 3,
        sidebarDisplayLevel: 1, // set sidebar display level
        }


    </script>
            <!-- Docsify v4 -->
            <script src="//unpkg.com/docsify/lib/plugins/search.js"></script>
    <script src="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/docsify-sidebar-collapse.min.js"></script>
            <script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
            <script src="https://unpkg.com/docsify-copy-code"></script>
        </div>
    </div>
    </body>
    </html>
  - To preview web pages, we installed the "Live Server" extension from the VS Code Marketplace.
  <br>
<br><img style="float: center;" width=100% src="image/pre.jpg">

<br>

   Once the live server preview is installed, We opened the HTML file, then right-click and select Open with Live Server. 
   <br>

<img style="float: center;" width=100% src="image/live.jpg">
<br>


  ### 5.  Add sidebar and navigation bar
 _sindebar.md

 <img style="float: center;" width=100% src="image/sd.jpg">
 
<!--docs/_sidebar.md -->

- ACTIVITIES

        + PROJECT MANAGEMENT

            - [Website Development](AC/step/page.md)

        + CAD
        
            - [Introduction to Fusion 360](AC/CAD/installation.md)
            - [Design and Workspace Tools](AC/CAD/tools.md)
            - [Assignment](AC/CAD/handson.md)
        
        + ARDUINO

            - [Assessment](AC/Arduino/assessment.md)

        + 3D PRINTING

        - [Theory](AC/3Dprinting/theory.md)
        - [Practice](AC/3Dprinting/practice.md)
        
        + LASER

        - [LASER CUTTING](#)

        + PROGRAMMING

        - [INTERFACE APPLICATION PROGRAMMING](#)

        + IOT

        - [IOT and INTERACTION](#)

        - FINAL PROJECT

        - [Proposal](AC/Project/proposal.md)
        

  
      -We open the index file and go to window. .$docsify and then add
              loadSidebar: true,

 - Collapsible sidebar
To make the sidebar collapsible,we just need to add this code in window.$docsify


             subMaxLevel: 3,
             sidebarDisplayLevel: 1, // Set sidebar display level

Then insert the script into the document, just like the official plugin usage

              <!-- plugins -->
               <script src="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/docsify-sidebar-collapse.min.js"></script>
 _navbar.md

 <img style="float: center;" width=100% src="image/nv.jpg">

 <br>

      <!--docs/_navbar.md -->
             - [HOME](home.md)
             - [MEMBERS](INTRO/NAVBAR/member.md)

Open the index file go to window.$docsify and add

             loadNavbar: true,


  ### 6. Upload Image

 We created an image folder in the document to store all the pictures.

A folder named "Image" is created in a directory named "docs". The purpose of this folder is to store all pictures or images related to a specific assignment or document.

Then we drag and drop them into the document.

We find the required image file in the images folder and drag it to the document we are working on. This action places the image at the desired location in the document.


    "...use 'img style="float: center;" width=100% src="IMAGE/nameof ourimage.png/jpg" format.'"

This section describes how to use the HTML <img> tag to insert images into a document.

 style="float: center;":
This attribute sets the float property of the image to "center", which means that the image will be centered horizontally within its containing element.

    width=100%:
 This attribute sets the width of the image to 100% pixels. This determines the visual size of the image in the document.

    src="image/foldr name.png": 
This attribute specifies the source of the image (src). In this case, it points to a file called "name of our image.png/jpg" located in the "image" folder. The path "name of our image.png/jpg" means that the image folder is located in the current directory, and the image file name is

    "name of our image.png/jpg".

Format: "Format" seems to be mentioned, but has no specific meaning in this context. It may be included as a placeholder or for other purposes, but it does not affect the image insertion itself.

In short, we describe the process of creating an image folder to store pictures. Then, add these pictures to our document by dragging and dropping them where we want. Images are inserted using the HTML <img> tag, which has specific properties to control its appearance, including alignment, size, and source.


 <br>
<img style="float: center;" width=100% src="image/im.jpg">

### 7. Set up  Members

 [Template](https://bestjquery.com/tutorial/our-team/demo16/)
<br>

 <img style="float: center;" width=100% src="image/mm.jpg">
 <br>
<br>

First we downloaded the "saveallresourse" tool and addded to the chrome extention. 
The "saveallresource" saves all the files and assets of any website. It downloads resources like HTML, CSS, JavaScript files, images, and more, preserving the folder structure. The tool helped us to quickly gather and preserve all necessary website files.

Here is the code to display the Members.   

            
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="stylesheet" href="style.css">
        <title>GLADIATORS</title>
        <link rel="stylesheet" href="teamstyle.css"/>
    </head>

    <body>
    <div class="container">
    <h2 style = "text-align: left; font-size:40px;">Group Introduction</h2>
            <strong><p> We , the Gladiators, are diverse group of passionate individuals studying industrial design engineering,<br> united by a common goal to create solutions that address the United Nations Sustainable Development Goals (SDGs).</</P></strong>
          
        </div>          
    </body>

    <div class="demo">
            <div class="container">
                <div class="row text-center">
                    <h2 class="white" style="text-align:left; font-size:40px;">Group Members </h2>
                    <br>
                    <br>
                </div>
    <div class="demo">
    <div class="container">         
                <div class="row">
                    <div class=" col-sm-4">
                        <div class="Members">
                            <div class="pic">
                                <img src="image/member1.jpg" alt=""/>
                            </div>
                            <div class="member-prof">
                            <li><a href="https://danialkassa.github.io/"><h2>Daniel Kassa</h2></a></li>
                                <span><h3>From Ethiopia</h3></span>
                                <p class="description">
                                      I am interested in design and programming. I stay updated in rapidly evolving fields with the latest technologies, trends, and design principles.</p>
                            </div>
                        </div>
                    </div>

    <div class="col-sm-4">
                        <div class="Members">
                            <div class="pic">
                            <img src="image/member2.jpg" alt=""/>
                            </div>
                            <div class="member-prof">
                            <li><a href="https://shahri128.github.io/EngShahari.github.io/"><h2>Arslan Ali</h2></a></li>
                                <span><h3>From Pakistan</h3></span>
                                <p class="description">
                                  I'm a versatile scholar with a background in agriculture engineering and am currently pursuing my master's in industrial design engineering at Zhejiang University, China. Beyond this, I share my passion for technical problem-solving as a content creator on YouTube.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    <div class="demo">
    <div class="container">         
                <div class="row">
                    <div class=" col-sm-4">
                        <div class="Members">
                            <div class="pic">
                                <img src="image/member3.jpg" alt=""/>
                            </div>
                            <div class="member-prof">
                            <li><a href="https://sahle1415.github.io/Sah/"><h2>Sahle Hagos</h2></a></li>
                                <span><h3>From Ethiopia</h3></span>
                                <p class="description">
                                      I am a chemical engineer with a passion of designing industry products in a user-centered and sustainability-oriented way, 
                                      and soon I will be in touch with anyone who needs my support in industry product design.</p>
                            </div>
                        </div>
                    </div>

    <div class="col-sm-4">
                        <div class="Members">
                            <div class="pic">
                            <img src="image/member4.jpg" alt=""/>
                            </div>
                            <div class="member-prof">
                            <li><a href="https://arsl0011.github.io/alif.github.io/"><h2>Arslan Ali</h2></a></li>
                                <span><h3>From Pakistan</h3></span>
                                <p class="description">
                                  I am an industrial design engineer. My studies focused on the resource development and management sides of designing.  have always been interested in the science behind designing, which is why I chose to pursue a career in this field.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    <div class="demo">
      <div class="container">
          <div class="row">
                    <div class="col-sm-4">
                        <div class="Members">
                            <div class="pic">
                            <img src="image/member5.jpg" alt=""/>
                            </div>
                            <div class="member-prof">,
                                <li><a href="https://steve12437.github.io/"><h2>Steve</h2></a></li>
                                <span><h3>From Cameroon</h3></span>
                                <p class="description">
                                  I am outgoing, dedicated,and open-minded. I get across to people and adjust to change with ease.
                                  believe that a person should work on developing their proffessional skills and learning new things all the time.
                                </p>
                            </div>
                        </div>
                    </div>

    <div class="col-sm-4">
                        <div class="Members">
                            <div class="pic">
                                <img src="image/member6.png" alt=""/></div>
                            <div class="member-prof">
                            <li><a href="https://atj12345.github.io"><h2>Ahmed Tajah</h2></a></li>
                                  <span><h3>From Sierra Leone</h3></span>
                                <p class="description">
                                  I am proud to be a Fula by tribe and a graduate of Njala University, holding both a BSc Hons in Business and Information Technology and an MSc in Information System Management.Currently based at Zhejiang University in China, I am pursuing my second master.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="col-sm-4">
                        <div class="Members">
                            <div class="pic">
                                <img src="image/member7.jpg" alt=""/></div>
                            <div class="member-prof">
                            <li><h2>Sana</h2></a></li>
                                  <span><h3>From pakistan</h3></span>
                                <p class="description">
                                  I hold a Bachelor's degree in BS Physics from Government Frontier College for Women, Peshawar. Currently, I am pursuing a Master's in Industrial Design Engineering at Zhejiang University, Ningbo, China, blending my passion for science and design into a unique skill set.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

### 8. Prepare and save documents In Vs Code

<br>
In Summary,To prepare and save documents in VS Code:
<br>Open VS Code.
<br><br>Create a new file or open an existing one.
<br><br>Edit the document.
<br><br>To save, go to "File" > "Save" or use Ctrl+S (Windows/Linux) or Cmd+S (Mac).
<br><br>To save with a different name or location, use "Save As" (Ctrl+Shift+S or Cmd+Shift+S).
<br><br>To save all open files, use "Save All" (Ctrl+K S or Cmd+K S).
<br><br>Consider using Auto Save for automatic saving (configure in "File" > "Auto Save"). 

<br>The whole Picture of docs file in VS code looks like this.

<br>
<img style="float: center;" width=100% src="image/vsc.jpg">
<br>

### 9: Upload files

<br>
  1. We established a connection between our local repository and the GitHub repository.
We commit and push the file to GitHub:

To upload our web files to GitHub, we used the command “push commits to the origin remote”.
The “push” command sends committed changes from our local repository to the GitHub repository.

 <br>

<img style="float: center;" width=100% src="image/commit.jpg">

 <br>
<img style="float: center;" width=100% src="image/push.jpg">
  <br>
   
<br>
 2. To publish our web page, we look for the settings for our GitHub repository. Then scroll down to the GitHub Pages section and select the branch that contains our web files.
We select the folder or root directory where the web page file is located.
Then click the "Save" or "Update" button to apply the changes.
GitHub generates a URL for our published web page that we can share and access publicly. We can see this process as follows.
<br>

<br>
<img style="float: center;" width=100% src="image/do.jpg">


## D. Collaboration

 ### Step 1: 

 <br>
As admin, I login the github group account, Then click  "Settings". In the "Access" section of the sidebar, click "Collaborators and teams". Then "add people" displayed as follows.
<br>
<br>
<img style="float: center;" width=100% src="image/add.jpg">
<br>

 ### Step 2: 

 <br>
As shown in the figure, there is   "add people" section.
 by clicking "add people", I invited the members by writing Username, Full name, or Email. Then after the following image dispalyed.
<br>
<br>
<img style="float: center;" width=100% src="image/select.jpg">
<br>

 ### Step 3: 
 <br>
   After sent invitation, I chose the role of every member in the team to have a mentain role. Now, every member has the right to change or edit the website. 
<br>
<br>
<img style="float: center;" width=100% src="image/list.png">
<br>

## E. How to write title,Header, content and picture

<br>
 How to Add Title and Home Image

<BR>

        <H2 style= "text-align: center; font-size:7vw" ><span style="color:orange"> Gladiators</span> </h2>
        <H3 style= "text-align: center; font-size:2vw" > <span style="color:light black">Smart Home</span>

    <img style="display: block;
        margin-left: auto;
        margin-right: auto; " src="image/home.png" alt="A beautiful image" class="center-image">


<img  style="display: block;
     margin-left: auto;
      margin-right: auto; " src="image/hm.jpg" alt="A beautiful image" class="center-image">
<BR>


 How to add Section 
<br> 

      ## A. Installing Necessary Tools
      ## B. Set up the Page
      ## C. Local Setup
      ## D. Collaboration
      ## E. How to write Title,Header, Content and Picture
      ## F. References

<BR>
 How to add subsections
<br>

        ### 1. Github Desktop
        ### 2. Vs Code
        ### 3. Install Docsify
        ### 4. Set up Index.html
        ### 5. Add sidebar and navbar
        ### 6. Upload Image
        ### 7. Set up Members
        ### 8. Prepare and Save Documents
        ### 9. Upload Files

<BR>
 How to Add Content and Picture .
<BR>
<br>
Here is a Sample

    ### 2. Vs Code Installation
        <b>Download:</b>

        Visit the official Visual Studio Code website at [visualstudio](https://code.visualstudio.com)
        Click on the "Download" button, which will automatically detect your operating system and provide the appropriate download link.

        <img style="float: center;" width=100% src="image/vs1.jpg">

        <br>
        <img style="float: center;" width=100% src="image/vs.jpg">

        <br>

        ### 3. Install Docsify


        In the VS code, We opened the terminal and New terminal.

        <br>
        <img style="float: center;" width=100% src="image/term.jpg">

        <br>

        And by Writing "npm i docsify-cli -g" in the terminal and hit enter, we installed docsify.

        <br>

        <img style="float: center;" width=100% src="image/installingdocsify.jpg">
        <br>

        We then initialize it by typing “docsify init./docs” in the terminal command and hit enter so that Docsify creates the necessary files and folders in the specified directory.

        <br>
        <img style="float: center;" width=100% src="image/initialize.jpg">

        We then type "docsify serve docs" into the command terminal to instruct Docsify to serve the documentation site. We open it in the browser by clicking CTRL + "https://losthost:3000".

        <br>
        <img style="float: center;" width=100% src="image/serve.png">

        <br>

        ### 4. Set up the index.html

        <br>

        <img style="float: center;" width=100% src="image/des.jpg">
        <br>

        <b> 1. .nojekyll:<b>
        <br>A file used by GitHub Pages to indicate that the site should not be processed as a Jekyll site.

        <b> 2. index.html:<b>
        <br>The main HTML file serving as the homepage of a website.
        <b> 2. README.md:<b>
        <br>A documentation file written in Markdown format, providing an overview and instructions for a project or repository.
            - To preview web pages, we installed the "Live Server" extension from the VS Code Marketplace.
        <br>

        <img style="float: center;" width=100% src="image/pre.jpg">

        <br>

        Once the live server preview is installed, We opened the HTML file, then right-click and select Open with Live Server. 
        <br>

        <img style="float: center;" width=100% src="image/live.jpg">
        <br>

        ### 5.  Add sidebar and navigation bar
        _sindebar.md

        <img style="float: center;" width=100% src="image/sd.jpg">
        
        <!--docs/_sidebar.md -->

    - ACTIVITIES
    
            + PROJECT MANAGEMENT

                - [Website Development](AC/step/page.md)

            + CAD
            
                - [Introduction to Fusion 360](AC/CAD/installation.md)
                - [Design and Workspace Tools](AC/CAD/tools.md)
                - [Assignment](AC/CAD/handson.md)
            
            + ARDUINO

                - [Assessment](AC/Arduino/assessment.md)

            + 3D PRINTING

            - [Theory](AC/3Dprinting/theory.md)
            - [Practice](AC/3Dprinting/practice.md)
            
            + LASER

            - [LASER CUTTING](#)

            + PROGRAMMING

            - [INTERFACE APPLICATION PROGRAMMING](#)

            + IOT

            - [IOT and INTERACTION](#)

            - FINAL PROJECT

            - [Proposal](AC/Project/proposal.md)
            

        
            -We open the index file and go to window. .$docsify and then add
                    loadSidebar: true,

        - Collapsible sidebar
        To make the sidebar collapsible,we just need to add this code in window.$docsify


                    subMaxLevel: 3,
                    sidebarDisplayLevel: 1, // Set sidebar display level

        Then insert the script into the document, just like the official plugin usage

                    <!-- plugins -->
                    <script src="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/docsify-sidebar-collapse.min.js"></script>
        _navbar.md

        <img style="float: center;" width=100% src="image/nv.jpg">
        
        <!--docs/_navbar.md -->
                    - [HOME](home.md)
                    - [MEMBERS](INTRO/NAVBAR/member.md)

        Open the index file go to window.$docsify and add

                    loadNavbar: true,
        
            
        <BR>

 How to add link 
<BR>


    Installing Tools to build the website:

    -[Git](https://git-scm.com); It serves as a control system for tracking changes to the code base, collaborating, managing project versions, which allows us to clone, commit, and push changes to GitHub。
    - [Github](https://about.gitlab.com/);This is where our web page is hosted.
    - [Github desktop](https://www.gitbook.com/);Since it is a user-friendly GUI application, we use it to streamline our Git workflow, allowing us to easily clone, commit, and sync repositories.
    - [VScode](https://code.visualstudio.com/); We enhanced our web development workflow with this versatile and customizable tool.
    - [Nodejs](https://nodejs.org/en/);  Since the tool includes NPM, we used it to manage packages, interact with the command line, and integrate with VScode
    - [Markdown language](https://www.nexmaker.com/doc/1projectmanage/markdown.html); This language helps us format plain text by creating headings, lists, links, images, and emphasis.<br>

## F. References 

 - [Nexmaker](https://www.nexmaker.com/)
 - [Docsify](https://docsify.js.org/#/?id=docsify)
 - [Template](https://bestjquery.com/tutorial/our-team/demo16/)
