## Sounds

In this step, you will see how the micro:bit can play sounds, including notes, melodies, and short audio clips (V2 only). 

The blocks in this step will all come from the `Music`{:class='microbitmusic'} menu in the toolbox.

If you are using a V1 micro:bit, you will need **wired** headphones and two **crocodile clip** cables for this step.

--- collapse ---

---
title: How to play sound on the V1
---

If you are using a V1 micro:bit, there is no speaker to play the sounds, so instead you have to attach headphones to the GPIO pins. 

Take a look at the [guide from micro:bit to help you attach your headphones](https://makecode.microbit.org/projects/hack-your-headphones/make){:target="_blank"}. 

Set the volume of the sound to around `60` before testing, as it is very **loud** by default.

You can test whether the headphones are working with the following code: 

```microbit
music.setVolume(60)
music.play(music.tonePlayable(262, music.beat(BeatFraction.Double)), music.PlaybackMode.UntilDone)
```

You can find the `play tone`{:class='microbitmusic'} and `set volume`{:class='microbitmusic'} blocks in the `Music`{:class='microbitmusic'} menu of your toolbox. 

<img src="images/headphone-test-blocks.png" alt="The Music menu open, with the play tone block highlighted in the Tone section." width="350"/>

You will have to download the program onto your micro:bit for this test. 

**Once you are sure it is working, make sure to delete the `play tone`{:class='microbitmusic'} block so you're ready for the next steps.**

--- /collapse ---

### Set up your workspace

--- task ---

**Choose:** Delete your previous code by dragging it over the toolbox.

**or**

Go back to the home screen and make a new project.

--- /task ---

### Play notes

The micro:bit can play individual notes or **tones**. 

--- task ---

Open the `Music`{:class='microbitmusic'} menu in the toolbox. 

Find the `play tone`{:class='microbitmusic'} block. 

<img src="images/play-tone-location.png" alt="The Music menu open, with the play tone block highlighted in the Tone section." width="350"/>

--- /task ---

--- task ---

Drag the `play tone`{:class='microbitmusic'} into the `on start`{:class='microbitbasic'} block. 

--- /task ---

--- task ---

Click on the `Middle C` part of the `play tone`{:class='microbitmusic'} block to change the note. 

Select `Middle E`. 

<img src="images/middle-e-change.png" alt="The play tone block, with the note select drop-down menu open, with Middle E selected." width="350"/>

--- /task ---

--- task ---

Right-click on the `play tone`{:class='microbitmusic'} block, and select **Duplicate**.

<img src="images/duplicate-play-tone.gif" alt="The play tone block is right-clicked, then Duplicate is selected from the menu. A new block appears and is dragged under the original inside the on start block." width="450"/>

Place the new block underneath the original, inside the `on start`{:class='microbitbasic'} block.

--- /task ---

--- task ---

Duplicate the block **five** more times. 

You should have **seven** `play tone`{:class='microbitmusic'} blocks in total.

--- /task ---

--- task ---

Change the notes in the `play tone`{:class='microbitmusic'} blocks so they match the code below. 

```microbit
music.play(music.tonePlayable(330, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
music.play(music.tonePlayable(294, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
music.play(music.tonePlayable(262, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
music.play(music.tonePlayable(294, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
music.play(music.tonePlayable(330, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
music.play(music.tonePlayable(330, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
music.play(music.tonePlayable(330, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
```

The notes are:
1. Middle E
2. Middle D
3. Middle C
4. Middle D
5. Middle E
6. Middle E
7. Middle E

--- /task ---

--- task ---

Listen to the tones when you are done, can you guess which song is playing?

--- /task ---

--- task ---

**Optional:** Use the internet to find the starting notes of a song you love, and see if you can change the tones in your `on start`{:class='microbitbasic'} block to match. 

--- /task ---

### Play melodies

You can also play some preprogrammed melodies from your micro:bit. 

You are going to use the `Input`{:class='microbitinput'} events you learnt about in the last step to do this. 

--- task ---

Open the `Input`{:class='microbitinput'} menu of your toolbox and drag an `on button`{:class='microbitinput'} block into your workspace.

--- /task ---

--- task ---

In the `Music`{:class='microbitmusic'} menu of the toolbox, find the `play melody`{:class='microbitmusic'} block in the **Melody Advanced** section.

<img src="images/play-melody-location.png" alt="The Melody Advanced section of the Music menu, with the play melody block highlighted." width="350"/>

--- /task ---

--- task ---

Drag the `play melody`{:class='microbitmusic'} block inside the `on button`{:class='microbitinput'} block. 

```microbit
input.onButtonPressed(Button.A, function () {
    music._playDefaultBackground(music.builtInPlayableMelody(Melodies.Dadadadum), music.PlaybackMode.InBackground)
})
```

--- /task ---

--- task ---

Use the drop-down menu to select a different melody. 

<img src="images/select-melody.gif" alt="The drop-down menu to select a melody is opened, showing the large amount of melodies available. Melody funk is chosen." width="350"/>

--- /task ---

--- task ---

Test your program using both the simulator and your physical micro:bit.

--- /task ---

--- task ---

If you are using a micro:bit V1, create another `on button`{:class='microbitinput'} to play a second melody when **button B** is pressed.

--- /task ---

### Play short audio clips (V2 only)

On the newer micro:bit, you have the ability to play short audio clips. 

--- task ---

From the `Input`{:class='microbitinput'} menu, drag another `on button`{:class='microbitinput'} block to your workspace. 

Change the button from `A` to `B`.

--- /task ---

--- task ---

Open the `Music`{:class='microbitmusic'} menu and find the `play`{:class='microbitmusic'} block from the micro:bit V2 section. 

<img src="images/play-block-V2-location.png" alt="The micro:bit V2 section of the music menu. A play block is highlighted at the top of the section." width="350"/>

--- /task ---

--- task ---

Drag the `play`{:class='microbitmusic'} block inside the `on button B pressed`{:class='microbitinput'} block.

```microbit
input.onButtonPressed(Button.B, function () {
    music.play(music.builtinPlayableSoundEffect(soundExpression.giggle), music.PlaybackMode.UntilDone)
})
```

--- /task ---

--- task ---

Click on the `giggle` part and select another clip. 

We have chosen `mysterious`!

```microbit
input.onButtonPressed(Button.B, function () {
    music.play(music.builtinPlayableSoundEffect(soundExpression.mysterious), music.PlaybackMode.UntilDone)
})
```

--- /task ---

--- task ---

Download the program onto your physical micro:bit. 

Test the program out: listen to the initial song and then press each of the buttons to hear the melody and audio clip. 

--- /task ---

### Challenge (optional)

Make a new program and use what you have learnt about events to create a piano (V1) or drum kit (V2).

--- collapse ---

---
title: Drum noises for the V2
---

You can get specific drum noises in the micro:bit v2 section of the `Music`{:class='microbitmusic'} menu. 

<img src="images/drum-noise-location.png" alt="The micro:bit V2 section of the music menu. A play block is highlighted at the top of the section." width="350"/>

You can use the drop-down menu on the block above, and open the **Gallery** tab to select one of the drum noises. 

<img src="images/drum-noise-gallery.png" alt="The Gallery tab of the play block, with the kick drum sound highlighted." width="350"/>

--- /collapse ---

Use the button events and add some sounds, so when you press each of the buttons, the notes or drum noises play.
