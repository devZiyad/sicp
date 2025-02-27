# SICP

This repository serves as a progress tracker for the book *Structure and Interpretation of Computer Programs* and Brian Harvey’s CS61A lectures. Over the years, I have attempted to start but never finished. I have faced multiple challenges along the way. Therefore, I dedicate this repository as a starting place to help others and as a personal progress tracker, in the hope that this time I will achieve my goal of finishing both the book and the course.  

Thanks to [teachyourself.cs](https://teachyourselfcs.com/) for introducing me to valuable resources like SICP.  
This repository is heavily influenced by [theurere](https://github.com/theurere)'s [berkeley_cs61a_spring-2011_archive](https://github.com/theurere/berkeley_cs61a_spring-2011_archive) repository and [zackads](https://github.com/zackads)' [sicp](https://github.com/zackads/sicp) repository. Some parts of this repository are directly copied from these sources rather than just being inspired by them.

## Getting Started

### Installing Racket  

[Download Racket](https://download.racket-lang.org/). At the time of this writing (February 2025), I am using version 8.15.  

To use Berkeley-defined functions such as [word](https://docs.racket-lang.org/manual@simply-scheme/#%28form._%28%28lib._simply-scheme%2Fmain..rkt%29._word%29%29) and [sentence](https://docs.racket-lang.org/manual@simply-scheme/#%28form._%28%28lib._simply-scheme%2Fmain..rkt%29._sentence%29%29), as shown in Lecture 1, we need to install the Berkeley package in Racket.  

Originally, as shown in [theurere](https://github.com/theurere)'s [berkeley_cs61a_spring-2011_archive](https://github.com/theurere/berkeley_cs61a_spring-2011_archive) repository, you would run the following command:

```
raco pkg install berkeley
```

However, this no longer works because the URL that `raco` tries to access for the zip archive of the package has been restricted.  
Instead, you can download the archive directly from [here](https://raw.githubusercontent.com/zackads/sicp/refs/heads/main/inst.eecs.berkeley.edu/%7Ecs61as/fa11/lib/berkeley.zip).

After downloading `berkeley.zip`, install it manually by running:

```
raco pkg install berkeley.zip
```

### Verifying the Installation

To test if everything works, open **DrRacket** and paste the following code snippet into the *definitions window*:
```
#lang racket

(require berkeley)

(sentence 'hello 'world)
```

Now, click the "Run" button. In the *interactions window*, you should see the following output:
```
'(hello world)
```

## [Video lectures](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?&sort=-titleSorter) and required corresponding reading from SICP

Readings should be done before lecture series.

1. Functional programming (1.1)
2. Functional programming (1.1)
3. Higher-order procedures (1.3)
4. Higher-order procedures (1.3)
5. User interface Alan Kay (1.3)
6. User interface Alan Kay (1.2.1–4)
7. Orders of growth (1.2.1–4)
8. Recursion and iteration (1.2.1–4)
9. Data abstraction (2.1, 2.2.1)
10. Sequences (2.1, 2.2.1)
11. Example calculator (2.1, 2.2.1)
12. Hierarchical data (2.2.2–3, 2.3.1,3)
13. Hierarchical data (2.2.2–3, 2.3.1,3)
14. Example Scheme (2.2.2–3, 2.3.1,3)
15. No lecture available
16. Generic operators (2.4–2.5.2)
17. Generic operators (2.4–2.5.2)
18. Object-oriented programming ([OOP above line reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/oop_programming_above_line_view.pdf))
19. Object oriented programming ([OOP above line reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/oop_programming_above_line_view.pdf))
20. Object oriented programming ([OOP above line reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/oop_programming_above_line_view.pdf))
21. Assignment and state (3.1, 3.2, [OOP below line reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/oop_programming_below_line_view.pdf))
22. Environments (3.1, 3.2, [OOP below line reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/oop_programming_below_line_view.pdf))
23. Environments (3.1, 3.2, [OOP below line reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/oop_programming_below_line_view.pdf))
24. Mutable data (3.3.1–3)
25. Mutable data (3.3.1–3)
26. Vectors (3.3.1–3)
27. No lecture available
28. No lecture available
29. No lecture available
30. Client-server programming (3.4)
31. Concurrency (3.4)
32. Concurrency (3.4)
33. Streams (3.5.1–3, 3.5.5, [Therac reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/an_investigation_of_therac-25_accidents.pdf))
34. Streams (3.5.1–3, 3.5.5, [Therac reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/an_investigation_of_therac-25_accidents.pdf))
35. Therac-25 (3.5.1–3, 3.5.5, [Therac reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/an_investigation_of_therac-25_accidents.pdf))
36. Metacircular evaluator (4.1.1–6, [MapReduce reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/mapreduce_simplified_data_processing_on_large_clusters.pdf))
37. Metacircular evaluator (4.1.1–6, [MapReduce reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/mapreduce_simplified_data_processing_on_large_clusters.pdf))
38. Mapreduce  (4.1.1–6, [MapReduce reader](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/mapreduce_simplified_data_processing_on_large_clusters.pdf))
39. Mapreduce (4.1.7, 4.2)
40. Analyzing evaluator (4.1.7, 4.2)
41. Lazy evaluator (4.1.7, 4.2)
42. Logic programming (4.4.1–3)
43. Logic programming (4.4.1–3)
44. Review (4.4.1–3)

> **Note:** According to this [source](https://romanbird.github.io/sicp/), no lectures are actually missing. The gaps in numbering (e.g., no Lecture 15, or 27–29) correspond to **half-term breaks and spring breaks**, rather than lost content.

## Course Documents
* Course Book - [Structure and Interpretation of Computer Programs](http://sarabander.github.io/sicp/)
* [Course timetable](https://people.eecs.berkeley.edu/~bh/61a-pages/first-day-handout.pdf#page=18)
* [Course syllabus](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_syllabus.pdf)
* [Homework assignments](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_1/homework_assignments.pdf) ([solutions](https://people.eecs.berkeley.edu/~bh/61a-pages/Solutions/))
* [Lab assignments](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_1/lab_assignments.pdf)
* Projects
  * Project 1 - [Twenty-One](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_1/project_1_twenty-one.pdf) ([code](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/code/projects/project_1_twenty-one/twenty-one.scm))
  * Project 2 - [Section 2.2.4 of SICP](http://sarabander.github.io/sicp/html/2_002e2.xhtml#g_t2_002e2_002e4)
  * Project 3 - [Adventure Game](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_1/project_3_adventure-game.txt) ([code](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/code/projects/project_3_adventure-game))
  * Project 4 - [Logo interpreter](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_1/project_4_logo-interpreter.txt) ([code](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/tree/master/code/projects/project_4_logo-interpreter))
* [Lecture Notes](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/lecture_notes.pdf)
* Sample Exams
  * Midterm 1
    * [Sample Exam 1](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_1/mt1-1.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_1/mt1-1_solutions.txt))
    * [Sample Exam 2](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_1/mt1-2.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_1/mt1-2_solutions.txt))
    * [Sample Exam 3](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_1/mt1-3.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_1/mt1-3_solutions.txt))
  * Midterm 2
    * [Sample Exam 1](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_2/mt2-1.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_2/mt2-1_solutions.txt))
    * [Sample Exam 2](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_2/mt2-2.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_2/mt2-2_solutions.txt))
    * [Sample Exam 3](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_2/mt2-3.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_2/mt2-3_solutions.txt))
  * Midterm 3
    * [Sample Exam 1](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_3/mt3-1.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_3/mt3-1_solutions.txt))
    * [Sample Exam 2](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_3/mt3-2.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_3/mt3-2_solutions.txt))
    * [Sample Exam 3](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_3/mt3-3.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/midterm_3/mt3-3_solutions.txt))
  * Final exam
    * [Sample Exam 1](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/final/f-1.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/final/f-1_solutions.txt))
    * [Sample Exam 2](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/final/f-2.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/final/f-2_solutions.txt))
    * [Sample Exam 3](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/final/f-3.pdf) ([solution](https://github.com/theurere/berkeley_cs61a_spring-2011_archive/blob/master/docs/course_reader_vol_2/sample_exams/final/f-3_solutions.txt))

## Task Tracking

To keep track of progress and manage tasks effectively, You can use Trello. I have created a Trello board template that others can use to organize their own learning journey through SICP and CS61A.  

You can access the Trello template here: **[Trello Board Template](https://trello.com/b/X9AlxWb6/sicp-cs61a-progress-tracker)**.  
Feel free to copy and customize it to fit your needs.

If you prefer to track your progress using Markdown, you can use the **study plan template** I created. It provides a structured way to document your learning journey.  

You can access the Markdown study plan template here: **[Study Plan Template](sicp-cs61a-study-tracker.md)**.

While setting up the study plan, I encountered some difficulties in structuring the weeks. The homework schedule follows a **15 week format**, whereas the syllabus is organized into **14 weeks**. Additionally, different sources suggest slightly different recommended readings, which made it challenging to align everything perfectly. If you notice discrepancies, feel free to adjust the board according to your preferred structure.

---

## Disclaimer

This repository is for **personal educational use** and does not claim ownership over any original course materials from UC Berkeley. Some parts of this repository, including code and resources, are directly copied from publicly available sources, specifically from [theurere](https://github.com/theurere)'s [berkeley_cs61a_spring-2011_archive](https://github.com/theurere/berkeley_cs61a_spring-2011_archive) repository and [zackads](https://github.com/zackads)' [sicp](https://github.com/zackads/sicp) repository.  

If any of the linked resources become unavailable or restricted, please refer to official UC Berkeley materials or alternative open-source resources.
