---
layout: default
title: "MA242: Real Analysis II"
course_description: "A further study of real numbers, their real-valued functions, and integration and differentiation of these functions through the analysis of Manifolds."
next: ../Unit03
previous: ../Unit01
---
**Unit 2: Riemann Integration in Higher Dimensions** <span
id="2"></span> 
*As you learned in* [MA241](http://www.saylor.org/courses/ma241/)*, the
integral is a form of a continuous sum that is developed and used to
measure the area between the graph of a function and the X-axis. The
graph of a “nice-enough” function
![](https://resources.saylor.org/archived/wp-content/uploads/2013/05/MA242-Unit2Description-Eq1.jpg)
encloses an area in
![](https://resources.saylor.org/archived/wp-content/uploads/2013/05/MA242-Unit2Description-R3.jpg)
which, at least intuitively, has volume. The Riemann integral for such
functions turns this idea into a concrete definition that is a direct
generalization of the concept of the Riemann integral for functions
![](https://resources.saylor.org/archived/wp-content/uploads/2013/05/MA242-Unit2Description-Eq2.jpg).
Unlike the case of differentiability, which we explored in the previous
unit of this course, the passage to higher dimensions presents
relatively little difficulty in the case of the Riemann integral. In
this unit you will define the n-dimensional Riemann integral; study the
basic properties of this integral; see the subtleties that do arise for
this case; and learn two important computation techniques: repeated
integrals and the Change of Variables formula. The latter is a
generalization of the Change of Variable formula that you learned about
in MA241.*

**Unit 2 Time Advisory**  
Completing this unit should take you approximately 45 hours.  
    
 ☐    Subunit 2.1: 3 hours  
    
 ☐    Subunit 2.2: 8 hours  
    
 ☐    Subunit 2.3: 34 hours

**Unit2 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:
-   define the Riemann integral of a function
    ![](https://resources.saylor.org/archived/wp-content/uploads/2013/05/MA242-Unit2LOs-Eq1.jpg);

<!-- -->

-   define and recognize sets of zero content;

<!-- -->

-   state and prove the basic properties of the Riemann integral;

<!-- -->

-   identify Riemann integrable functions;

<!-- -->

-   relate multiple and iterated integrals;

<!-- -->

-   compute Riemann integrals using iterated integrals;

<!-- -->

-   deine and recognize Jordan measurable sets;

<!-- -->

-   summarize the role of Jordan measurable sets in the theory of the
    Riemann integral;

<!-- -->

-   formulate and prove the Change of Variables formula;

<!-- -->

-   compute integrals with the Change of Variables formula; and

<!-- -->

-   use polar and spherical coordinates.

**2.1 A Review of Riemann Integration in
![](https://resources.saylor.org/archived/wp-content/uploads/2013/05/MA242-Unit2-Rbox.jpg)**
<span id="2.1"></span> 
-   **Reading: Trinity University: Dr. William F. Trench's *Introduction
    to Real Analysis*: “Chapter 3, Section 1: Definition of the
    Integral” and “Chapter 3, Section 2: Existence of the Integral”**
    Link: Trinity University: Dr. William F. Trench's *Introduction to
    Real Analysis*: [“Chapter 3, Section 1: Definition of the
    Integral”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF) and [“Chapter 3, Section 2: Existence of the
    Integral”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Read Chapter 3, titled “Integral Calculus of
    Functions of One Variable,” on pages 113 through 134. Skip the
    subsection on page 125 regarding the Riemann-Stieltjes Integral. You
    will return to this textbook throughout this unit, so you may prefer
    to save this PDF to your computer for quick reference.  
        
     The aim of this reading is to refresh your memory regarding the
    definition and intuitive geometric meaning of the integral of
    functions of one variable. As you read, please pay particular
    attention to the notions of intervals, lower and upper sums, and the
    rigorous definition of the Riemann integral and its geometric
    interpretation. Remember that this reading comprises a review of
    material you already have learned, and thus you do not need to
    complete the reading’s supplementary exercises unless you feel they
    will benefit your studies. Please keep in mind that you may find
    yourself returning to this reading to review material as you
    approach the remaining topics of this unit.  
        
     Taking this review reading seriously will provide you with a sound
    foundation for understanding the material in the rest of this unit.
    Unless you feel completely fluent with the details of the Riemann
    integral from [MA241](http://www.saylor.org/courses/ma241/), you
    should spend up to 3 hours on this reading.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**2.2 Riemann Integration in R<sup>n</sup>** <span id="2.2"></span> 
**2.2.1 Integrals over Rectangles** <span id="2.2.1"></span> 
-   **Reading: Trinity University: Dr. William F. Trench’s *Introduction
    to Real Analysis*: “Chapter 7, Section 1: Definition and Existence
    of the Multiple Integral”**
    Link: Trinity University: Dr. William F. Trench’s *Introduction to
    Real Analysis*: [“Chapter 7, Section 1: Definition and Existence of
    the Multiple
    Integral”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Read Section 1, “Definition and Existence of the
    Multiple Integral.” Begin on page 435 at section titled “Integrals
    over Rectangles” and read through page 441, stopping when you reach
    the section titled “Upper and Lower Integrals.”  
        
     As you read through the material, visualize only the case n=2, as
    this case is sufficient to understand the subtleties of all higher
    dimensions. Try to absorb the concepts and results you see on these
    pages as directly analogous to familiar concepts from
    [MA241](http://www.saylor.org/courses/ma241/). In particular, notice
    how the concepts of intervals and the Riemann integral that you
    reviewed in Subunit 2.1 are now being generalized to higher
    dimensions.  
        
     Reading this section should take approximately 1 hour.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above. 

**2.2.2 The Volume of Rectangles; Upper and Lower Sums** <span
id="2.2.2"></span> 
-   **Reading: Trinity University: Dr. William F. Trench’s *Introduction
    to Real Analysis*: “Chapter 7, Section 1: Definition and Existence
    of the Multiple Integral”**
    Link: Trinity University: Dr. William F. Trench’s *Introduction to
    Real Analysis*: [“Chapter 7, Section 1: Definition and Existence of
    the Multiple
    Integral”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Read Section 1, titled “Definition and Existence of
    the Multiple Integral.” Start on page 441 at the section titled
    “Upper and Lower Integrals.” Read through page 448 and stop at the
    section titled “Sets with Zero Content.”  
        
     In this reading you will encounter many elementary properties of
    the Riemann integral in higher dimensions. To help you interpret
    these results in the right context, please note that the text refers
    to results about the Riemann integral of functions of one variable,
    which you reviewed at the beginning of this unit. In this sense, the
    new results about the Riemann integral in higher dimensions are
    analogous to familiar properties of the Riemann integral from
    [MA241](http://www.saylor.org/courses/ma241/). Note that many of the
    proofs presented in these pages are left to you, the reader, to
    complete. Please be sure to work through these exercises as you
    read.  
        
     Reading this section and completing the exercises should take
    approximately 3 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above. 

**2.2.3 Sets of Zero Content** <span id="2.2.3"></span> 
-   **Reading: Trinity University: Dr. William F. Trench’s *Introduction
    to Real Analysis*: “Chapter 7, Section 1: Definition and Existence
    of the Multiple Integral”**
    Link: Trinity University: Dr. William F. Trench’s *Introduction to
    Real Analysis*: [“Chapter 7, Section 1: Definition and Existence of
    the Multiple
    Integral”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Read Section 1, entitled “Definition and Existence of
    the Multiple Integral.” Start on page 448 at the section titled
    “Sets of Zero Content.” Read through page 453 and stop when you
    reach the section titled “Differentiable Surfaces.”  
        
     In this reading, you will encounter the geometric subtleties of
    higher dimensions that relate to integration. Intuitively, sets of
    zero content are sets that do not affect the Riemann integral, and
    thus these sets are important in stating properties of the Riemann
    integral and understanding its behavior. Sets of zero content also
    are relevant for the Riemann integral of functions of one variable.
    However, in higher dimensions, sets of zero content can be very
    complicated and include many interesting cases. You will encounter
    some of these sets in the next sub-subunit of this course.  
        
     Reading this material should take approximately 1 hour and 30
    minutes.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**2.2.4 Differentiable Surfaces** <span id="2.2.4"></span> 
-   **Reading: Trinity University: Dr. William F. Trench’s *Introduction
    to Real Analysis*: “Chapter 7, Section 1: Definition and Existence
    of the Multiple Integral”**
    Link: Trinity University: Dr. William F. Trench’s *Introduction to
    Real Analysis*: [“Chapter 7, Section 1: Definition and Existence of
    the Multiple
    Integral”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Read Section 1, “Definition and Existence of the
    Multiple Integral.” Start on page 453 at the section titled
    “Differentiable Surfaces.” Read through page 455 and stop when you
    reach the section titled “Properties of Multiple Integrals.”  
        
     This chapter presents a particular family of sets of zero content.
    These sets are carved out of the ambient space ***R<sup>n</sup>***
    by the use of differentiable equations. You will see in the examples
    presented in the text that such sets include many familiar and
    important spaces.  
        
     Reading this section should take approximately 1 hour.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**2.2.5 Properties of the Riemann Integrals** <span id="2.2.5"></span> 
-   **Reading: Trinity University: Dr. William F. Trench’s *Introduction
    to Real Analysis*: “Chapter 7, Section 1: Definition and Existence
    of the Multiple Integral”**
    Link: Trinity University: Dr. William F. Trench’s *Introduction to
    Real Analysis*: [“Chapter 7, Section 1: Definition and Existence of
    the Multiple
    Integral”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Read Section 1, entitled “Definition and Existence of
    the Multiple Integral.” Start on page 455 at the section titled
    “Properties of Multiple Integrals.” Read through page 459 and stop
    when you reach the section entitled “7.1 Exercises.”  
        
     In this reading, you will explore the many basic properties that
    are true of the Riemann integral, which was developed at the
    beginning of this unit. Notice that the results presented here in
    the text are direct analogues of the properties of the Riemann
    integral for functions of one variable. Also note that most of the
    proofs presented on these pages are left as exercises for you, the
    reader, to complete. It is vital that you complete the proofs
    presented here in order to cement your understanding of these
    concepts. If you’ve carefully studied the material developed so far
    in this course, especially in the context of the familiar results of
    [MA241](http://www.saylor.org/courses/ma241/), then you should be
    able to complete all the proofs presented on these pages.  
        
     Reading this material should take approximately 1 hour and 30
    minutes.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**2.3 Techniques of Integration** <span id="2.3"></span> 
**2.3.1 Preparatory Exercises** <span id="2.3.1"></span> 
-   **Activity: Trinity University: Dr. William F. Trench’s
    *Introduction to Real Analysis*: “Chapter 7, Section 1: Definition
    and Existence of the Multiple Integral”**
    Link: Trinity University: Dr. William F. Trench’s *Introduction to
    Real Analysis*: [“Chapter 7, Section 1: Definition and Existence of
    the Multiple
    Integral”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Work through all the exercises in the section titled
    “7.1 Exercises” beginning on page 459.  
        
     So far, this unit of the course has covered the definition and
    basic properties of the Riemann integral in higher dimensions. This
    set of exercises is concerned with developing techniques of
    computation and simplification of the Riemann integral. You should
    proceed to the next sub-subunit of this course only after you feel
    comfortable with the exercises presented on these pages.  
        
     Working through these exercises should take approximately 10
    hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**2.3.2 Iterated Integrals and Repeated Integrals** <span
id="2.3.2"></span> 
-   **Reading: Trinity University: Dr. William F. Trench's *Introduction
    to Real Analysis*: “Chapter 7, Section 2: Iterated Integrals and
    Multiple Integrals”**
    Link: Trinity University: Dr. William F. Trench's *Introduction to
    Real Analysis*: [“Chapter 7, Section 2: Iterated Integrals and
    Multiple
    Integrals”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Read Section 2: “Iterated Integrals and Multiple
    Integrals” on pages 462 through 484.  
        
     As you read this section, you will be introduced to a very
    important technique for reducing the computation of a Riemann
    integral in dimension *n* to the computation of n ordinary Riemann
    integrals. This new technique allows all the techniques for
    computations of integrals that you learned in
    [MA241](http://www.saylor.org/courses/ma241/) to be used in higher
    dimensions as well. This section is quite lengthy, not because the
    technique is very complicated, but rather because many examples are
    worked out in great detail. You will see that in practice, this is a
    rather simple method to implement. Be sure to work through all the
    problem exercises presented on pages 480-484 of this reading.  
        
     Reading this section and completing the exercises should take
    approximately 10 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**2.3.3 The Change of Variables Formula** <span id="2.3.3"></span> 
*This sub-subunit is concerned with the Change of Variables formula for
the Riemann integral in higher dimensions. Recall that the Change of
Variable formula for the ordinary Riemann integral, which you met in*
[MA241](http://www.saylor.org/courses/ma241/)*, involved changing the
bounds of integration ***–*** in effect, changing the set over which the
function is integrated. A similar phenomenon occurs in higher dimensions
as well, but in higher dimensions the change required can be far more
elaborate and subtle than it is in the one-dimensional case. In the
following sub-subunits of this course, prepare yourself to be confronted
with rather complicated geometrical difficulties before arriving at the
sought formula.*

**2.3.3.1 Change of Variables in Multiple Integrals** <span
id="2.3.3.1"></span> 
-   **Reading: Trinity University: Dr. William F. Trench's *Introduction
    to Real Analysis*: “Chapter 7, Section 3: Change of Variables in
    Multiple Integrals”**
    Link: Trinity University: Dr. William F. Trench's *Introduction to
    Real Analysis*: [“Chapter 7, Section 3: Change of Variables in
    Multiple
    Integrals”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Read Section 3, entitled “Change of Variables in
    Multiple Integrals,” on pages 484 through 494, and stop when you
    reach the section entitled “Formulation of the Rule for Change of
    Variables.”  
        
     This section will guide you through the concepts of Jordan
    measurable sets, transformations of such sets, and the change of
    content that occurs under a linear transformation. It turns out that
    Riemann integration works well when integrating over what are known
    as Jordan measurable sets. Anticipating that a change of variables
    will distort the set upon which the function is integrated, you
    first must understand how Jordan measurable sets are transformed
    – in particular, the effect of linear transformations on the content
    of such sets.  
        
     Reading this section should take approximately 1 hour.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**2.3.3.2 Formulation of the Rule for Change of Variables** <span
id="2.3.3.2"></span> 
-   **Reading: Trinity University: Dr. William F. Trench's *Introduction
    to Real Analysis*: “Chapter 7, Section 3: Change of Variables in
    Multiple Integrals”**
    Link: Trinity University: Dr. William F. Trench's *Introduction to
    Real Analysis*: [“Chapter 7, Section 3: Change of Variables in
    Multiple
    Integrals”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Read Section 3, entitled “Change of Variables in
    Multiple Integrals,” on page 494 through 496, and stop when you
    reach the section entitled “The Main Theorem.”  
        
     This section will guide you through the geometric intuition that
    leads to the Change of Variables formula. Since the formula itself
    takes some time to get used to, it would be a good idea for you to
    read through this section at least twice. On your first reading, try
    to absorb the geometric intuition, but do not stop to contemplate
    any details. Following your first reading, spend some time
    considering and interpreting the Change of Variables formula. Then,
    read these pages again, this time spending as much time as is
    required for you to understand each step.  
        
     Reading this section should take approximately 1 hour.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**2.3.3.3 The Main Theorem** <span id="2.3.3.3"></span> 
-   **Reading: Trinity University: Dr. William F. Trench's *Introduction
    to Real Analysis*: “Chapter 7, Section 3: Change of Variables in
    Multiple Integrals”**
    Link: Trinity University: Dr. William F. Trench's *Introduction to
    Real Analysis*: [“Chapter 7, Section 3: Change of Variables in
    Multiple
    Integrals”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF) (PDF)  
        
     Instructions: Read Section 3, entitled “Change of Variables in
    Multiple Integrals,” on page 496 through 505, and stop when you
    reach the section entitled “Polar Coordinates.”  
        
     This section is concerned with the proof of the Change of Variables
    formula. This proof is quite involved and certainly not easy to
    comprehend – it is therefore recommended that you tackle this proof
    in two stages. For this assignment, try not to spend more than one
    hour reading over the material, keeping in mind that it is
    acceptable not to understand each step of the proof at this point.
    You can refer back to this reading after you have progressed through
    the next subunit of this course and completed a few exercises that
    apply the Change of Variables formula. After you have worked through
    some exercises using this formula, you likely will find this proof
    more palatable and easier to understand.  
        
     Reading this section should take approximately 2 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**2.3.3.4 Polar Coordinates, Spherical Coordinates, and Exercises**
<span id="2.3.3.4"></span> 
-   **Reading: Trinity University: Dr. William F. Trench's *Introduction
    to Real Analysis*: “Chapter 7, Section 3: Change of Variables in
    Multiple Integrals”**
    Link: Trinity University: Dr. William F. Trench's *Introduction to
    Real Analysis*: [“Chapter 7, Section 3: Change of Variables in
    Multiple
    Integrals”](http://ramanujan.math.trinity.edu/wtrench/texts/TRENCH_REAL_ANALYSIS.PDF)
    (PDF)  
        
     Instructions: Read Section 3, entitled “Change of Variables in
    Multiple Integrals,” on page 505 through 517.  
        
     In this reading, you will see the Change of Variables formula
    demonstrated for two particular changes of variables known as polar
    coordinates and spherical coordinates. These changes of variables
    have a geometric interpretation – as explained and illustrated in
    the text – so as to make it easier for you to understand the general
    formula. Be sure to work through all the problem exercises presented
    on pages 514-517 of this reading.  
        
     Reading this section and completing the exercises should take
    approximately 10 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.


