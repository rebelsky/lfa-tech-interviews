---
title: "EBoard 09: Practice interviews"
number: 9
section: eboards
held: 2023-10-31
link: true
---
# {{ page.title }}

_Approximate overview_

* Administrivia
* About prereg
* Practice interviews

Administrivia
-------------

* Happy halloween!
    * Candy at the back of the room.
* Today is a different day; I thought we'd use some class time for
  interviews and some other things.

About preregistration
---------------------

### Some numbers

We have about 

* 60 CS majors in the class of 2024, 
* 80 CS majors in the class of 2025, and 
* 50 students in the two sections of CSC-207 this semester (most of whom are likely CS majors). 

That's approximately 190 people who might need seats in 200- and 300-level 
CS classes in the spring. 

* Some people (seniors) need two classes. 
* We have some mid-year graduates.
* Some third-years are studying abroad. 
* Some of the 207 students are third-years. 

I think the numbers balance out. Maybe that's 180 people who need seats.

Our spring offerings (after hiring two two-course visitors)

* CSC-211 (24), 
* CSC-301 (2 x 20), 
* CSC-324 (2 x 20), 
* CSC-341 (2 x 20), and 
* CSC-395 (2 x 20). 

That gives 184 seats. 

So things are tight.  If things work out, everyone will get one upper-level
CS course (except for a few seniors who need two courses, who will get two).

It sounds like one of the sections of CSC-395 won't be approved
before rounds 1/2.  That means that some people who try to register
for an upper-level CS class will be closed out.

I don't know how we're handling the second section of CSC-395.

"Don't blame me, I'm only the messenger."

### Questions

Is round 3 first-come, first-served?

> Yes, at least as I understand it.  However, it is "seniors, first-come,
  first-served" on Friday.  Then "third-years, first-come, first-served"
  on Monday.  Then second years.  Then first years.

What are the prereqs for the new CSC-395 on game programming?

> I think it's CSC-207 + (MAT/CSC-208 or MAT-218)

How does this new system work?

> See the Web site.

Peer interview time
-------------------

Everyone has a card.  If you have a red card, grab a red sheet.  If
you have a black card, grab a black sheet.

Find your card partner.

Spend five minutes reading your sheet so that you know the questions
that you will be asking.

Spend black will spend twenty minutes interviewing red.

Red will spend twenty minutes interviewing black.

We will debrief afterwards.

Red questions
-------------

1. `sum-nested-number-list`

2. "compress space"

Black questions
---------------

1. Test sorting

2. Improved merge sort

Debrief on questions
--------------------

### Sum of nested number list

What questions did you ask?

* Do we have to deal with non-numbers?  No.
* Can we look at some examples?
* How deep is the nesting?  Arbitrary.
* What do lists look like in Python?
* I'm not quite sure what to do in this case; any advice?
* Can the list be empty?
* Can I solve it in Scheme first?

How did you solve it?

```
(define nnl-sum
  (lambda (nnl)
    (if (number? nnl)
        nnl
        (reduce + (map nnl-sum nnl)))))
```

In Python

```
def nnl-sum(nnl):
  if type(nnl) == list:
    int sum = 0;
    for val in nnl:
      sum += nnl-sum(val)
    return sum
  else
    return nnl
```

### Test sorting

What questions did you ask?

* What types should we deal with?  What are we sorting?  Answer: Any types.
  (The answer could have been: "For simplicity, let's assume you're sorting integers.")
* Do we have to deal with heterogeneous array?  No.
* Are we dealing with arrays or lists or ...?  Assume you're dealing with arrays.
* What is the signature of the sort method?
* Does the sorting method have to deal with duplicate elements?
* Is the sorting method supposed to be stable?
    * A stable sorting method preserves the order of "equal" elements.  
      For example, if we sort people by first name and then sort again by
      last name, we know that the "Amy Smith" will precede "Bill Smith".
* Does the sorting method have to deal with empty arrays (lists/...)

What did you write as your tests?

* Specific tests in code.
* Tests in English.  "I'd test the empty list, a list of all identical elements,
  a list of mostly different elements with a few differences, some in reverse
  order, ..."

* Did you write something that generates tests?
* Did you write something that does comprehensive testing?
* Did you write something that does randomized testing?
    * Generate a sorted array.
    * Make a copy and permute it.
    * Sort the new copy.
    * Compare to the original.

### Compress space

What questions did you ask?

* Can I have an example?

What approaches did you come up with?

### Improved merge sort

What questions did you ask?

* What is mostly sorted?  "That's a good question.  What do you think it means?"

How hard was it to implement?
