# Week 0 Lecture Notes

Run time: 1:10:34

Computer Science is mainly about *problem solving* collaboratively with other people or the work of others before you.

How you solve these problems comes down to how you represent the problem and what the issue might be. 

Example: How do you figure out how many people are in a class?

Either the old fashioned way with a piece of chalk or by using different combinations of raising a finger (or a few) to represent roughly 31-32 different people depending on whether or not you start at zero. 

Computers only speak one language: Binary. O or 1. Best representation of that is whether or not electricity is flowing through your computer, be it through a battery or a wall outlet.

How can they do anything useful?

If human beings can ascribe meaning to decimal points, computers can ascribe meaning to binary, just that the ones and zeroes represent different things. We go from ones, tens, hundreds, thousands, etc. to a ones, twos, fours, eights, sixteens and soon and so forth. 

Why?

One and 10 and 100 are powers of 10. 10 to the 0 is 1. 10 to the 1 is 10, 10 to the 2 is 100, and so on and so forth. Computers are using powers of two. (Binary-two)

If a computer was storing 0,0,0, it's zero in our human world. If it's 0,0,1, it's 1 in our human world. 

So why does 2 come to 0,1,0? All you are doing is representing another number by raising another value like you would if you are counting on your hand.

If you have five fingers or five bits (binary digits), you can get to as high as 31 just by starting to zero. On your hand, it's physically painful to represent all of those numbers but you can. 

*Why is this useful?*

Because a computer can represent any number of values from 0 to 1 to 2 to 3 and so on and so forth with enough bits.

*What are bits?*

