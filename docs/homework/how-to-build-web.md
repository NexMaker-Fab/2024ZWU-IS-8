<h1 style="color: #e19cab;">How to Build a Website</h1>
<h2 style="color: #e19cab;">1. Preparation</h2>
  
We will use the following tools to construct our own web page:

- Git: Used to control versions of our code in GitLab. (PS. Based on experience, Mac users also need to download and install it. Remember to disconnect from the internet during installation, or it might get stuck.)
- GitHub: Serving as our web page hosting service.
- GitHub Desktop: Facilitating the transfer of our code from local to GitHub.
- Node.js for building environment.
- VScode for document writing.
- Markdown language for writing our documents.
- Image upload service: We use PicGo to store our images in the cloud (e.g., on GitLab) and use them in our markup documents.

<h2 style="color: #e19cab;">2. Web Page Setup</h2>

<h3 style="color: #e19cab;">Creating GitHub Repository</h3>

Firstly, you need to create a new repository on GitHub to host your website.

1. Log in to your GitHub account.

2. Create a public repository where you can collaborate with your team to create web content.

  ![图片1](https://cdn.jsdelivr.net/gh/zhuotiantian1/Mary/img/1.png)）

3. Name your repository, choose whether it's public or private. Add a README file to share your information, then click the "create repository" button.

    ![图片2](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/2.png)

4. 
Set the page to be empty. Click on the settings of the repository and select "Pages" on the left. Choose "main" and "/root" and save. The link above allows you to view the page.

    ![图片3](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/3.png)


<h3 style="color: #e19cab;">Invite Team Members</h3>

1. Open the created repository.
   ![图片4](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/4.png)

2. Click on "Settings", find "Collaborators" on the left, then click "Add people", enter their email addresses, and set their role (maintainer). 
   
   ![图片5](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/5.png)  

   ![图片6](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/6.png)

<h3 style="color: #e19cab;">Clone the repository to GitHub.</h3>

1. Click on "Add", "Clone a resource", find the repository you want to clone. Finally, click "Clone".

   ![图片7](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/7.png)  

   ![图片8](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/8.png)


<h2 style="color: #e19cab;">3. How to Deploy and Analyze Docsify Document Website</h2>
Docsify is a lightweight document website generation tool that allows you to quickly build interactive document websites. Below is a brief tutorial on how to deploy and analyze a document website using Docsify.

<h3 style="color: #e19cab;">1. Preparation:</h3>
Ensure that Node.js and npm are installed on your computer. You can run the following commands in the terminal (open VScode, open a new terminal) or command prompt to check if they are installed:

   <code>node -v</code>
   <code>npm -v</code>


![图片12](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/12.png)

If not installed, you can download and install from the official website of Node.js: [https://nodejs.org/](https://nodejs.org/)

Click on "Setting", find "Developer Setting", click on "Tokens (classic)", select "generate new token (classic)", then enter a name in the note, change the expiration to the desired time, then select "repo", "workflow", "write:packages", generate the key, and then copy it.

<h3 style="color: #e19cab;">2. Install Docsify</h3>

1. Install Docsify: Input the following code
   <code>npm i docsify-cli -g</code>

![图片19](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/19.png)

2. Determine the location, then initialize the environment: After entering the following code, input y in the yellow box.
            `docsify init ./docs`
![图片20](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c13c15d6c49abcfabcb0de1635df615765529b29/images/webbuild/20.png)

3. Preview: `docsify serve docs`

4. Access in browser:：http://localhost:3000

![图片21](https://cdn.jsdelivr.net/gh/zhuotiantian1/Mary/img/21.jpg)

<h3 style="color: #e19cab;">3. Deploying to GitHub Pages (Optional)</h3>

If you want to deploy the document website to GitHub Pages, you can push the Docsify project to a GitHub repository and enable the GitHub Pages feature.

<h3 style="color: #e19cab;">GitHub Desktop Login</h3>

1. Find your repository, click "Open in Visual Studio Code", input new content in Visual Studio Code, and save.

   ![图片9](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/9.png)

2. After making changes to the document, input any content in the first box, then click "Commit to main", and then "Push origin". If the icon displays a loop, synchronization is successful.

   ![图片10](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/10.png)  

   ![图片11](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/11.png)


<h2 style="color: #e19cab;">4. Image Upload</h2>

1. Install PicGo.
2. Create a new image repository on GitHub.
3. Access the image bed settings.
4. Obtain the key.
5. Set the custom domain to use CDN acceleration. For example, `https://cdn.jsdelivr.net/gh/username/repository`, complete the PicGo setup.

![PicGo Setup](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/13.png)  

![PicGo Key](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/14.png)  

![PicGo Upload](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/15.png)

6. Click on "Image Bed Settings", find GitHub, copy the key to the token, and fill in the rest as required.  

![PicGo Up load](https://cdn.jsdelivr.net/gh/zhuotiantian1/Mary/img/%E5%AF%86%E9%92%A5.png)
7. Then drag the picture to the upload area, check if it is uploaded successfully in the album, and you can also copy the picture path. 

![Upload Successful](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/17.png)  

![Copy Path](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/webbuild/18.png)

(ps. If PicGo configuration keeps failing, you can directly create a folder named "images" in your GitHub repository and add files to it.)


<h2 style="color: #e19cab;">5. Creating Webpage Cover</h2>

1. Create a new folder to store your Docsify project, and within that folder, create an HTML file named index.html. In Visual Studio, select "File" > "New" > "File", choose "HTML File" as the file type, and name the file.

![图片22](https://cdn.jsdelivr.net/gh/zhuotiantian1/Mary/img/22.png)

2. Write Configuration and Content: In the newly created HTML file, write the basic structure of the webpage, including <html>, <head>, and <body> tags. Within the <body> tag, write the content of the webpage cover, including titles, slogans, background images or videos, etc.ps: Because markdown only supports basic text writing, we often need <html> to assist with complex formats and styles

![图片24](https://cdn.jsdelivr.net/gh/zhuotiantian1/Mary/img/24.jpg)

<h2 style="color: #e19cab;">6. Add CSS Styles</h2>

In the `<head>` tag, you can use `<style>` tags or link external CSS files to add styles to the webpage cover, including adjusting the size of background images, text color, and size, etc.

```html
<!DOCTYPE html>/* Document type html */
<html lang="en">/* Specify language as English */
<head>
  <meta charset="UTF-8">/*Set character set to UTF-8 */
  <title>BUNBUN TEAM</title>/*Set page title */
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
  <meta name="Welcome! Here is the website of the BUNBUN Group, we are a group of five people with no basic computer knowledge, but we are always curious, learning spirit and our own unique personality! Let's always keep it warm!" content="Description">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">

  <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify@4/lib/themes/vue.css">/*Import Docsify default theme style */
  <link rel="stylesheet" href="custom.css"> /*Import custom CSS file */
</head>
<body>
  <div id="app"></div>
  <script>
    window.$docsify = {/*Set Docsify configuration */
      name: 'BUNBUN TEAM',/*Set website name */
      repo: 'https://nexmaker-fab.github.io/2024ZWU-IS-BUNBUN/',/*Set repository link*/
      loadSidebar:true,  /*Whether to load the sidebar*/
      coverpage: 'coverpage.md',/*Set cover page*/
    }
  </script>
  <!-- Docsify v4 --> /*Import Docsify library  */
  <script src="//cdn.jsdelivr.net/npm/docsify@4"></script> 
</body>
</html>
```

<h2 style="color: #e19cab;">7. Setting up the Cover Page</h2>

Create a cover page file

![Cover Page](https://cdn.jsdelivr.net/gh/zhuotiantian1/Mary/img/25.png)
```markdown
<!-- coverpage. md —> /*Markdown language */
<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/   /*Title "BUNBUN"  */
7a18b93ef8f24a06ee2b7e4459f9f88af37e92df/images/WechatIMG357-jpg" alt="Group
Image"width="500" style="display:block;margin:auto;">
#<span style= "color: white:">BUNBUN</span>  /*Use white font */
><span stvle="color: white:">Hello! This is Group 8 - BUNBUN! Here is our
group's website! Nice to meet you!</span>
-<span style="color: white;'>Keep the passion!</span>
[Get Started] (Team-introduce/Team-introduce.md)  /*Link to team introduction page */
<!--Set background in Markdown file-->
<!-- Set background color-->
! [color] (#030e1b)
```
<h2 style="color: #e19cab;">8. Establishing the Sidebar</h2>

<h3 style="color: #e19cab;">1. Add a Sidebar Container in the Webpage Cover</h3>

In the HTML structure of the webpage cover, add a `<div>` or other container element as the container for the sidebar.

<h3 style="color: #e19cab;">2. Write Sidebar Content</h3>

Within the sidebar container, write the content of the sidebar, including navigation links, search box, personal profile or information, etc.

![Sidebar Content](https://cdn.jsdelivr.net/gh/zhuotiantian1/Mary/img/sideba2r.png)

```markdown
-  [Team introduce](Team-introduce/Team-introduce.md)
- Team members   /* Main Part 1 */
  - [Rain](Teammembers/Rain.md)      /* Subpart */
  - [Mary](Teammembers/Mary.md)
  - [Ivy](Teammembers/Ivy.md)
  - [Jessica](Teammembers/Jessica.md)
  - [Harlan](Teammembers/Harlan.md)
- Daily homework     /* Main Part 2 */
  - [1. how to build web](homework/how-to-build-web.md)
  - [2. arduino basic](homework/arduino-basic.md)
  - [3. arduino input](homework/arduino-input.md)
  - [4. arduino output](homework/arduino-output.md)
  - [5. processing](homework/processing.md)
  - [6. CAD](homework/cad.md)
- Final project      /* Main Part 3 */
  - topic
  - innovation
  - market
  - how to design
  - how to make
  - SDGs
```
<h3 style="color: #e19cab;">3. Add CSS Styles to the Sidebar</h3>

Use CSS styles to add styles to the sidebar container and its contents, including setting background color, border styles, text styles, etc.

![PicGo](https://cdn.jsdelivr.net/gh/zhuotiantian1/Mary/img/css.png)
```html
body {
background-color:#030e1b; /* Background color for the main body */
color:#ffff; /* Font color for the main body */
}
h1, h2, h3 {
color:#f9f9f9: /* Font color for headings */
}
.sidebar {
background-color:#e19cab; /* Background color for the sidebar */
color: #030e1b; /* Font color for the sidebar */
}
.coverpage {
background: linear-gradient(to right, #030e1b, #0b3459) !important; /* Gradient background color for the cover page */
color:white !important; /* Font color for the cover page */
}
```

<h3 style="color: #e19cab;">4. Testing and Debugging</h3>

After saving the file, view the effect of the webpage cover and sidebar in a browser to ensure they display and respond correctly on different devices.

<h2 style="color: #e19cab;">9.Markdown Sample Document</h2>

This is a simple example demonstrating how to write documents using Markdown.

```markdown
## Setting Font Size

You can use HTML `<span>` tag to set font sizes. For example:

<span style="font-size: 24px;">This is text with font size of 24px.</span>

<span style="font-size: 18px;">This is text with font size of 18px.</span>

## Headings

Use `#` symbol to create headings. You can use different number of `#` symbols to represent different levels of headings. For example:

# This is a first-level heading

## This is a second-level heading

### This is a third-level heading

#### This is a fourth-level heading

## Code Highlighting

You can use triple backticks ``` to surround code blocks and specify the code language for syntax highlighting. For example:

```python
def greet(name):
    print("Hello, " + name + "!")


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>This is a sample HTML document.</p>
</body>
</html>
```
This is a simple Markdown sample document showing how to set font sizes, headings, and code highlighting.  You can modify and expand it according to your needs.

Because markdown only supports basic text writing, we often need <html> to assist with complex formats and styles. A simple code demonstration follows


```C++
# <h1 style="color: #e19cab;">Arduino basic</h1>

## <font size="5"><h2 style="color: #e19cab;">2.Arduino IDE</h2></font>


### <h3 style="color: #e19cab;"> (1) Introduction</h3>


**To download the Arduino IDE:** 

The Arduino Integrated Development Environment (IDE) is the place to write, compile, and upload code to Arduino boards.It can be downloaded for free from the [Arduino website](https://www.arduino.cc/en/Main/Software)where you can choose the version you want and install it on your computer.

**Connecting to the computer:** 

Connect the Arduino board to the computer using a USB cable, and the computer will automatically detect the board. 

In the Arduino IDE, open a new sketch by selecting`File` > `New`, which opens a new window for writing code. A basic Arduino sketch consists of two main functions: `setup()`and`loop()`。The `setup()` function is called once when the board starts, and the `loop()`unction is called repeatedly as long as the board is powered on.

**Uploading the sketch:** 

After writing the code, click the upload button (right arrow icon) in the Arduino IDE to upload it to the Arduino board. The IDE compiles the written code and sends it to the Arduino board.

**Connecting components:** 

Once the Arduino board is set up and the code is uploaded, we can begin to connect components such as LEDs, sensors, motors, etc., to the Arduino board, using Dupont wires to make connections between the components and the pins on the board.

**Testing the project:** 

After everything is connected, power on the Arduino board and observe the actual operation of the project. If something isn't working as expected, you can return to the code, make changes, and then re-upload it.


![Arduino-IDE](https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/cfe7ae2c17bd472adca8561bedfd0ecc1638589b/images/Arduino/ArduinoIDE.png)
```