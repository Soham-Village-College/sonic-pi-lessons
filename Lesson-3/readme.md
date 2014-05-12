# Lesson 3 - Conditionals & Randomisation

##Introduction

If we want to make some meaningful and interesting musical structures, we need to learn some meaningful and interesting programming structures.

## Learning Objectives

- Know that computer programs can make decisions, and that a simple form of decision is called a conditional.
- Understand that computer programs can contain random acts.
- Be able to use comments to explain interesting parts of a program.

## Learning Outcomes

###All students will be able to:

- Play a random note.
- Use an `if` statement.
- Place a comment in their code.

###Most students will be able to:

- Play random notes with varying randomness (by supplying a different argument to `rand`).
- Write useful comments.
- Modify code in the `if` branches to create different execution paths.

###Some students will be able to:

- Use `rand` to sleep for a random amount of time.
- Understand that using `rand` as a test with `<` allows for different probability distributions other than 50/50.
- Nest `if` statements inside other `if` statements.
- Understand that comments are about communicating intent.

##Lesson Summary

-  Simple use of randomisation.
-  Using conditionals to make decisions.
-  Combining randomisation and conditionals. 
-  Comments as a programming tool.

##Starter

Connect your Raspberry Pi in pairs and open the Sonic-Pi Application, can you recall how we used loops to save time coding? Why did we do this, what's the alternative?

##Activity 1

1. We can use randomisation to change the behaviour of our code, making it unpredicable. Try running the code below, what do you think it does? Can you describe it after the # symbol. The # symbol makes the computer ignore that line, it can be used to describe what is happening.

	```ruby
	#
	3.times do
	  play 60 + rand(10)
	  sleep 0.5
	end
	```
	Invite the pupils to observe the actual number of the note played in the output window.

###If Statement
We can use another programming concept to control the program flow, the *if* command allows our program to take descisions. It asks a question and does a different thing depending on the answer to the question.

##Activity 2 
Copy the following code into your sonic pi window and see what it does. make sure you
	```ruby
	if rand < 0.5
      play 60
	  sleep 0.5
	  play 62 
	else       #Explain what else does
      play 72
      sleep 0.25
      play 71
      sleep 0.25
      play 70
	end        #Why do we need this end command?
	```

###Can you make the code above loop?
###Can you adapt the code to make one note play more often than the other?
###Can you make it randomly play 1 of 3 notes? (hint: try using "else if")




## Plenary

We've done a little bit of commenting in today's lesson. Here's an exmaple of how we might use comments to explain our code.


```ruby
# Toss a virtual coin 
if rand(1) < 0.5
# if heads, play two ascending notes
  play 60
  sleep 0.5
  play 62
else
  # if tails, play three descending notes
  play 72
  sleep 0.25
  play 71
  sleep 0.25
  play 70
end
```
##Challenge
Can you combine all we've learnt so far into your own composition. Try to include:

Play note
sleep
sample
loops
randomisation
if statements

There are no rules! If just has to sound good!
