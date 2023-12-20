## The MakeCode editor

In this step, you will take a tour of the MakeCode editor and create your first program for the micro:bit. 

### Open MakeCode

--- task ---

Open the MakeCode editor at [makecode.microbit.org](https://makecode.microbit.org){:target="_blank"}.

--- collapse ---

---
title: Offline version of the editor
---

There is also a [downloadable version of the MakeCode editor](https://makecode.microbit.org/offline-app){:target="_blank"}.

--- /collapse ---

--- /task ---

### The MakeCode homepage

The first screen you are presented with is the MakeCode homepage. Here, you will find the button to create new projects. 

![The MakeCode homepage, which has a banner that runs across the top. Underneath is the 'New Project' button. Finally, there is a row of tutorials underneath that.](images/makecode-homepage.png)

There are also loads of example projects and tutorials you can jump into when you are feeling confident using the micro:bit. 

### Start a project

--- task ---

Click on the **New Project** button.

<img src="images/new-project-button.png" alt="The New Project button inside MakeCode." width="250"/>

--- /task ---

--- task ---

Give your project a name — we will use **my first project**.

Click **Create** to get started with your project.

![The 'Create a Project' dialogue box, with the name 'my first project' written in the input box.](images/my-first-project.png)

--- /task ---

### The MakeCode editor

Now you will see the MakeCode editor; this is the screen you will use to program your micro:bit. 

![The MakeCode editor. On the left is the micro:bit simulator. The middle section is the Toolbox, with many categories of blocks you can use. Finally, the Workspace is a wide section on the right of the page. Two blocks are already in the Workspace, an 'on start' and a 'forever' block.](images/makecode-editor.png)

--- task ---

The very first thing that will happen is you will be offered a tour of the editor. Take the tour to explore the MakeCode interface.

--- /task ---

Below is a quick reminder of the different parts of the editor, for you to refer back to later or to help you better understand the interface.

--- collapse ---

---
title: The simulator
---

<img src="images/microbit-simulator.png" alt="The micro:bit simulator, a virtual version of the micro:bit with buttons below to start a simulation, restart a program, and debug." width="350"/>

On the left-hand side of the editor is a virtual version of the micro:bit — called **the simulator**. This allows you to test your projects while you create them, without having to download them to the physical device. 

--- /collapse ---

--- collapse ---

---
title: The toolbox
---

The micro:bit can be programmed using blocks, JavaScript, or Python. For your first few projects, we recommend you stick with the blocks. 

The toolbox is where you get the blocks that make up your program. It is split into **categories** that are colour-coded. You might be familiar with this sort of thing if you have used Scratch. 

The blocks in each category will do a specific type of task — like playing music or doing maths operations. 

You will be using the toolbox a lot!

<img src="images/toolbox.png" alt="The Toolbox of MakeCode, with menus for Inputs, Music, Loops, and more."/>

--- /collapse ---

--- collapse ---

---
title: The workspace
---

<img src="images/workspace.png" alt="The MakeCode workspace, with two blocks on it - 'on start' and 'forever'." width="350"/>

This is the biggest section of the editor, and it is where your program goes. 

When you grab blocks from the toolbox, you will place them in the workspace. Only things in your workspace will run. 

Every new project automatically has two blocks to get you started: `forever`{:class='microbitbasic'} and `on start`{:class='microbitbasic'}.

--- /collapse ---

### Create your first program

--- task ---

You only need the `forever`{:class='microbitbasic'} block for this program. 

Grab the `on start`{:class='microbitbasic'} and drag it over the toolbox.

![The MakeCode editor, with the 'on start' block held over the Toolbox. The Toolbox is highlighted red and a purple bin is over the top of it.](images/delete-block.png)

You should see a rubbish bin appear when you do this. Release the block to **delete** it. 

--- /task ---

--- task ---

Open the `Basic`{:class='microbitbasic'} menu in the toolbox. 

<img src="images/show-string-location.png" alt="The Basic menu, with the 'show string' block highlighted." width="350"/>

Grab a `show string`{:class='microbitbasic'} block. 

--- /task ---

--- task ---

Place the `show string`{:class='microbitbasic'} block **inside** the `forever`{:class='microbitbasic'} block in the workspace. 

The blocks will fit together like puzzle pieces.

![A demonstration of dragging the show string block from the ToolBox and placing it inside the 'forever' block. The blocks clip together when placed.](images/place-block.gif)

--- /task ---

--- task ---

The simulator will immediately run your program. You will see the word `Hello!` scroll across the LEDs. 

Change the text in the `show string`{:class='microbitbasic'} to your name. 

My name is Mac, so I will change it to that. 

```microbit
basic.forever(function () {
    basic.showString("Mac!")
})
```

**You should notice that when you make a change to your code, the simulator restarts.**

--- /task ---

--- task ---

From the `Basic`{:class='microbitbasic'} menu of the toolbox again, grab a `show icon`{:class='microbitbasic'} block. 

<img src="images/show-icon-location.png" alt="The Basic menu, with the 'show icon' block highlighted." width="350"/>

--- /task ---

--- task ---

Drag the `show icon`{:class='microbitbasic'} block **underneath** the `show string`{:class='microbitbasic'} block in the workspace. 

```microbit
basic.forever(function () {
    basic.showString("Mac!")
    basic.showIcon(IconNames.Heart)
})
```

--- /task ---

The `show icon`{:class='microbitbasic'} block will display a picture on the LEDs. There are loads for you to choose from. 

--- task ---

Click on the heart icon at the end of the `show icon`{:class='microbitbasic'} block. 

You will see a drop-down menu, with all the available pre-made icons. 

<img src="images/show-icons.png" alt="The 'show icon' menu expanded, showing a choice of 20 icons, with the option to scroll to see more. Icons shown include a tick symbol, a cross symbol, a smiley face, and a duck." width="350"/>

Pick an icon you like!

--- /task ---

--- task ---

Watch your program in the simulator. 

--- /task ---

In the next step, you will learn how to download your program onto your physical micro:bit.
