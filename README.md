# Overview
DO NOT EDIT SOURCE CODE IN THIS LAB EXCEPT WHERE EXPLICITLY INSTRUCTED

You will be submitting line numbers as answers to quiz questions - if at any point you think you might have altered your lines, check with your demonstrator or tutor.

In this lab you are going to work on code you should be familiar with from the previous weeks labs.

Results for this week will be submitted on Moodle to Week 4 Lab 4.1 Results.

You will have two sets of exercises:
* Basic tests of your debugger knowledge to show you can execute basic functions 
* More challenging work to find the specific locations of lines of code causing JUnit tests to fail

## Setup
* Fork oose_05_find_bug
* Clone yourself a copy 
* Open in your IDE
* Open the moodle quiz to record answers as you work through this lab https://moodle.gla.ac.uk/mod/quiz/view.php?id=3486311
 - note there is no GitLab submission this week and no need to add demonstrators as developers to your repository this week

## Debugging Basics
* For each of the following, debug by running the main method in BlackJack.java
* Make sure you run in debug mode so your breakpoints are observed
* If you can't see an option to run the main method you want to use, look in the "Debug Configurations..." option below that


### Q1. Warnings
* Find the class which is importing HashMap and not making use of it then enter the class name into Q1 on Moodle.

### Q2. Stack Traces
* Set a breakpoint on line 70 of BlackJack.java
* Run BlackJack main - when prompted, give the username as bob and the value 2 for number of players
* An error should occur and create a stack trace for you to inspect before the breakpoint
* There is a single mistake on a single line of code that you need to add a -1 to
THIS ISSUE MUST BE FIXED BEFORE CONTINUING - GET HELP IF YOU CAN'T FIX IT


### Q3. Breakpoints and Variable Inspection
* Run BlackJack main - when prompted, give the username bob and the value 2 for number of players
* What name does the player have when the breakpoint on line 70 is hit?

### Q4. Stepping In
* Carrying on from the hitting the debug point on line 70...
* (If you already stopped the process run BlackJack main - when prompted, give the username bob and the value 2 for number of players)
* Step into the code twice
* What class do you end up in?

### Q5. Setting a watchpoint
* Set a watchpoint on the variable maxscore in BlackJack.java
* Run BlackJack main - when prompted, give the username bob and the value 2 for number of players
* What is the SECOND line of code to access maxscore? (This should include the initialisation of the variable)

## Debugging with Unit Tests and Debugger
Now you have the basics of using a debugger, it's time to apply those skills to identifying some harder to find issues.

### Q6. Player Name
* Find the class and line of code responsible for the name of the player not being bob. 

Run the JUnit tests on your code.

### Q7. JUnit Test Failure getScoreAceLow 
* Which class/line of code contains the mistake that is causing the getScoreAceLow test to fail?

### Q8. Wildcard mistake
* There is a final, single line of code somewhere in the project sometimes causes an error 
* Hints: 1) the bug has not shown itself yet but happens with certain console input and 2) the bug does not  relate to unimplemented functionality - it is a feature of the code that is not working correctly becasue there is a single line of code that has been written in a way that does not conform to the rules outlined to the user
* Use debugging to identify the error
* Find the class and line of code that is responsible for the mistake  

 

