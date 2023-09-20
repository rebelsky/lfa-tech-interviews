---
title: "EBoard 04: Thinking aloud"
number: 4
section: eboards
held: 2023-09-19
link: true
---
# {{ page.title }}

_Approximate overview_

* Administrivia
* Visitor presentation
* Sample tech interview one
* Sample tech interview two
* Debrief
* Steps for success, revisited (if time)

Administrivia
-------------

* Welcome to our visitor.
    * Our visitor may be doing different questions than I sent out.
      (Don't worry, the voluntolds did not get the questions.)
* Next week: Halle Remash returns to campus (virtually).
* Expect to see the visitor schedule evolve over the next few weeks.
* I may steal a week for a return to "What skills should you practice
  for your technical interview?"

Visitor Presentation
--------------------

_Sam may attempt live notes._

### Background

* Started at Grinnell in 2000.  [Wow, that's a long time ago.]
* Planned to do math.  Took CS on a lark.  Got stuck with SamR.
  151.  Loved it.
* [Snarky comments about other majors.]
* Networked a lot working with people in Noyce late at night.
* Didn't do any internships while at Grinnell.  Did summer research
  in Mathematics in Summer 2003.
* Had no plan when graduating in 2004.
* Faculty member forwarded along an email.  Moved out to California.
  Worked for O'Reilly Media.
* Decided to go to grad school.  Went to Vanderbilt.  Did a Ph.D.
  In Nashville.
* In 2011, started looking for jobs.  Applied to Amazon (job offer),
  Google (rejected), NSA (hired).  
* Worked for the government for two years.  [Learned how to spy on US
  Citizens.]
* Decided to interview with Google again.  Read _Cracking the Coding
  Interview_ this time.
* "Interviewing is a skill.  Like any other skill you can get good at it."
    * It makes all the difference.
    * [Hmmm ... we've heard that before.]
* Four years in Mountain View.  Then got married and moved to Switzerland.
    * Eventually ended up as a manager.
* In March of 2023, laid off.  (The whole division was laid off.)
    * Prepared for managerial interviews.  Came up with 50 or so questions.
        * "Tell us about a time you had difficulty with a team member"
    * Lots of coding practice too.  Decided to interview in Python.
    * 30 minutes per day practicing.  Doing lots of other things.
    * Got an offer in April.  Stayed in Switzerland until June.
* Currently a senior engineering manager.
    * Manages seven people.
    * Does a lot of interviewing / screens.
* Has kids and is about to buy a house.  Yay real life!

### Questions

How did you structure your preparation?
  : Remember: You'll be presented with a problem.  You should never jump
    into the solution right away.  Ask questions.  It shows the interviewer
    that you care about the problem.  It also helps ensure that you are
    thinking about the same problem.
  : Sample problem: "You have to parse a file and extract all the phone
    numbers."
  : Sample questions: 
      * "What kind of file is it?"
      * "Will it fit in memory?"
      * "What do phone numbers look like?"
      * "Do I have to validate that they are real phone numbers?"
  : Make sure to think aloud while you are developing the solution in
    the editor.
  : Be creative in your test cases.  Think about edge cases.
  : In preparing for this set of interviews, wrote a bunch of small questions
    that helped them ensure that they knew the core aspects of Python.
  : "In real life, you can look things up."
  : In technical interviews, there's coding and algorithms.  They were
    pretty sure that the understood the algorithm.

What was your thesis?
  : Robust routing in wireless mesh networks.
  : Never worked on networking again.
  : Some time during grad school, decided that academia wasn't the
    right direction for them.
  : Cared about flexibility in place and work/life balance.

What did you do at Google?
  : For four years, worked on Google Analytics.  They worked on a product
    that told advertisers when someone searched for a product immediately
    after an ad was shown.
  : Worked on the front-end.
  : In 2017, moved to a new team (and a new country).
  : Worked on Google shopping to speed up databases.  His team provided
    data.

What is a workday like?
  : Once they became a manager ...
  : "A lot of meetings."  "More than half of my time is in meetings."
  : A lot of stand-up meetings with two-week sprints.
  : Meetings with other companies (e.g., third-party vendors that are
    doing software as a service).
  : Lots of hiring meetings with candidates.
  : Responding to questions on Slack.
  : Forwarding tickts to the next person.
  : Doing forward planning.  Small company (500-people) planning is 
    very different than Google-size planning.  Small companies have
    to be ready to pivot.

What was working for the NSA like?
  : The interview was mostly background checking (they got a top-secret
    background clearance; it took 4-5 months).
  : Rotated between several (three) different offices.
  : First one: Processing data.  Wrote a lot of Perl scripts and Python
    scripts.
  : Second one: Cloud analytics fusion (CAFe).  Big data store.
  : Third one: "Setting up some database stuff."

How is government different than academia or industry?
  : There's more stability in the job.  "The government doesn't really
    do layoffs."
  : On the other hand, there are fewer perks and smaller salaries.
  : Google has nap pods, free food, buses, and more.
  : Congress doesn't like government offices to spend money that way.
    NSA parking was awful.  Before 7:30 a.m.: 1/4 mile to office. After
    7:30 a.m: 1/2 mile to office.  After 8:00 a.m., "Park on the other
    side of the interstate and wait for the shuttle."
  : But you have a public interest mission rather than a "make money"
    mission.
 
Sample Tech Interview One
-------------------------

_Sam is not recording the question or the work.  Just a few comments._

_There would normally be some introductions and then a short, partially
ambiguous question._

_Note: There are normally stages to a question.  How would you add X to your code?_

Sample Tech Interview Two
-------------------------

_Always start with questions._

_Work through some examples._

_Make sure that you have time to do the algorithm._

_Pause and think through the algorithm._

_Think through your data structures._

_Come up with some test cases/unit tests._

Debrief
-------

### Notes

* Ask for help!
* Think about other directions!
* Clarifying questions are nice way to start things off.
* Don't start coding too early.
* Try to predict what kinds of questions the interviewer might ask
  and then ask them of the interviewer.
* Think about tradeoffs (maintainability and readability)
    * Interviewers expect you to discuss them.
* People care about process as much as the solutions.

### Sam's questions

* Good questions: 
    * What is the format of the input?
    * Should I handle things that are outside.
    * What kind of security do we want?
    * Do I have access to _these data_.
    * What is the return type?
    * Are there naming conventions I should follow?
    * What should I do in _these exceptional situations_?
* They were good at responding to the interviewer's questions and in
  asking their own; there was a conversation.
* They weren't rushing.
* Interesting example: One of the first mars landers crashed because
  of inconsistency in units throughout the program.
* Good at talking about where they are getting stumped.
* Know some strategies.  E.g., "Convert it to a graph and use a graph
  algorithm", "Use dynamic programming", "Use a greedy algorithm"
    * What will the graph look like?
* Criticisms:
    * Don't work with a language you don't know (well).
    * More object thinking!
    * Make sure to discuss the algorithm before coding.
    * Know your data structures/ADTs/algorithms.

Tips

* Know your classes.  There's more than just algorithms and data structures
  in your solutions.  Sometimes you get design problems.
* Learn how to use a mac keyboard.
* Find the right balance of when to jump into the code.
    * You may want to explicitly address that with the interviewer.
    * "Is this the right time to start writing some code?"
* It's okay if you have a bad interview.  Think about how you can give the
  interviewer positive signals.  Keep the momentum going.
* Interviewers may feel like a blank wall; you will likely have to take
  initiative.



Steps for success, revisited
----------------------------

See the [course schedule](../schedule/).

