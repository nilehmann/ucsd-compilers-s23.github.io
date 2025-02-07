---
layout: page
title: "Compiler Construction – CSE 131 F19"
doodle: "/doodle.jpg"
---

# Compiler Construction (Spring 2023 Edition)

- <a href="https://jpolitz.github.io">Joe Gibbs Politz</a> (Instructor)
- FILL staff

<p>
<a href="#basics">Basics</a> -
<a href="#schedule">Schedule</a> -
<a href="#staff">Staff &amp; Resources</a> -
<a href="#grading">Grading</a> -
<a href="#policies">Policies</a>
</p>

In this course, we'll explore the implementation of **compilers**: programs that
transform source programs into other useful, executable forms. This will
include understanding syntax and its structure, checking for and representing
errors in programs, writing programs that generate code, and the interaction
of generated code with a runtime system.

We will explore these topics interactively in lecure, you will implement
an increasingly sophisticated series of compilers throughout the course to
learn how different language features are compiled, and you will think
through design challenges based on what you learn from implementation.

This web page serves as the main source of announcements and resources for the
course, as well as the syllabus.

<a id="basics"></a>
## Basics

- Lecture: [Catalyst 0125](https://map.concept3d.com/?id=1005#!m/576554), 12:00-12:50pm (noon) Mon/Wed/Fri
- Discussion Section: [SOLIS 107](https://blink.ucsd.edu/sponsor/advancement/advancement-services/stewardship/named-buildings/solis-hall.html), 4:00-4:50pm Friday
- Tests **(in Friday Discussion Section)**: May 5 (Week 5), June 2 (Week 9)
- Final Exam: Wed June 14, 11:30-2:30, Location TBD

- Podcasts: Coming soon
- Q&A Forum: Coming soon
- Gradescope: <a href="https://www.gradescope.com">https://www.gradescope.com</a> will be used for submissions (instructions will accompany the first programming assignment)
- Textbook/readings: There's no official textbook, but we will link to
  different online resources for you to read to supplement lecture. Versions
  of this course have been taught at several universities, so sometimes I'll
  link to those instructors' materials as well. Some useful resources are:
  - [The Rust Book](https://doc.rust-lang.org/book/) (also [with embedded quizzes](https://rust-book.cs.brown.edu/))
  - [An Incremental Approach to Compiler Construction](http://scheme2006.cs.uchicago.edu/11-ghuloum.pdf)
  - [UMich EECS483](https://maxsnew.com/teaching/eecs-483-fa22/)
  - [Northeastern CS4410](https://courses.ccs.neu.edu/cs4410/)


<a id="schedule"></a>
## Schedule

The schedule below outlines topics, due dates, and links to assignments. The
schedule of lecture topics might change slightly, but I post a general plan so
you can know roughly where we are headed.

The typical due dates are that **assignments** are due on Tuesday evenings and
**quizzes** are due Sunday evenings.

**Week 1 - Rust and Source to Assembly Conversion**

- [Assignment (due Tuesday, April 11, 10pm)](/week1/){:target="_blank"}
- Reading and resources:
  - [Rust Book Chapters 1-6](https://doc.rust-lang.org/book){:target="_blank"}
  - [x86-64 quick reference (Stanford)](https://web.stanford.edu/class/archive/cs/cs107/cs107.1196/guide/x86-64.html){:target="_blank"}
  - [x86-64 quick reference (Brown)](https://cs.brown.edu/courses/cs033/docs/guides/x64_cheatsheet.pdf){:target="_blank"}


<a id="staff"></a>
## Staff & Resources

Office hours are concentrated on Friday, Monday, and Tuesday, since most
assignments are due Tuesday evening. Please check the calendar before you come in
case there have been any changes. When you come to the office hour, we may
ask you to put your name in the queue using the whiteboard. Read the
description about [collaboration below](#policies) for some context about office
hours.



<a id="grading"></a>
## Course Components and Grading

Your grade will be calculated from **engagement**, **assignments**, and **tests**.

**Assignments** are given periodically, typically at one or two week intervals.
FILL grade criteria

There are two **tests** in the course, one in week 5 and one in week 9, given
in the Friday discussion sections. Tests get one of three scores: **High
Pass**, **Pass**, and **No Pass**. FILL grade criteria

**Engagement** has two components – class participation and weekly (p)review
quizzes. Most lectures will come with a 1-2 page handout, and you can submit
the handout any time up until the start of the next lecture. Credit is given
for reasonable effort in engaging with the notes from the day on the handout.
Quizzes will release each week around Wednesday, and be due Sunday evening.
These serve as a review of the past week and a preview of the coming week. You
get credit for a quiz by getting most of the questions right. **Engagement** is
used to add +/- modifiers at the end of the quarter, and won't make the
difference between A/B/C etc.

<a id="policies"></a>
## Policies

### Programming

In your professional programming life, some of your work will be highly
collaborative with lots of expert advice available from senior developers and
from sites like StackOverflow. This is a common case in many Web-focused
companies, in academia, and on open-source projects. It’s a great way to get
exposed to new techniques, share knowledge, and generally enjoy teamwork. In
contrast, some of your work will involve figuring out programming problems on
your own, where you are the first person to encounter an issue, or the first
person to try using a new library in the context of your application. You
should get experience in both types of situations; we might call the former
kind of process **open to collaboration** and the latter **closed to
collaboration**.

In terms of courses, this split also makes sense. Programming assignments
serve (at least) two roles. First and foremost, they are a mechanism for you
to learn! By directly applying the techniques and skills we discuss in class,
you get practice and become a better programmer. Second, they are an
assessment mechanism – as instructional staff we use them to evaluate your
understanding of concepts as demonstrated by your programs. Open
collaboration can reduce frustration while learning and give you chances to
enjoy collaboration and lots of help, but may not let us accurately evaluate
your understanding. Closed assignments are an opportunity for you to
demonstrate what you know by way of programming (and some of the frustration
of working through a problem on your own is _healthy_ frustration).

There are two types of assignments in this course:

- **Open collaboration** assignments, for which you can talk to anyone else in the
  course, post snippets of code online, get lots of help from TAs, and
  generally come up with solutions collaboratively. TAs will be happy to look
  at your code and suggest fixes, along with explaining them. There are a few
  restrictions:
  - Any code that you didn't write must be cited in the README file that goes
    along with your submission
      - **Example:** On an open collaboration assignment, you and another
        student chat online about the solution, you figure out a particular
        helper method together. Your README should say “The FOO function was
        developed in collaboration with Firstname Lastname”
      - **Example:** On an open collaboration assignment, a student posts the
        compilation strategy they used to handle a type of expression you were
        struggling with. Your README should say “I used the code from
        the forum post at [link]”
  - Anyone you work with in-person must be noted in your README
      - **Example:** You and another student sit next to each other in the lab,
        and point out mistakes and errors to one another as you work through
        the assignment. As a result, your solutions are substantially similar.
        Your README should say “I collaborated with Firstname Lastname to
        develop my solution.”
  - You cannot share an entire repository of code or paste an entire solution
    into a message board. Keep snippets to reasonable, descriptive chunks of
    code; think a dozen lines or so to get the point across.
  - You still _cannot_ use code that you find online, or get assistance or code
    from students outside of this offering of the class. All the code that is
    handed in should be developed by you or someone in the class.

  This doesn’t mean the staff will be handing out answers. We’ll mostly
  respond with leading questions and advice, and you shouldn’t expect a
  direct answer to questions like “am I done?” or “is my code right?”

  There is no guarantee the assistance you get from your classmates is
  correct. It is your responsibility to use your judgment to avoid using an
  idea on the course message board that is wrong, or doesn’t work with your
  solution; we won’t necessarily tell you one way or another while the
  assignment is out.

  If we see that you used code from other students and didn’t cite it in
  the README, the penalty will range from a point deduction to an academic
  integrity violation, depending on the severity. Always cite your work!

- **Closed collaboration** assignments, where you cannot collaborate with others.
  You can ask clarification questions as private posts or of TAs.
  However, TAs will not look at your code or comment on it. Lab/office hours
  these weeks are for conceptual questions or for questions about past
  assignments only, no code assistance. On these assignments:
    - You cannot look at or use anyone else's code
    - You cannot discuss the assignment with other students
    - You cannot post publicly about the assignment on the course message
      board (or on social media or other forums). Of course, you can still
      post questions about material from lecture or past assignments!
    - All of the examples in the open collaboration section above would be
      academic integrity violations on a closed collaboration assignment

Programming assignments will explicitly list whether they are open or closed
collaboration.

You should be familiar with [the UCSD
guidelines](http://senate.ucsd.edu/Operating-Procedures/Senate-Manual/Appendices/2)
on academic integrity as well.

### Late Work

Late work is generally not accepted, because often we'll release partial or
full solutions immediately following the deadline for an assignment.
Opportunities for making up missed credit are given in other ways, and will be
described throughout the quarter.

### Regrades

Mistakes occur in grading. Once grades are posted for an assignment, we will
allow a short period for you to request a fix (announced along with grade
release). If you don't make a request in the given period, the grade you were
initially given is final.


### Exams

There will be two tests during the quarter (held in discussion section) and a
final exam. There are no make-up tests for the tests during the quarter.
However, the final exam will have sections that correspond to each of the
in-class tests, and if your score on that part of the final is higher than
your score on that in-class test, the exam score replaces it. This includes
the case where you miss an in-class test (scoring a 0), but can regain credit
from that part of the final exam. This policy is designed to encourage you to
treat the in-class tests as _learning opportunities_ so that you can study
any mistakes you make and re-apply that knowledge on the final.

In addition, if you score high enough on the tests during the quarter, you can
skip the final exam with no penalty and just have the test grades applied as
your exam score.

You are not allowed any study aids on exams, aside from those pertaining to
university-approved accommodations. References will be provided along with
exams to avoid unnecessary memorization.

You cannot discuss the content of exams with others in the course until grades
have been released for that exam.

Some past exams are available at the link below for reference on format
(content changes from offering to offering so this may not be
representative):

https://drive.google.com/drive/folders/1yPxZ-nqRpC9Gz63JIavhQgfnyhA0uGIs?usp=sharing

### Laptop/Device Policy in Lecture

There are lots of great reasons to have a laptop, tablet, or phone open
during class. You might be taking notes, getting a photo of an important
moment on the board, trying out a program that we're developing together, and
so on. The main issue with screens and technology in the classroom isn't your
own distraction (which is your responsibility to manage), it's the
distraction of **other students**. Anyone sitting behind you cannot help but
have your screen in their field of view. Having distracting content on your
screen can really harm their learning experience.

With this in mind, the device policy for the course is that if you have a
screen open, you either:

- Have only content onscreen that's directly related to the current lecture.
- Have unrelated content open and **sit in one of the back two rows of the
room** to mitigate the effects on other students. I may remind you of this
policy if I notice you not following it in class. Note that I really don't
mind if you want to sit in the back and try to multi-task in various ways
while participating in lecture (I may not recommend it, but it's your time!)

### Diversity and Inclusion

We are committed to fostering a learning environment for this course that
supports a diversity of thoughts, perspectives and experiences, and respects
your identities (including race, ethnicity, heritage, gender, sex, class,
sexuality, religion, ability, age, educational background, etc.).  Our goal is
to create a diverse and inclusive learning environment where all students feel
comfortable and can thrive.

Our instructional staff will make a concerted effort to be welcoming and
inclusive to the wide diversity of students in this course.  If there is a way
we can make you feel more included please let one of the course staff know,
either in person, via email/discussion board, or even in a note under the door.
Our learning about diverse perspectives and identities is an ongoing process,
and we welcome your perspectives and input.

We also expect that you, as a student in this course, will honor and respect
your classmates, abiding by the UCSD Principles of Community
(https://ucsd.edu/about/principles.html).  Please understand that others’
backgrounds, perspectives and experiences may be different than your own, and
help us to build an environment where everyone is respected and feels
comfortable.

If you experience any sort of harassment or discrimination, please contact the
instructor as soon as possible.   If you prefer to speak with someone outside
of the course, please contact the Office of Prevention of Harassment and
Discrimination: https://ophd.ucsd.edu/.

