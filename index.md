---
title: CIS 421/521 - Artificial Intelligence - University of Pennsylvania
layout: default
img: R2D2.png
active_tab: main_page 
---



<div class="alert alert-danger" markdown="1">
To get a permit for CIS 421/521, you should [sign yourself up for the CIS waitlist](https://forms.cis.upenn.edu/waitlist/index.php) when it opens on April 30.   After you've added yourself to the waitlist, I can issue you a permit.  You will receive an email saying permit available. You will receive another email when the permit is issued. At that point, you may register on CoursesInTouch.   You don't need to email me in order to get a permit.  Permits aren't available during advance registration. 
</div>

<!-- Display an alert about upcoming homework assignments -->
{% capture now %}{{'now' | date: '%s'}}{% endcapture %}
{% for page in site.pages %}
{% if page.release_date and page.due_date %}
{% capture release_date %}{{page.release_date | date: '%s'}}{% endcapture %}
{% capture due_date %}{{page.due_date | date: '%s'}}{% endcapture %}
{% if release_date < now and due_date >= now %}
<div class="alert alert-info">
<a href="{{page.url}}">{{ page.title }}</a> has been released.  
{% if page.deliverables %}
The assignment has multiple deliverables.
<ul>
{% for deliverable in page.deliverables %}
<li>{{ deliverable.due_date | date: "%b %-d, %Y" }} - {{deliverable.description}}.</li>
{% endfor %}
</ul>
{% else %}
It is due before {{ page.due_date | date: "%I:%M%p" }} on {{ page.due_date | date: "%A, %B %-d, %Y" }}.
{% endif %}
</div>
{% endif %}
{% endif %}
{% endfor %}
<!-- End alert for upcoming homework assignments -->



<div class="alert alert-success" markdown="1">
[When you borrow one of the programmable toy R2D2s for the semester, please fill out this Robot Checkout Form.](https://docs.google.com/forms/d/e/1FAIpQLSeVrCvG_2zcb2bPdn0bor61EOTzzqesI748l1pG4u9TqJ_GgQ/viewform?usp=sf_link)
</div>



<div class="alert alert-info" markdown="1">
R2D2 ***Extra Credit*** Assignments (late submission not allowed):
* [Robot Exercise 1: Using Python to Control R2D2](r2d2_assignments/hw1/homework1.html)
* [Robot Exercise 2: Robot Navigation](r2d2_assignments/hw2/homework2.html)
* [Robot Exercise 3: Flag Capture Game using a Minimax Algorithm](r2d2_assignments/hw3/homework3.html)
* [Robot Exercise 4: Commanding Robots with Natural Language](r2d2_assignments/hw4/homework4.html)

Extra Credit Bounty Items:
* ~~Get the Python API that we developed working on Windows~~ (solved by Hanbang with Raspberry Pi)
* Find a way to communicate the robot's gyroscopic sensor info back to Python
* Develop a Python collision detection protocol 
</div>



Course number
: CIS 421/521 - Artificial Intelligence 

Instructor
: [Chris Callison-Burch](https://www.cis.upenn.edu/~ccb/)

Discussion Forum
: [Piazza](http://piazza.com/upenn/fall2019/cis521)

Time and place
: Tuesdays and Thursdays from noon-1:30pm in Wu and Chen Auditorium (Levine Hall room 101)

Office hours
: Monday 3-5pm in GRW 5th Floor Bump Space
: Monday 6-8pm in 268 GRW
: Tuesday 9-10am in GRW 5th Floor Bump Space
: Tuesday 9-11am in GRW 5th Floor Bump Space
: Tuesday 3-4pm in 3401 Walnut room 463C
: Wednesday 2-4pm in GRW 5th Floor Bump Space
: Thursday 9-10am in GRW 5th Floor Bump Space
: Thursday 9-11am in in GRW 5th Floor Bump Space
: Thursday 3-4pm in 3401 Walnut room 463C
: Friday 1:30-3 pm in Moore 100A

Textbooks
: [Artificial Intelligence: A Modern Approach (3rd edition) by Russel and Norvig](https://www.amazon.com/Artificial-Intelligence-Approach-Stuart-Russell/dp/9332543518/)
: [Speech and Language Processing (3rd ed. draft) by Jurafsky and Martin](https://web.stanford.edu/~jurafsky/slp3/)


Grading
: 55% Homework Assignments
: 15% Midterm 1
: 15% Midterm 2
: 15% Midterm 3 <br/>
There is roughly one homework assignment per week, aside from weeks with exams.  Students enrolled in CIS 421 may skip one HW assignment, or they may discard their lowest scoring HW assignment.  You do not get late days back on the homework that you discard.  Students enrolled in CIS 521 must complete all HW assignments and cannot discard their lowest scoring assignment.


Collaboration Policy
: Unless otherwise noted, you are not allowed to work in groups on the homework assignments. You can discuss homework problems with others (you must explicitly list who you discussed problems with on each homework submission), but   *all code must be your own independent work.*  You are not allowed to upload your code to publicly accessible places (like public github repositories), and you are not allowed to access anyone else's code.  If you discover someone else's code online, please report it to the course staff via a private note on Piazza. 


Late Day Policy
: Each student has five free "late days".  Homeworks can be submitted at most two days late.  If you are out of late days, then you will not be able to get credit for subsequent late assignments. One "day" is defined as anytime between 1 second and 24 hours after the homework deadline. The intent of the late day policy it to allow you to take extra time due to unforseen circumstances like illnesses or family emergencies, and for forseeable interruptions like on campus interviewing and religious holidays.  You do not need to ask permission to use your late days.  No additional late days are granted. 

