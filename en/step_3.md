## The MakeCode editor

In this step you will take a tour of the MakeCode editor, and create your first program for the micro:bit. 

### Opening MakeCode

--- task ---

Open the MakeCode editor at [makecode.microbit.org](https://makecode.microbit.org){:target="_blank"}

--- collapse ---

---
title: Offline version of the editor
---

There is also a [downloadable version of the MakeCode editor](https://makecode.microbit.org/offline-app){:target="_blank"}.

--- /collapse ---

--- /task ---

### The MakeCode homepage

The first screen you are presented with is the MakeCode homepage. Here you will find the button to create new projects, and all your existing projects (Once you have made some). 

![The MakeCode homepage, a banner runs across the top. Underneath is the 'New Project' button. Finally there is a row of tutorials underneath that.](images/makecode-homepage.png)

There are also loads of example projects and tutorials you can jump in to when you are feeling confident using the micro:bit. 

### Start a project

--- task ---

Click on the **New Project** button.

<img src="images/new-project-button.png" alt="The New Project button inside MakeCode." width="250"/>

--- /task ---

--- task ---

Give your project a name - we are going with **my first project**.

![The 'Create a Project' dialogue box, with the name 'my first project' written in the input box](images/my-first-project.png)

--- /task ---

--- task ---

Click **Create** to get started with your project

--- /task ---

### The MakeCode editor

Now you are presented with the MakeCode editor, this is the screen you will use to program your micro:bit. 

![The MakeCode editor, on the left is the micro:bit simulator. The middle section is the Toolbox, with many categories of blocks you can use. Finally the Workspace is a wide section on the right of the page. Two blocks are already in the Workspace, an 'on start' and a 'forever' block.](images/makecode-editor.png)

--- task ---

The very first thing that will happen is you will be offered a tour of the editor. Take the tour to explore the MakeCode interface

--- /task ---

Below is a quick reminder of the different parts of the editor, for you to refer back to later or to help you better understand the interface. 

#### The micro:bit simulator

On the left hand side is a virtual version of the micro:bit - called **the simulator**. This allows you to test your projects while you create them, without having to download them to the physical device. 

#### The Toolbox

The micro:bit can be programmed using blocks, javascript or Python. For your first few projects we recommend you stick with the blocks. 

The toolbox is where you get the blocks that make up your program. It is split into **categories** that are colour coded. You might be used to this sort of thing if you have used Scratch. 

The blocks in each category will do a specific type of task - like playing music or doing maths operations. 

You will be using the Toolbox a lot!

#### The Workspace

This is the biggest section of the editor, and it is where your program goes. 

When you grab blocks from the Toolbox, you will place them in the Workspace. Only things in your Workspace will run. 

### Creating your first program

--- task ---

You only need the <code style="background-color: #1e90ff">forever</code> block for this program. 

Grab the <code style="background-color: #1e90ff">on start</code> and drag it over the Toolbox.

![The MakeCode editor, the on start block is held over the Toolbox. The Toolbox is highlighted red and a purple bin is over the top of it.](images/delete-block.png)

You should see a rubbish bin appear when you do this. Release the block to **delete** it. 

--- /task ---

--- task ---

Open the <code style="background-color: #1e90ff">Basic</code> menu in the Toolbox. 

<img src="images/show-string-location.png" alt="The Basic menu, with the 'show string' block highlighted." width="350"/>

Grab a <code style="background-color: #1e90ff">show string</code> block. 

--- /task ---

--- task ---

Place the <code style="background-color: #1e90ff">show string</code> block **inside** the <code style="background-color: #1e90ff">forever</code> block in the Workspace. 

The blocks will fit together like puzzle pieces.

![A demonstration of dragging the show string block from the ToolBox and placing it inside the forever block. The blocks clip together when placed.](images/place-block.gif)

--- /task ---

--- task ---

The simulator will immediately run your program, you will see the word `Hello!` scroll across the LEDs. 

Change the text in the <code style="background-color: #1e90ff">show string</code> to your name. 

My name is Mac so I will change it to that. 

<div style="position:relative;height:calc(150px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/---codeembed#pub:_T3yfhfdbC9y6" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

--- task ---

Again in the <code style="background-color: #1e90ff">Basic</code> menu of the Toolbox, this time grab a <code style="background-color: #1e90ff">show icon</code> block. 

<img src="images/show-icon-location.png" alt="The Basic menu, with the 'show icon' block highlighted." width="350"/>

--- /task ---

--- task ---

Drag the <code style="background-color: #1e90ff">show icon</code> block **underneath** the <code style="background-color: #1e90ff">show string</code> block in the Workspace. 

<div style="position:relative;height:calc(175px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/---codeembed#pub:_EhKLF2HxhbuL" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

The <code style="background-color: #1e90ff">show icon</code> block will display a picture on the LEDs. There are loads for you to choose from. 

--- task ---

Click on the heart icon at the end of the <code style="background-color: #1e90ff">show icon</code> block. 

You will see a drop down, with all the available pre-built icons. 

<img src="images/show-icons.png" alt="The 'show icon' menu expanded, showing a choice of 20 icons, with the option to scroll to see more. Icons shown include a tick symbol, a cross symbol, a smiley face and a duck." width="350"/>

Pick an icon you like!

--- /task ---

--- task ---

Watch your program in the simulator. 

--- /task ---

In the next step you will learn how to download your program onto your physical micro:bit.