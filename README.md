## Sonic Pi Scheme of Work

![](sonic-pi.png)

###Introduction

[Sonic Pi](http://www.cl.cam.ac.uk/projects/raspberrypi/sonicpi/) is an open source programming environment developed by Dr Sam Aaron, designed to explore and teach programming concepts through the process of creating new sounds. This is a scheme of work which emphasises the importance of creativity in the learning process and gives users the control to turn their sonic ideas into reality.

This scheme of work is specifically targetted towards introductory KS3 Computer Science. This has been developed in harmony with the new Computing curriculum in the UK. This scheme of work is the result of a close collaboration between Computing & ICT teachers and researchers at the University of Cambridge. It has been successfully trialled at a number of schools.

###Students will learn:

Over the course of six lessons, students will learn:

- What a Raspberry Pi is, what are it's main features, and how to setup and use one.
- How to write text based code to produce a music track.
- Computer Science concepts:
	- Sequencing
	- Debugging
	- Iteration
	- Conditionals
	- Data Structures
	- Algorithms
	- Functions
	- Concurrency

# Getting Set Up!

##Step 1: Do you have a GitHub account?

Make sure that you have signed up for [GitHub here](https://github.com/). You should use you school email account and your username should match. eg (email: jsmith1234@sohamcollege.org.uk username: jsmith1234)
##Step 2: Make a copy of this *repository*

A repository is a type of folder on github. Making a copy of a respoistory is called **forking**. Click on the 'Fork' button at the top of the screen on the right hand side, and a copy of everything in this respoitory called **change-code-task** will appear in your account.

![](forking.png)

##Step 3: Locate the code!

Now navigate back to your account and find the starter code called **code.rb**. The code will look like this but will be in a text file:

````ruby
define :drums do
  sample :drum_heavy_kick, rate: 0.75
  sleep 0.5
  sample :drum_heavy_kick
  sleep 0.5
end

define :synths do
  use_synth :mod_pulse
  use_synth_defaults amp: 1, mod_range: 15, attack: 0.03, release: 0.6, cutoff: 80, pulse_width: 0.2, mod_rate: 4
  play 30
  sleep 0.25
  play 38
  sleep 0.25
end

in_thread(:drums){loop{drums}}
in_thread(:synths){loop{synths}}
````

##Step 4: Copy the code to your Raspberry Pi

Next you will want to transfer the text file containing the code from your computer to your Raspberry Pi. You can use the **copy to clipboard** button to copy and paste the code into a text file on your computer, or you can download the entire repository using the **download zip** button. Once you have file containing the code, transfer it to a Raspberry Pi using a removable storage device such as a usb memory stick.

##Step 5: Change the code

Open the text file on your Raspberry Pi and copy and paste the code into Sonic-Pi. Change this code to make it more interesting in any way that you like. It is now your version of **code.rb**. When you have finished your code, copy and paste it back into a text file and save it onto the usb memory stick.

##Step 6: Upload the changed code to Github

The easiest way for you to do this without having to use the command line is to open the file on github by clicking on the **code.rb** file in your forked repository. (Not our original!) Then click on **edit**. You can then paste your new code over the top. To save your code you need to **commit** it to the repository. You will notice that there is a comment box in which you can give a description to the code that you have changed. Add an explanantion here and then click on **Commit Changes**.

![](commit.png)

##Step 7: Share and Comment

Follow [Sam](http://github.com/samaaron) or [Carrie Anne](http://github.com/missphilbin) and anyone else from the project. Then you will be able to see their forked repositories and their changed versions of code.rb

You can comment on their work and give feedback by navigating to their forked respository and then clicking on the **issues** button on the right hand side of the screen. The icon looks like an exclamation mark in a circle. Then you can fill out a comment box and submit it. 

![](issues.png)

##Step 8: Learn more about GitHub in Education

You can learn more about how to use [GitHub in Education here](https://education.github.com/guide). Including steps on administrating accounts for students. 





## Licence

Unless otherwise specified, everything in this repository is covered by the following licence:

![Creative Commons License](http://i.creativecommons.org/l/by-sa/4.0/88x31.png)

***Sonic Pi Lessons*** by the [Raspberry Pi Foundation](http://raspberrypi.org) is licenced under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).

Based on a work at https://github.com/raspberrypilearning/sonic-pi-lessons
