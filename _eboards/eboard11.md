---
title: "EBoard 11: More interview practice"
number: 11
section: eboards
held: 2023-11-14
link: true
---
# {{ page.title }}

_Approximate overview_

* Administrivia
* Activity
* Debrief

Administrivia
-------------

* Next week we'll have a founder of AppDev visiting (remotely).

### Questions

How do I find out about REUs and more?

> CSstudents mailing list.

> Sam has links on [his summer opportunities page](https://rebelsky.cs.grinnell.edu/cs-summer.html)

Activity
--------

* Five minutes of reading and trying to understand the question you will
  ask your partner.  (There's also some prep you may want to do.)
* Twenty minutes of Red Interviews Black.
* Five minutes discussion with each other.  "Here's what you did well."
* Twenty minutes of BLack Interviews Red.
* Five minutes discussion with each other.  "Here's what you did well."
* Back to the main group to debrief.

Debrief
-------

### For the GrinCo problem (also the Waymo problem)

* Intentionally open-ended.  (Perhaps a little too open-ended; I should
  have specified number of cars and the time cost of getting from place
  to place; or perhaps not, since there are bigger issues at play.)
* What are the goals I'm trying to meet?
    * Minimizing average wait time.
    * Minimizing energy use.
    * Maximize "in use time"
    * Maximizing profit.
    * Avoid certain locations.
* "Do you have historical data and how consistent are they?"
    * If you do have historical data and its consistent, your answer might
      be "ML".
         * It would be nice to know what the policies ML comes up with
           are.
    * If they aren't consistent, you need to be a bit more creative in
      designing policy.
* Some ideas worth sharing.
    * How do you decide who to get?  (Assuming only one car available.)
        * Nearest
        * Shortest trip of "here to pickup to destination"
        * The one waiting longest
        * A formula based on all of those.
    * How do you decide which car to send?  (Assuming only one request.)
        * Closest?
    * Where do cars go when they aren't engaged?
        * Designated garages.
        * Distributed
        * To where we expect people.

Elevator problem

* What is the UI for people waiting for the elevator?
    * Up/Down from where I am.
    * I want to go to floor X (only available in the lobby)
    * ???

### For the MegagoogazonbookInc problem
   
Suppose you build a hash table: How do you efficiently
figure out which color each key in the hash table is closest to?

* Think of it as a graph problem.
