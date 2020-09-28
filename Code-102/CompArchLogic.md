# Notes on Computer Architecture and Logic: Reading 06b = Watching Videos

I. Video One: Introduction by Bill Gates to the series on how computers work

II. May-Li: Dsigner and Inventor; Nat: Designer of the x-box

    A. What makes a computer a computer? 

        i. it takes input;
        ii. stores information;
        iii. processes that information;
        iv. and outputs the result.

    B. How does it work?

    C. We've always built tools, first to help with manual work, now with intellectual work. 

    D. The earliest computers

        i. were made out of wood and metal with mechanical levers and gears;
        ii. by the 20th century, they were being built with electrical components;
        iii. they were large (the size of a room) and slow, taking hours to do a simple math problem, making them basic calculators;
    
    E. Modern computers

        i. still do the same four things as their predecessors
            a. Types of input: 
                - keyboard
                - mouse
                - microhone
                - camera
                - listening (to heartbeat, e.g.)
                - touchscreen
            b. Storage and processing
                - inputs stored in memory
                - the processor takes information from the memory and changes it using an algorithm--a series of commands--and sends the processed info back to storage until the processed info is ready to be output
            c. Output
                - text
                - photos
                - videos
                - games
                - virtual reality
                - signals to control a robot
                - to another computer via the internet

III. Limor: founder of and engineer at Adafruit Industries; with Federico, a software developer at Microsft; 

    A. Ones and Zeroes: how a computer works on the inside

        i. Electric wires and ciruits carry all the info in a computer
        ii. How info is stored or represented using electricity:
            a. single wire: the signal is either on or off, or a yes/no, or true/false, or 1/0 or anthing else with only two options.
            b. This single wire is called a bit = the smallest piece of info that a computer can store
            c. The more wires you have, the more bits you have
            d. The more bits you have, the more complex the information that can be represented
        iii. The binary number system
            a. Only two digits in this system: 0, 1
            b. the ones position, twos position, fours position and eights position (multiples of two) and so on
            c. E.g., the number 9 in binary = 1001 = (1x8)+(0x4)+(0x2)+(1x1)
            d. As such, any number can be respresented by 1s and 0s or by a bunch of wires that are either on or off.
            e. The more wires used in a computer, the larger the numbers that can be stored. 
            f. With 8 wires, numbers between 0 and 255 can be stored; with 32 wires, this number increases to over 4 billion.
            g. Text, images, and sound can also be represented by numbers.
        iv. Text in numbers: each letter is represented by a number.
        v. Images and video
            a. Produced by pixels
            b. Each pixel has a color
            c. Each color is represented by a number
        vi. Sound
            a. These are vibrations or waves
            b. A wave when graphed can be, at any point, assigned and represented by a number
            c. The more bits in a sound, the better its quality, becaue there are more numbers assigned to the wave.

    B. Circuits and Logic: Limor and Nat

        i. Circuits: millions of electronic components
        ii. The simplest circuit takes an electrical signal and flips it from on to off and vice versa, so if the input is a 1, the circuit gives you a 0. This is the "not" cirucit, because you do NOT get out what you put in.
        iii. More complicated cirucits can handle multiple signals and combine them to produce a different result. 
            a. Eg., a circuit can receive two signals simultaneously, a 1 and a 0, producing a 0. 
            b. This ciruit will produce a 1 if both inputs are a 1. 
            c. This one is call "and". 
        iv. There are many small circuits that perform simple logical calculations
        v. By connecting these circuits togther, we can produce complex circuits that perform complex calculations. 
            a. Eg. combining two bits together to form a circuit called an "adder"
            b. This one takes in 2 bits, adds them together and produces a sum
            c. 0+0=0, 0+1=1, 1+1=2
            d. The output requires two wires exiting the circuit to represent the sum
            e. These adders can be grouped to process much larger sums.
        vi. The computer does lots and lots of small mathematical operations very quickly
        vii. Why are smaller computers (microchips) faster?
            a. less distance for the signal to travel
            b. electricty moves at almost the speed of light

IV. Madison, smart-fabric designer; Danielle, founder of Othermachine Company

    A. How input is transformed from physical to binary
        i. The letter b on the keyboard: is converted to a number when you press it
        ii. That binary number is sent into the computer.
        iii. The CPU calculates how to display this number on the screen pixel by pixel.
        iv. The CPU requests step-by-step instructions from the memory
        v. The CPU runs the instructions and transfers the result in pixels back to the memory.
        vi. The pixel info is sent as binary info to the screen.
        vii. The screen converts the output into what you see (RGB)
        viii. The pressing of a key and its display on the screen is the result of thousands of instructions

V. Hardware and Software: Erica, engineering manager at Amazon; Jerome, program manager at xbox

    A. Hardware: the physical components that make up your computer
    B. Software: the code or programs that run on a machine
    C. How they interact with each other
        i. CPU
            a. has circuits for doing logic and math and for sending and receiving
            b. it uses commands to determine which curcuits to use (e.g., the add command triggers the add curcuit)
        ii. binary code is the most basic form of software and controls all of the hardware of a computer
        iii. Nobody now writes software in binary, because it would take too long
    D. Today's code look a lot like english
    E. A high-level command written in today's coding languages is converted into thousands of binary commands 
    F. The operating system, with Bill Gates
        i. controls all the other software on a computer
        ii. Determines whether a program can access the computer's input and output devices.
        iii. Switches among all the programs that you're running, meaning that you're only running one program at a time, technically speaking. 
    G. You make a computer smart. 

[<--home-->](../README.md)