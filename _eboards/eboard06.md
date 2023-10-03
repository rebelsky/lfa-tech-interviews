---
title: "EBoard 06: Exponent and Preamp (and Debugging)"
number: 6
section: eboards
held: 2023-10-03
link: true
---
# {{ page.title }}

_Approximate overview_

* Administrivia
* Exponent and Pramp
    * Overview from Dr. Barks
    * Discussion of your experiences
    * Side notes: Intellectual property
* Steps for success, revisited
* Reflections on practice (or non-practice) interviews, if there were any
* Debugging strategies (if time)

Administrivia
-------------

* Attendance.
* As you've likely discovered, my plans for the course have not quite
  matched what is actually happening.
    * The best laid plans o' mice and men gang aft agley
    * I hope that you're still finding what we do valuable.
* Depending on what next week's alum plans, I'll probably send you some
  pairings and questions to do practice interviews.

Exponent and Pramp: Some Background
-----------------------------------

Welcome to Sarah Barks from CLS

* Directs the STEM Learning Community.
* Responsible for helping people get jobs in tech, data science, plus 
  those other STEM subjects (except for health sciences)
* Unfortunately, they cannot run a mock tech interview for you; they are 
  not a coder.
* Exponent helps prepare you for tech interviews.
    * Courses
    * Sample interviews you can watch
    * Practice questions
    * Etc.
* Also a question bank: Real questions that companies have asked.
    * Helps with inside knowledge.
* Connects you to peers to do mock interviews.
* There's an extra feature that lets you pay to do a real mock interview.
* Seems like a nice "all in one package".

How big is the question bank?

* They claim 2424.
* It's not all tech stuff.
* We will have an event with Exponent on October 26 at 7pm on Webex.
    * It's on Handshake
    * It will also be on career.grinnell.edu
    * It will be recorded

Is a "mock tech interview" one in which you mock technology?

* "Can you believe that the designers at Microsoft are so incompetent
  that ..."
* No.  
* In reality, it's a practice interview to help make you better in prepartion
  for your real interview.

What's Handshake?

* A platform that CLS uses as a job board and as a scheduling platform.
* <https://grinnell.joinhandshake.com/login>
* Handshake vets each job on handshake.
* LinkedIn will also give you jobs, but they are for all levels.
* The more you give your data freely to Handshake and LinkedIn, the more
  they give you back.
* Dice is also good.  Once again, not vetted.
* Data Jobs.
* Tech Crunch.

Back to Exponent

* This year is a trial.  Please try it out and let Dr. Barks know what
  you think.

Experiences with Exponent and Pramp
-----------------------------------

Lessons and Courses

* There are sample solutions.
* Videos may be helpful as well.
* There are classes on what to do once you have the offer or once you're
  in the work environment.
    * Advisors in the CLS will also talk to you about negotiating offers
      (salary, benefits, etc.)
    * It's good to get info from a variety of areas.
    * Don't forget about GlassDoor as a way to check current salaries.
    * Exponent seems to be a vetted source.
    * Historically, places will lowball people from historically
      underserved groups.
    * Once they've made you an offer, they've decided they want you.
      It's fine to negotiate.
* Seems to have courses targeted toward a wide variety of areas.
* Certificates might be useful for those who didn't pursue a CS major
  or who are early in their careers.  Tells employers that you have
  skills that they can trust.

Pramp

* Part of exponent, but something different.
* A channel through which you can connect with someone elsewhere to do
  a practice interview.
    * We hope that you're at the same interview.
* Answering questions for people you don't know is a good way to
  to practice for real interview, which will be someone you don't know.
* Perhaps it's easier to get things wrong in front of someone you don't
  know.

Coaching

* You can apply for CLS professional funding.
* You could also consider our friend Anthony D. Mays

Tell us about CLS funding

* CLS has lots of funding sources.
* There is internship funding for people who have UNPAID internships
  (or a stipend that ends up being less than minimum wage).
    * Unpaid internships should be at non-profits.
    * For-profit companies should be paying you.
* There is professional development funding
    * Certification
    * Professional conferences
* There is also a professional attire grant
* And a CLS clothing closet (basement of the JCC, by appointment)
* Senior interview grant (travel to job interview or grad school)
* Grad program application feeds, test prep, etc.
* See details at career.grinnell.edu
* In general, higher need students get more funding
* "Spend our money, it's there for you."
* But it's limited.  E.g., our professional development funding is limited
  to something like $500.
* Use it or you lose it.

What resources are available to alumni?

* You can still meet with CLS advisors.
* Alumni are welcome to attend on-campus events.
* Alumni can attend virtual meetings.

What are your favorite resume questions?

> Why aren't the apostrophes in resume?

> How do you set a right tab?

Should you have a gpa on a resume?

> It's optional.  It's subjective.  Most employers don't care.

> Most want to see the skills you have.  What will you do for them.

IP and Exponent
---------------

Is it ethical to post the question you were asked on an interview?

> Yes.

> No.

> It depends.  What did the company say about the interview?  Many
  say "Don't discuss your interview questions with other people."

> Privilege is at play.

Steps for Success, revisited
----------------------------

* I'll use [the schedule](../schedule) as our starting point.

Testing example: Determine if a string of all lowercase letters is a permutation of a palindrome (it contains nothing other than lowercase letters; no spaces)

Let's look at some examples.

* Palindomes should be permutations of palindromes

        pp("abccba") -> true (1)
        pp("abcba") -> true (1)

* Permutations of those should be permutations of palindromes

        pp("aabbcc") -> true(1)
        pp("aabbc") -> true(1)

* Some things that are not permutations of palindromes

        pp("abdcba") -> false (0)
        pp("ab") -> false (0)

* We can turn those to printfs at the end.

        int pp(char *str) {
          // Build an array of counters
          int counts[26];
          // The following may not be necessary in many implementations
          // of C, which will zero out memory for safety.  But Sam is old.
          for (int i = 0; i < 25; i++) {
            counts[i] = 0;
          }

          // Add to the counts
          while (*str) {
            int pos = *str - 'a';
            if ((pos >= 0) && (pos < 25)) {
              counts[pos]++;
            }
            str++;
          } // while

          // Make sure all the counts are even
          for (int i = 0; i < 25; i++) {
            if (counts[i] % 2 == 1)
              return false;
          } // for

          // If we made it this far, they are all even
          return true;
        } // pp
          
        int main(int argc, char *argv[]) {
          printf("abccba: %d\n", pp("abccba"));
          printf("abcba: %d\n", pp("abcba"));
        }

Reflections on interviews
-------------------------

Behavioral interview

* 30 minutes long (it feels long)
* Let's talk about your resume.
* What conflicts do you have and how do you resolve that?
* How do you keep up with what's current with tech?
* Recommendations: Practice on these, keep eye contact, ...
* How do you react in team settings?
* What do you do when you have a difficult teammate?
* Use the STAR (Situation, Task, Action, Result) approach.
* Prepare stories ahead.

Technical interview (60 minutes)

* Also included some behavioral questions
* System design, very open ended, not many parameters, not many
  constraints.
* Limited options: Python or Javascript (no advance warning).
* Debugging: Solve using print statements.

BBM Technical Interviews

* Done on shared coding platform.
* Interviewer walks you through the question.
* Follows the "traditional" interview process we talked about (you
  should be asking questions, etc.)
* Practice decreases stress.

Behavioral interviews

* Similar questions
* Also "What do you do outside of CS?"

Debugging strategies
--------------------

_If we have time._
