# Quick Reaction Game
within this tutorial you will create a quick reaction game using an electronic circuit, that we will create below and we will code it using a Raspberry Pi and EduBlocks.

## Equipment You Will Need

* 2 x Buttons
* 1 x LED
* 1 x Breadboard
* 1 x 220Ω resistor
* 6 x Male to Female jumper wires
* 1 x  Raspberry Pi set up

## Creating The circuit
Using the components within this kit create the circuit below.

**NOTE:** *Make sure you have the LED's the right way round. The longer leg is the postive leg, this is marked by a bent leg on the digram.*

![Reaction Diagram](Images/Reaction.png)

<div class="page-break"></div>

## Opening EduBlocks

If EduBlocks is not already open double click on ![EduBlocks Logo](Images/EduBlocks.png) This should be located on your Desktop.

## Controlling The LED
When programming a project it makes sense to break it down into sections so you can tackle one problem at a time. This also makes it easier to to test your project at different stages.

Lets start with coding the LED.

![Controlling LED code](Images/Code01.png)

* To locate the pink blocks click on  ![Basic](Images/Basic.png)

* To locate the yellow blocks click on ![gpiozero](Images/GPIO_Zero.png) --> ![General](Images/General_Zero.png)

* To locate the red blocks click on ![gpiozero](Images/GPIO_Zero.png) --> ![Outputs](Images/Outputs.png) --> ![LED](Images/LED.png)


To test that the code works click on ![Run](Images/Run1.png).

If your LED does not turn on for 5 seconds and turn off again. you need to go back through your code and see where you went wrong. This is an important skill in programming called **debugging**. Which means finding and fixing errors or bugs within your code.

## Adding an Elemment of Surprise
The object of the game is to see who can press their button first when the LED goes off, so to make this better would be if the length of time the LED stayed on were random. You need to edit your code to make this happen.

![Code 02](Images/Code02.png)

To add the element of surprise we need to add the random library, which will be found in the ![Basic](Images/Basic.png) menu. Then we need to edit the time. sleep code.

Now run your code by clicking on ![Run](Images/Run1.png) and your light should now come on for a random amount of time between 5 and 10 seconds.

## Coding the Buttons
Now that the LED is working, it is time to get the buttons working, so you can detect which player wins. Edit your code to look like the code below.

![Code block 3](Images/Code03.png)  

* To locate the blue code blocks click on ![gpiozero](Images/GPIO_Zero.png) --> ![Inputs](Images/Inputs.png) --> ![Button](Images/Button.png)

## Writing the Function
At the end of the code we are now going to add a function, that will be called everytime a button is pressed.

![code04](Images/Code04.png)

## Adding the function to the buttons
We now need to add code to the buttons, so when they are pressed they call the function that we created

![code05](Images/Code05.png)

Now grab a friend and try out your game.

## Getting Player Names
Lets get players names, so the program will tell you who won, rather than which button was pressed.

To add the player names locate ![ = ](Images/Blank.png) and edit them to look like the code below.

![Code 06](Images/Code06.png)

## Editing the function

We now need to edit our function to output the name of the winner.

![code 07](Images/Code07.png)