Bits are just a series of ones and zeroes that represent powers of 2. The more digits, the more numbers you can represent. (1, 1, 1 comes to seven because it's a four, two, and a 1, and the sum comes to 7.)

*How do you represent say... letters with bits?*

Relate the numbers to letters by deciding upon a pattern to represent the letter A.

Years ago, humans decided that 65 was gonna be the decimal number for a capital A. A capital B, C, D, etc. is represented by 66, 67, 68, and so on and so forth. There's a mapping of 128 or 256 possible values for all keys seen on a typical keyboard to represent letters. 

*What distinguishes numbers from letters?*

Context, mainly. If you use a calculator program, the computer will represent this pattern of zeros and ones as numbers or symbols. Same with word processing applications or text messaging on your phone. 

This system is called ASCII (pronounced Ask-ee), the American Standard Code for Information Interchange.

72 and 73 in decimal translate to "Hi". 

If this message had a third byte (or an extra 8 bits), you can count even higher and account for more values.

72, 73, and 33 translate to "Hi!"

These decimal values respectively translate to 1001000, 1001001, 100001. 

*What we described above is referred to as Abstraction.*

**Abstraction: A term used to refer to taking low-level details and simplifying them for the purpose of conversation and contextualization.**
 
Problem: A keyboard has 100-200 characters that need to be represented on a screen. ASCII is only one standard that comprises 256 characters using numbers. That's not enough to rperesent all the symbols, accents or emojis. 

At some point human beings decided that ASCII and eight bits aren't enough, so the world started using Unicode to represent thousands or millions of characters using 1 or 2 or 3 or even 4 bytes, meaning 8, 16, 24, or even 32 bits to represent characters.  

Unicode is often a specific version known as UTF8. 

This emoji (and the most popular iPhone emoji btw): 😂 is represented in decimnal as 128,514 or 11111011000000010.

*How do you represent color?*

By interpreting it as imagery through RGB (Red Green and Blue). If you want to represent a single pixel, you use three bytes to respectively represent red, green, and blue. It's a lot like combining paint, only with waves of light emanating from your display.

72, 73, and 33 (out of 255 from 0, 256 from 1), come to a light yellow like in the emoji seen above. 

Zoom in even further and that emoji begins to pixelate. If you count up all the pixels onscreen, and multiply it by one, two, three bytes, thats how many bytes or kilobytes or megabytes to represent the image. 

So those are images. How about videos?

As a collection of images, each representing a frame that is shown in frames per second (usually 24 or 30 frames.) It's like a paper flipbook. Animojis, video files, and GIFS follow this principle.

Videos are bunches of images, images are bunches of colors, colors are bunches of bits and bits at the end of the day is the result of electricity going through your machine and its transistors. 

This hierarchy is especially important because it's a way to *represent* the various inputs and outputs to problems we need to solve. 

**Algorithms: Step by step instructions to solve a problem**

For instance: finding "Mike Smith" in a phone book.  You hypotehtically can go one page at a time except it would be extremely slow. You can go 2, 4, 6, 7, 10 etc. pages at a time but you might miss him. So to fix it you would start maybe towards the middle or towards the letter "S" after the middle of the phone book, and cut off however many pages out of the phone book depending on what you need. You go from 1000 pages to maybe 500 to even 200 bytes out of the problem. If you keep repeating this process, you solve the problem much faster.

Algorithms like this come down to a case of divide and conquer to efficiently narrow and solve a problem effectively. 

**Psuedocode: Using english-like syntax or any spoken language to express yourself succinctly and correctly so that a computer, robot or a person can understand what you're trying to say.**

For the phone book problem:

0. *pick up* phone book
1. *open to* middle of phone book
2. *look at* names
3. **if** *_Smith is among names_*
4.      *call* mike
5. **else if** *_Smith is earlier in book_*
6.      *open* to middle of left half of book
7.      go back to step 2
8. **else if** *_Smith is later in book_*
9.      *open* to middle of right half of book
10.     go back to step 2.
11. **else**
12.     *quit*

Italics: Functions
Bold: Conditionals 
Combined emphasis: Boolean expressions
Step 7 and Step 10 relate to loops. 


**Scratch: Programming with a graphical user interface using the above building blocks**

Building blocks in question?
1. Functions
2. Conditions
3. Boolean Expressions
4. Loops
5. Variables
6. Threads
7. Events
and more as we explore C, Python and much much more.

Scratch is very graphical, relying on actual building blocks to build programs using the above components. 

 Yellow: Functions
 Blue: Boolean
 Purple: Event

 Green Flag: Run Program
 Stop Sign: Stop Running

Characters can be added as sprites to represent different animations, actions, etc.

Each block fits together to map functions, loops, conditions, and variables to a program that can be run through the scratch editor. 

Scratch also allows you to take inputs from users to fill for variables. Questions like "what's your name?" or "How old are you?" are good examples.

To concatenate phrases to fulfill certain criteria like "Hello, <NAME>", you use the join block and drag the variable for <NAME> in the block. 

To play sounds, you can use the sound block to play a certain sound when a function is invoked (Hover, click, etc.)

If you want a sound to play multiple times, you need to use a loop to play the sound over and over again. You can even choose how many times the sound plays.

Scratch, like many programming languages, can perform arithmetical operations, including being able to double or square certain numbers. Numbers can reach as high as infinity or around 10^250th.

Forever blocks can listen in perpetuity for certain events to occur, a lot like a for loop.
(if mouse hovers over the sprite then play a sound for the time its hovering over the sprite)

If or Else blocks can listen for multiple events. (If a mouse is hovering over the sprite, play sound A, else play sound B.)

Animations can be performed through different versions of the same sprite. Making a character move around a screen without scrolling the sprite left and right can occur with a different sprite with its leg moving ever so slightly to mimic a walking motion.

Sprite art from video-games in the 8-16 bit era is a very good example of how sprite animations are made. The Mega Man games are a great example of this. 

Point Towards will allow you to create interactivity through making sprites point toward certain objects such as your mouse pointer.

Threads are used to simnultaneously chain together multiple scripts to achieve a more complex and/or interactive result.   

Events are needed to augment certain blocks or components and receive certain messages or conditions from other blocks. For instance, a sprite needs the broadcast block to hear the events from other sprites.

Custom Blocks can also be made using inputs, booleans, and labels to fulfill certain functions and execute certain events.

Scratch and custom blocks are a lot like solving problems in other programming languages like C and JavaScript, often by using things called libraries, or code that other people wrote that's useful to get the job done. 
 
DRY: Don't Repeat Yourself! Use a loop of some kind to keep yourself from repeating your own code.

All Scratch Projects demonstrated in this lecture are available from the CS50 website. 


# Week 0 Problem Set

*What to Do*
Download and install the latest version of Chrome, if you don’t have it already.
Implement your very own Scratch project using Chrome, per this specification.
Advice
Here’s how to try out David’s examples from lecture:

Download one or more of them or a ZIP of all of them, which you should then unzip.
Visit scratch.mit.edu, click Start Creating, select File > Load from your computer, and select the .sb3 file that you’d like to try out.

*Project 5050*
If you’d like to learn a bit more about others who’ve come before you, take a look at Project 5050 by CS50’s own Hailey James ‘19 et al.

https://youtu.be/0S7isdzIBU4?list=PLhQjrBD2T383RLDItqbDRs-4gWy8Wgec2


https://docs.cs50.net/2019/x/psets/0/index.html