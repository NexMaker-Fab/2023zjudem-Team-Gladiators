## A. 脚步

  ### 第1步：使用GitHub开发网站所需的工具
 安装构建网页所需的所有工具
    
- [Git](https://git-scm.com); 它用作跟踪代码库更改、协作、管理项目版本的控制系统，这使我们能够克隆、提交更改并将更改推送到 GitHub。
- [Github](https://about.gitlab.com/); 这是我们的网页的托管位置。
- [Github desktop](https://www.gitbook.com/); 由于它是一个用户友好的 GUI 应用程序，我们用它来简化 Git 工作流程，使我们能够轻松克隆、提交和同步存储库。
- [VScode](https://code.visualstudio.com/); 我们使用这种多功能且可定制的工具来增强您的 Web 开发工作流程。
- [Nodejs](https://nodejs.org/en/);  由于该工具包含 NPM，因此我们用它来管理包、与命令行交互以及与 VScode 集成。
- [Markdown language](https://www.nexmaker.com/doc/1projectmanage/markdown.html); 这种语言通过创建标题、列表、链接、图像和强调来帮助我们格式化纯文本。

  ### 第二步：设置页面
 我们访问了 GitHub 网站 (https://github.com) 并注册了一个新帐户。登录后，我们单击 GitHub 主页右上角的“+”按钮，然后选择“新建存储库”。然后我们给它起了一个名字，并选择它是公共的还是私有的。然后，在启用自述文件后，我们编写了项目的一些描述。
<br>
<img style="float: center;" width=700 src="image/Createrepository.jpg">

  ### 第 3 步：本地设置

   ### 1. Github Desktop

 在 GitHub Desktop 中，我们转到“文件”和“克隆存储库”。
选择要克隆的存储库后。我们选择了保存克隆存储库的目录。然后我们单击“克隆”开始克隆过程。克隆完成后，我们导航到克隆存储库的位置。

<br>
<img style="float: center;" width=700 src="image/clone.jpg">



   ### 2. Vs Code

W我们使用 VS Code 的文本编辑器来自定义模板。
<br>
<img style="float: center;" width=700 src="image/clone.jpg">

### 3. 安装Docsify


 -我们打开终端，并通过在终端中输入“npm i docsify-cli -g”，我们安装了 docsify。
<br>
<img style="float: center;" width=600 src="image/installingdocsify.jpg">

 然后我们通过在终端命令中输入“docsify init./docs”对其进行初始化，以便 Docsify 在指定目录中创建必要的文件和文件夹。
  <br>
<img style="float: center;" width=600 src="image/initialize.jpg">

  -   然后，我们在命令终端中输入“docsifyserve docs”，指示 Docsify 为文档站点提供服务。我们通过单击 CTRL +“https://losthost:3000”在浏览器中打开。
  <br>
<img style="float: center;" width=600 src="image/serve.png">

 ### 4. 显示index.html.

        <!DOCTYPE html>
    <html lang="en" xmlns="http://www.w3.org/1999/html">
    <head>
    <meta charset="UTF-8">
    <title>Gladiators' docs File</title>
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
            placeholder: 'search',
            noData: 'No Results!',
            // Headline depth, 1 - 6
            depth: 6,
            hideOtherSidebarContent: false, // whether or not to hide other sidebar content
        },

        copyCode: {
        buttonText: {
        '/zh-cn/': '点击复制',
        '/'      : 'Copy to clipboard'
        },
        successText: {
        '/zh-cn/': '复制',
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

  - 为了预览网页，我们从 VS Code Marketplace 安装了“Live Server”扩展。打开 HTML 文件后，右键单击并选择“使用 Live Server 打开”。在网络浏览器中查看我们的网站。

   ### 5.  添加侧边栏和导航栏

-  活动

 + 网页

    - [Web开发](CHINESE/AC/step/page.md)
 
 + CAD
  
    - [Fusion 360 简介](CHINESE/AC/CAD/installation.md)
    - [任务](CHINESE/AC/CAD/handson.md)

 + ARDUINO

    - [ ARDUINO](CHINESE/AC/AD/arduino.md)

 + 印刷

   - [ 3D打印](#)
 
 + LASER

   - [ 激光切割](#)

 + 编程

   - [ 接口应用程序编程](#)

+物联网

   - [ 物联网与交互](#)

- 最终项目

   - [标题](CHINIESE/Project/proposal.md)
  
  
      -我们打开索引文件并转到窗口。.$docsify 然后加

              loadSidebar: true,

 - 可折叠侧边栏
要使侧边栏可折叠，您只需要在 window.$docsify 中添加这些代码即可


             subMaxLevel: 3,
             sidebarDisplayLevel: 1, // 设置侧边栏显示级别

然后将脚本插入到文档中，就像官方插件的用法一样

              <!-- plugins -->
               <script src="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/docsify-sidebar-collapse.min.js"></script>

- NAVBAR

创建文件e Navbar.md

             - [会员](INTRO/NAVBAR/member.md)
             - 语言
              - [中文](/中文/)

打开索引文件转到窗口.$docsify，然后添加

             loadNavbar: true,

   ### 6. 准备并保存文档

   ### 7. 法师上传
 我们在文档中创建了一个图像文件夹，用于存储所有图片。

名为“Image”的文件夹是在名为“docs”的目录中创建的。此文件夹的目的是存储与特定作业或文档相关的所有图片或图像。

然后我们将它们拖放到文档中。

我们在图像文件夹中找到所需的图像文件，并将其拖到我们正在处理的文档中。此操作将图像放置在文档中的所需位置。

“...使用 'img style="float: center;" width=700 src="IMAGE/nameof ourimage.png/jpg" 格式。'"

本部分描述如何使用 HTML <img> 标签将图像插入到文档中。

style="float: center;"：此属性将图像的浮动属性设置为“center”，这意味着图像将在其包含元素内水平居中。

width=700：该属性将图像的宽度设置为 700 像素。这决定了文档中图像的视觉尺寸。

src="IMAGE/Imageupload.png"：该属性指定图像的来源（src）。在本例中，它指向位于“IMAGE”文件夹中名为“name of our image.png/jpg”的文件。路径“nameof our image.png/jpg”表示图像文件夹位于当前目录内，图像文件名为““nameof our image.png/jpg”.png”。

格式：似乎提到了“格式”，但在此上下文中没有特定含义。它可能是作为占位符或出于其他目的而包含的，但它不会影响图像插入本身。

简而言之，我们描述了创建图像文件夹来存储图片的过程。然后，通过将这些图片拖放到所需位置，将它们添加到文档中。图像使用 HTML <img> 标签插入，该标签具有特定属性来控制其外观，包括对齐方式、大小和来源。
 <br>
<img style="float: center;" width=700 src="image/debugging.png">

 ### 第8步：上传文件
  1. 在我们的本地存储库和 GitHub 存储库之间建立了连接。
我们将文件推送到 GitHub：

为了将我们的网页文件上传到 GitHub，我们使用了命令“push commits to the origin remote”。
“push”命令将提交的更改从我们的本地存储库发送到 GitHub 存储库。
 <br>
<img style="float: center;" width=700 src="image/push.jpg">
   
 2. 
要发布我们的网页，我们查找 GitHub 存储库的设置。然后向下滚动到 GitHub Pages 部分并选择包含我们的网页文件的分支。
我们选择网页文件所在的文件夹或根目录。
然后单击“保存”或“更新”按钮以应用更改。
GitHub 为我们发布的网页生成了一个 URL，我们可以公开共享和访问该 URL。我们可以看到这个过程如下。

<br>
<img style="float: center;" width=700 src="image/setting.jpg">

<br>
<img style="float: center;" width=700 src="image/page.jpg">
<br>
<img style="float: center;" width=700 src="IMAGE/save.jpg">

## B. Setting up  the Members

 [Template](https://bestjquery.com/tutorial/our-team/demo16/)
<br>
 首先，我们下载了“saveallresource”工具并将其添加到 Chrome 扩展程序中。
“saveallresource”保存任何网站的所有文件和资产。它下载 HTML、CSS、JavaScript 文件、图像等资源，并保留文件夹结构。该工具帮助我们快速收集和保存所有必要的网站文件。

这是会员代码  

                    <div class="demo">
                        <div class="container">
                            <div class="row text-center">
                                <h1 class="white" style="text-align:left; font-size:40px;">小组成员 </h1>
                                <br>
                                <br>
                            </div>

                <div class="row">
                                <div class="col-sm-4">
                                    <div class="Members">
                                        <div class="pic">
                                            <img src="IMAGE/member1.jpg" alt=""/>
                                        </div>
                                        <div class="member-prof">
                                        <li><a href="https://danialkassa.github.io/"><h2>丹尼尔 卡萨</h2></a></li>
                                            <span><h3>来自埃塞俄比亚<h3></span>
                                            <p class="description">
                                            我对设计和编程感兴趣。我随时了解快速发展的领域的最新技术、趋势和设计原理。
                                            </p>
                                        </div>
                                    </div>
                                </div>

                <div class="col-sm-4">
                                <div class="Members">
                                    <div class="pic">
                                        <img src="IMAGE/member2.jpg" alt=""/>
                                        </div>
                                        <div class="member-prof">
                                        <li><a href="https://shahri128.github.io/EngShahari.github.io/"><h2>Shahar Yar</h2></a></li>
                                            <span><h3>来自巴基斯坦<h3></span>
                                            <p class="description">
                                                我是一位具有农业工程背景的多才多艺的学者，目前正在中国浙江大学攻读工业设计工程硕士学位。除此之外，我还与 YouTube 上的内容创作者分享了对解决技术问题的热情。</p>
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
                                            <img src="IMAGE/member3.jpg" alt=""/>
                                        </div>
                                        <div class="member-prof">
                                        <li><a href="https://sahle1415.github.io/Sah/"><h2>Sahle Hagos</h2></a></li>
                                            <span><h3>来自埃塞俄比亚</h3></span>
                                            <p class="description">
                                                我是一名化学工程师，热衷于以用户为中心和可持续发展的方式设计工业产品
                                                
                很快我将与任何需要我在行业产品设计方面支持的人联系。</p>
                                        </div>
                                    </div>
                                </div>

                <div class="col-sm-4">
                                    <div class="Members">
                                        <div class="pic">
                                        <img src="IMAGE/member4.jpg" alt=""/>
                                        </div>
                                        <div class="member-prof">
                                        <li><a href="https://arsl0011.github.io/alif.github.io/"><h2>Arslan</h2></a></li>
                                            <span><h3>来自巴基斯坦</h3></span>
                                            <p class="description">
                                            我是一名工业设计工程师。我的研究重点是设计的资源开发和管理方面。我一直对设计背后的科学感兴趣，这就是我选择在这个领域从事职业的原因。
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
                                        <img src="IMAGE/member5.jpg" alt=""/>
                                        </div>
                                        <div class="member-prof">,
                                            <li><a href="https://steve12437.github.io/"><h2>Steve</h2></a></li>
                                            <span><h3>从喀麦隆出发</h3></span>
                                            <p class="description">
                                            我性格外向、敬业、思想开放。我能够与人沟通并轻松适应变化。
                                            相信一个人应该努力发展自己的专业技能并不断学习新事物。
                                            </p>
                                        </div>
                                    </div>
                                </div>

                <div class="col-sm-4">
                                    <div class="Members">
                                        <div class="pic">
                                            <img src="IMAGE/member6.png" alt=""/></div>
                                        <div class="member-prof">
                                        <li><a href="https://atj12345.github.io"><h2>Ahmed Tajah</h2></a></li>
                                            <span><h3>从塞拉利昂出发</h3></span>
                                            <p class="description">
                                            我很自豪能成为部落富拉人，毕业于恩贾拉大学，拥有商业和信息技术荣誉学士学位和信息系统管理硕士学位。目前，我正在中国浙江大学攻读第二个硕士学位。
                                            </p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>



## C. 语言

在 VS Code 中打开时的文档文件内容

    .
    └── docs
       ├── README.md
       ├── index.htm
       ├── Sidebar.md
       └── navbar.md

英文版和中文版的网站是这样的

    .
    └── docs
       ├── README.md
       ├── Home.md
       ├── index.html
       ├── Sidebar.md
       └── navbar.md
    └── China
       ├── Home.md
       ├── README.md
       ├── index.html
       ├── Sidebar.md
       └── navbar.md

 索引文件

     homepage: 'home.md',
     mergeNavbar: true,

<br>
<img style="float: center;" width=700 src="image/language.jpg">

## D. 合作

 ### step1: 
   作为管理员，我登录 github 组帐户，然后单击“设置”。在侧边栏的“访问”部分中，单击“协作者和团队”。然后“添加人员”显示如下。

<br>
<img style="float: center;" width=700 src="image/add.jpg">
<br>

### Step2: 
如图所示，有“添加人员”部分。
 通过单击“添加人员”，我通过输入用户名、全名或电子邮件邀请了成员。然后显示以下图像后。

<br>
<img style="float: center;" width=700 src="image/select.jpg">
<br>

### Step3:
发出邀请后，我选择了团队中每个成员的角色作为维护角色。现在，每个会员都有权更改或编辑网站。
<br>
<img style="float: center;" width=700 src="image/list.png">
<br>


## E. 参考
 - [Nexmaker](https://www.nexmaker.com/)
 - [Docsify](https://docsify.js.org/#/?id=docsify)
 - [Template](https://bestjquery.com/tutorial/our-team/demo16/)
 - [Google Translate](https://translate.google.com)