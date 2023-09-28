## Inputs

In this step you will use the buttons and some gestures to trigger **events** on your micro:bit. 

### Set up your workspace

--- task ---

**Choose:** 

Delete your previous code by dragging it over the Toolbox

**or**

Go back to the home screen and make a new project

--- /task ---

### Using the buttons

All micro:bits have **two** buttons you can use to trigger pieces of code in your programs. 

<img src="images/microbit-buttons.png" alt="The micro:bit simulator, with the two buttons A and B highlighted" width="250"/>

You can find the blocks to use the buttons in the `Input`{:class='microbitinput'} menu. 

--- task ---

Open the `Input`{:class='microbitinput'} menu and find the `on button`{:class='microbitinput'} block.

<img src="images/onbutton-location.png" alt="The Input menu with the on button block highlighted at the top." width="350"/>

--- /task ---

--- task ---

Drag the block into the workspace. 

--- /task ---

This is an **event** block, you can put other blocks inside of it and they will all run when the event happens. In this case the event is **button A being pressed**.

--- task ---

Drag a `show icon`{:class='microbitbasic'} block into the `on button `{:class='microbitinput'}.

```microbit
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Heart)
})
```

--- /task ---

--- task ---

**Choose:** an icon to show when the A button is pressed.

--- /task ---

--- task ---

Test your program on the simulator. 

Press the A button to see your icon.

--- /task ---

### Adding the other button

You can have many events in a single program! 

--- task ---

Open the `Input`{:class='microbitinput'} menu and drag another `on button`{:class='microbitinput'} block into the Workspace.

--- /task ---

At first the block will be faded out, because you can only have one event for each input. 

--- task ---

Use the dropdown to change the button for the event to `B` instead. 

<img src="images/switching-buttons.gif" alt="Using the dropdown to switch the second on button block to B" width="350"/>

--- /task ---

--- task ---

Add a block to run when you press B. 

You can use `show string`{:class='microbitbasic'}, `show leds`{:class='microbitbasic'} to draw your own icon or `show icon`{:class='microbitbasic'} to pick another pre-made icon.

--- /task ---

### Gestures

You can also use **gestures** as events in your programs as well. 

Gestures are movements with the micro:bit that you can react to, like **shake**, **tilting left or right** or **dropping** the micro:bit. 

--- task ---

In the `Input`{:class='microbitinput'} menu find the `on shake`{:class='microbitinput'} block.

<img src="images/on-shake-location.png" alt="Input menu open with the on shake block highlighted" width="350"/>

Drag it into your Workspace.

--- /task ---

This block will trigger whenever the micro:bit is shaken! 

--- task ---

Add some code to show something on the LEDs when you shake the micro:bit. either an icon, some words or a number!

--- /task ---

Your finalised code should look something like this...

```microbit
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Happy)
})
input.onButtonPressed(Button.B, function () {
    basic.showString("B button")
})
input.onGesture(Gesture.Shake, function () {
    basic.showIcon(IconNames.Confused)
})
```

### Touch logo (V2 only)

The newer version of the micro:bit has some extra events that use the new **touch sensitive** logo. 

You can trigger code when:

+ The logo is pressed 
+ The logo is held for a long time
+ The logo is released

--- task ---

If you are using a micro:bit V2, open the `Input`{:class='microbitinput'} menu and scroll to the micro:bit V2 section. 

Drag the `on logo`{:class='microbitinput'} block into your Workspace. 

<img src="images/on-logo-location.png" alt="The micro:bit v2 section of the Input menu open with the on logo block highlighted" width="350"/>

--- /task ---

--- task ---

Use the dropdown to change the event the `on logo`{:class='microbitinput'} block uses.

<img src="images/on-logo-event-options.png" alt="The on logo block, with the dropdown menu open to select which event to choos. The options are pressed, touched, released or long pressed." width="350"/>

--- /task ---

--- task ---

This is another event, so you can add some code inside the `on logo`{:class='microbitinput'} block.

This code will run when the event you have selected happens. 

In this example we have chosen to show some text when the logo is touched.

```microbit
input.onLogoEvent(TouchButtonEvent.Touched, function () {
    basic.showString("Logo!")
})
```

--- /task ---