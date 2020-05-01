---
layout: essay
type: essay
title: Software Design Patters&#58; <br /><h3><i>The key to building a large software company</i></h3>
date: 2020-04-30
labels:
  - Software Engineering
  - Meteor
  - Ethics
  - Self Driving Cars
  - Design Patterns
---
<h2 style="color: yellow; text-shadow: 2px 2px red">Design patterns can solve many issues facing software teams</h2>
Imagine the boss at a construction site asks a team member to frame a door so the boss can install it.  The team member frames the door, and the next day the boss goes to install the door.  The boss tries to install a door that has two door knobs and three hinges, however, the door frame was only <i>designed</i> for one door knob and two hinges.  This lack of agreement on design patterns would stall the entire project and would require backtracking.  The boss and all team members would need an agreed upon structure for each module and it's dependencies.  We see this in software engineering and we have a name for this, <i>Design Patterns</i>.  The three most important design patterns in my opinion are dependencies between modules, naming, and single responsibility.

<h2 style="color: green">Dependencies Between Modules</h2>
The construction of a home can be dvidided into many modules. One such module could be pouring the cement foundation. Another module could be framing the house.  Another module could be designing the blue prints of the home.  Could you frame the house without the cement foundatoin?  Could you frame it without the blue prints?  You can't because these modules are dependent on eachother.  An ownership graph is a design pattern that is useful to help all team members understand how an app functions so they don't alter and break depedencies between modules.  For example, imagine there is a function called studentShedule.  It requires two parameters, a student ID number and a year.  studentSchedule might be disigned to pull the class schedule from a data file by matching the student ID to the correct section of the data file.  If one of the software engineers weren't completely aware of the ownership graph, they might remove the ID section from the data file.

<h2 style="color: green">Naming</h2>
How long would it take a team of construction workers to build a house if each team member had a different name for a 2x4 board?  How about if each team member had a different name for nails, hammers, saws, etc.  The boss could ask an employee for a nail gun and instead be given a saw.  It would be as if each team member spoke a different language.  What you need is everyone to speak the same language. This relates to variables in coding. There must be a design pattern to naming variables, functions, and classes so they are understood by the other team members.

<h2 style="color: green">Single Responsibility</h2>
Imagine there are three team members building a home. All tasks are divided equally between the three.  One person, Bob, gets sick and dies.  Does the house get finished?  How much arguing would occur between the remaining two team members about why certain tasks weren't completed and who's responsibility they are.  Now imagine there are 100 team members, and each has only one job to do.  Now let's say that same person, Bob, gets sick and dies.  His job was to frame doors, and now no doors are being framed, and the remaining team members want to find out why the doors are not being framed.  They would realize quickly that it was Bob's job to frame the doors and they would fix this issue quickly by hiring a new door framer.  In software, it is best to try and make every class, function, and data files singlely responsible if possible.  For example, say there is a data file created to hold all the supplies needed to build the house.  One typo would create a bug in the entire folder and none of the data would be accesable.  It would be very hard to find the bug.  However if each type of inventory was placed in it's own data file, it would be very easy to identify which file contains the bug and fix it quickly. 
