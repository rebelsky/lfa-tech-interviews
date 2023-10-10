---
title: "EBoard 07: Brainstorming"
number: 7
section: eboards
held: 2023-10-10
link: true
---
# {{ page.title }}

_Approximate overview_

* Administrivia
* Visitor talk(s) 
* Visitor practice interview.
* Reflections on practice (or non-practice) behavioral interviews, 
  if there were any
* Brainstorming strategies (if time)

Administrivia
-------------

Visitor Talk
------------

* Welcome to our visitor!
* Sam has permission to take notes.  But only if he uses vim.
* Graduated in 2017.
* Took old 151.  In the old 151, students scripted the Gimp (an open-source
  version of photoshop).
* Built a DormsDB program.  "A Yelp for dorms."
    * No, PHP is not a good language.
    * JavaScript and MySQL are pretty good things to learn.
* Was part of AppDev, an organization that built applications for campus.
  Menu, other stuff.
* Did some other stuff. 
* Summer research: a functional language for building images.
    * Learned Full Stack development and Node.js
* Like many alums, has trouble remembering some things.
* Managed to get an internship at Google because they knew how to parse
  a Scheme-like language and how to compute from that.  (Magic of getting
  a question on just that topic.)
    * Worked on a single-sign-on app, just like DUO.
* Did Grinnell in London, with an internship.
* Like many alums, has trouble remembering some things.
* Another internship, this time at Nest.
* Followed SO to LA, got a position at Amazon Studios.  Learned React.
* Amazon is everything they say.  Read this as you may.
* Recruited to Riot Games.
* Built a game server deployment tool (e.g., deploy with Kubernetes
  or Docker).
* Got PIPped.  It's on your permanent record.
* Joined high-touch consulting company in 2019.  The benefit of knowing
  people. 0260 (it's almost a zip code).
* Returned to Iowa in Fall of 2019.  Lots of different kinds of consulting.
  Modernization: Cloud and serverless technology.
* The danger of consulting: Clients sometimes stop paying.  If you don't
  have enough clients, you're screwed.
* It is still a rough tech time.

More on the consulting company

* There were lots of doors (and windows?) that opened.
* How do you choose which to do?  Analysis paralysis.
* If you are going into business for yourself, you need to understand
  business (or you have to work with someone who really understands
  business).
* Understand the value of what you're doing; something you can.

AppDev

* A student group on campus that built iOS and Chrome apps.
* Deep organizational infrastructure.

Things recommended:

* Work on projects for yourself.
    * You end up touching every part for yourself.
    * Searching for data can be interesting.  At least if you're
      that kind of person.  Figure out where the hurt is.
* Learn MySQL.
* Learn JavaScript, Learn Node.js, Learn React.
* Learn about the organizational culture of the place that's hiring you.
* Figure out what matters to you.
* Learn how to suck up to faculty while faculty are in the room.
* Watch Silicon Valley on TV.  It's more realistic than you'd think.
  Can help to understand how companies are organized and their
  value proposition.

What was the interview process like?

* Once you get an internship at one of the big companies, people treat you 
  differently.
* Most internships are designed as "path to job".

How do you find customers?

* Fancy gyms.

How do you determine the tech needs of random clients?

* It was often data analysis as a starting point.
* The other co-founder had built a data analysis tool.
* Tried to democratize the tool (more clients, lighter touch).
* Timing issue: Generative AI threw a fork into the plan.
* "It's all fancy stats, but no one understands the stats."
* "You should post THIS TYPE OF CONTENT at THIS TIME because THIS REASON."

Mock interview
--------------

Write a function that takes a string, `s`, and an integer, `k`, that produces
all the strings of length `k` that contains only characters from `s`.

Questions

* Is "aa" part of the result if the input is `fun("abc", 2)`?
    * Interviewer says "yes", Sam says "no".
* Can I return an array of strings?
    * Interviewer says "yes", Sam says "I'd assume you could come up with
      something better than that."

Ideation

* Since it doesn't matter how many times a letter appears in the string
  we'll set up an array that keeps track of which letters appear.  
    * Or maybe a set (hashset?).
* It may be helpful to write a helper function.

Time complexity?

* $$len(s)^k$$?

Space complexity?

Reflections

* Some good early questions to set the stage. [+1]
* Moved to code fairly early.  Are there better ways to talk through your
  ideas?

Reflections on Behavioral Interviews
------------------------------------

Brainstorming Strategies
------------------------

_If there's time._
