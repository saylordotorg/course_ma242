**Unit 3: Integration on Chains** <span id="3"></span> 
*The n-dimensional space **R<sup>n</sup>** may contain, for any
dimension k smaller than n, subspaces that locally look just like
**R<sup>k</sup>**. Such subspaces are examples of k-dimensional
manifolds (think of the two-dimensional sphere inside **R<sup>3</sup>**
as the set of points of distance 1 from the origin). It is natural and
desirable to be able to integrate suitable quantities defined over
k-dimensional manifolds inside **R<sup>n</sup>**.  
    
 Unfortunately, the adaptation of integration on **R<sup>n</sup>** to
integration over arbitrary manifolds is far from being a trivial task.
Part of the reason for this is that manifolds in **R<sup>n</sup>** can
be extremely complicated as soon as n\>2. The case n=1 presents little
difficulty since the only possible manifold
in ![](https://resources.saylor.org/wwwresources/archived/site/wp-content/uploads/2013/05/MA242-Unit2-Rbox.jpg) that
is of smaller dimension than that of
![](https://resources.saylor.org/wwwresources/archived/site/wp-content/uploads/2013/05/MA242-Unit2-Rbox.jpg)
is a point. The case n=2 already presents some difficulties, since now
manifolds inside **R<sup>2</sup>** include curves. This situation still
can be managed rather straightforwardly because the boundary of a curve
is a rather simple thing: either a point or a pair of points, or else an
empty set. In contrast, things get significantly more complicated in
higher dimensions since boundaries of arbitrary manifolds in
**R<sup>n</sup>**, for n\>2, can be very wild indeed. Thus, a more
systematic approach is required to allow us to circumvent these
geometric subtleties in order to arrive at a unifying theory.  
    
 Historically, it took mathematicians quite some time to develop the
unifying approach that is presented in this final unit of the course.
This approach requires quite a large dose of linear algebra involving
some very abstract notions. However, it also allows us to obtain a
unification of very complicated geometric notions as well as a very easy
proof of the Fundamental Theorem of Calculus in its most general
form – encompassing all notions of integrals on manifolds in the context
of this course. *

**Unit 3 Time Advisory**  
Completing this unit should take you approximately 26 hours.  
    
 ☐    Subunit 3.1: 5 hours  
    
 ☐    Subunit 3.2: 7 hours  
    
 ☐    Subunit 3.3: 5 hours  
    
 ☐    Subunit 3.4: 5 hours  
    
 ☐    Subunit 3.5: 4 hours

**Unit3 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:
-   define differential forms, their product, the exterior derivative,
    and the Hodge star operation;

<!-- -->

-   compute with differential forms;

<!-- -->

-   define n-chains and identify boundaries and cycles;

<!-- -->

-   define, compute, and use the winding number of a curve;

<!-- -->

-   define the integral of k-forms on n-chains;

<!-- -->

-   state and prove Stokes’ Theorem; and

<!-- -->

-   obtain the formulas of Green, Gauss, and Stokes as special cases.

**3.1 Manifolds** <span id="3.1"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar's *Manifolds and
    Differential Forms*: “Chapter 1, Sections 1-4: Introduction”**
    Link: Cornell University: Dr. Reyer Sjamaar's *Manifolds and
    Differential Forms*: [“Chapter 1, Sections 1-4:
    Introduction”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read the first four sections of Chapter 1,
    entitled “Introduction,” on pages 1 through 15. You will return to
    this textbook throughout this unit, so you may prefer to save this
    PDF to your computer for quick reference.  
        
     These sections will introduce you to the notion of manifolds in Rn.
    The numerous illustrations on these pages are very helpful for
    understanding the relevant geometric concepts, and the examples here
    are carefully chosen to indicate the importance of this notion. When
    you have completed this reading, you should attempt to solve all the
    exercises presented on pages 13-15. While it is advisable that you
    work through all the given exercises, you may also choose to
    concentrate only on the more crucial ones at this point in time,
    returning to the rest of the exercises later. If this is the case,
    make sure that you are able to solve exercises 1.1-1.6 at this time,
    and return to the remainder of the exercises as you progress through
    this unit, particularly when you feel that you need some
    experiential groundwork for the abstract notions being discussed.  
        
     Reading these sections and solving the exercises should take
    approximately 5 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.2 Differential Forms on Euclidean Space** <span id="3.2"></span> 
**3.2.1 Elementary Properties** <span id="3.2.1"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 2, Section 1: Elementary Properties”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 2, Section 1: Elementary
    Properties”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 1, entitled “Elementary Properties,” on
    pages 17 through 20, and stop when you reach the section
    entitled “The Exterior Derivative.”  
        
     This section introduces you to the concept of the differential
    form. In stark contrast with Chapter 1, which was very geometric in
    approach, this chapter is very algebraic in approach. It is likely
    that you will feel as if you do not understand how the abstract
    notions presented on these pages are at all related to integration.
    Don’t worry – things will become clearer as you progress through the
    upcoming subunits of this course. For now, focus on fully absorbing
    the algebraic concepts presented here so that you are prepared to
    see them in action in future readings. Remember that the way forward
    is by understanding all the arguments presented in the proofs on
    these pages. If a concept is not clear in this reading, try going
    back to earlier subunits of this course to review relevant
    definitions or previous results.  
        
     Reading this section should take approximately 1 hour.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.2.2 The Exterior Derivative** <span id="3.2.2"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 2, Section 2: The Exterior
    Derivative”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 2, Section 2: The Exterior
    Derivative”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 2, entitled “The Exterior Derivative,”
    on pages 20 through 22, and stop when you reach the section entitled
    “Closed and Exact Forms.”  
        
     This section introduces you to the exterior derivative operation,
    which as you will see, establishes a connection between differential
    forms and the gradient of a function (which you’ve met before). With
    this connection in place, you will begin to understand the relevance
    of differential forms to the theory of integration. As you read,
    remember that you will need to become proficient in performing
    computations with differential forms and the exterior derivative
    – both for concrete instances and for generic ones.  
        
     Reading this section should take approximately 30 minutes.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.2.3 Closed and Exact Forms** <span id="3.2.3"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 2, Section 3: Closed and Exact
    Forms”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 2, Section 3: Closed and Exact
    Forms”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 3, entitled “Closed and Exact Forms,” on
    pages 22 through 23, and stop when you reach the section
    entitled “The Hodge Star Operator.”  
        
     In this reading, you will discover that, upon using the exterior
    derivative introduced in the previous subunit, a differential form
    may exhibit certain properties, called *closed* and *exact*. The
    significance of these terms will become clearer to you later in this
    course. For now, you may consider these notions abstractly and focus
    on the definitions as they are presented in the reading. Please pay
    special attention to Example 2.10 on page 23, as it is central to
    your understanding of these concepts and will appear again later in
    this course.  
        
     Reading this section should take approximately 30 minutes.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.2.4 The Hodge Star Operator** <span id="3.2.4"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 2, Section 4: The Hodge Star
    Operator”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 2, Section 4: The Hodge Star
    Operator”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 4, entitled “The Hodge Star Operator,”
    on pages 23 through 24, and stop when you reach the section
    entitled “Div, Grad and Curl.”  
        
     This section describes the Hodge star operator on differential
    forms. The Hodge star operator is a combinatorial construction and
    thus computable. It has an elegant interpretation relating to vector
    fields and 1-forms. As such, it serves to relate the abstract
    notions of differential forms with more familiar geometric concepts
    of integration. As you read this section, focus on understanding the
    definition of the Hodge star operator. You will relate this abstract
    construction to more familiar concepts in the next subunit of this
    course.  
        
     Reading this section should take approximately 30 minutes.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.2.5 Divergence, Gradient and Curl** <span id="3.2.5"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 2, Section 5: Div, Grad and Curl”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 2, Section 5: Div, Grad and
    Curl”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 5, entitled “Div, Grad and Curl,” on
    pages 24 through 27, and stop when you reach the section
    entitled “Exercises.”  
        
     This section relates differential forms to divergence, gradient,
    and curl operators. This relationship is established by means of the
    Hodge star operator and is worked out in detail on these pages. In
    particular, the three equations surrounded by boxes on pages 26 and
    27 illustrate concepts that are fundamental to your work in this
    course. Please aim to understand these equations fully before
    proceeding to the next subunit.  
        
     Reading this section should take approximately 1 hour.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.2.6 Exercises** <span id="3.2.6"></span> 
-   **Activity: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 2, Exercises: Differential Forms on
    Euclidean Space”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 2, Exercises: Differential Forms on
    Euclidean
    Space”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Complete all the exercises presented in the section,
    which is on pages 27 through 30.  
        
     As you work, keep in mind that the concept of differential forms
    that you met at the beginning of this chapter – and the basic
    concepts related to it – form the computational heart of the rest of
    this unit of the course. Mastering these concepts now, which you can
    achieve by seriously attempting all the exercises on these pages,
    will facilitate your understanding of upcoming results and their
    proofs.  
        
     Working through these exercises should take approximately 3 hours
    and 30 minutes.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.3 Pulling Back Forms** <span id="3.3"></span> 
**3.3.1 Determinants** <span id="3.3.1"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 3, Section 1: Determinants”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 3, Section 1:
    Determinants”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 1, entitled “Determinants,” on pages 31
    through 36, and stop when you reach the section entitled “Pulling
    Back Forms.”  
        
     This section is a review of the concept of the determinant in
    linear algebra. In particular, this text approaches the determinant
    as a volume function and deduces its basic properties. The
    appearance of the determinant in the context of integration should
    not come as a surprise to you here, since you already have seen the
    determinant of the Jacobian play a prominent role in the Change of
    Variables formula for the Riemann integral. As you read, note how
    this section emphasizes the geometric interpretation of the
    determinant – particularly its effect on the concept of volume.  
        
     Reading this material, depending on your current understanding of
    the determinant, should take, at most, 1 hour.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.3.2 Pulling Back Forms** <span id="3.3.2"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 3, Section 2: Pulling Back Forms”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 3, Section 2: Pulling Back
    Forms”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 2, entitled “Pulling Back Forms,” on
    pages 36 through 45.  
        
     This section will introduce you to the important operation of
    pulling back differential forms along certain functions. You will
    learn the precise meaning of this operation as well as recount and
    prove its basic properties. Intuitively, pulling back a differential
    form is the result of changing the variables appearing in the form
    to new ones, with the old variables being expressed as smooth
    functions of the new ones. In this situation, there are some
    technical difficulties – or, to describe them more accurately, some
    unfamiliar direction reversals – that make grasping the results a
    bit more difficult here. But, if you have carefully followed the
    material presented in Chapter 2 and Chapter 3 of this textbook and
    have completed all the exercises assigned from those chapters, then
    you should be able to follow this section proficiently. The section
    ends by relating the pull-back operation to the determinant, thereby
    illuminating the geometric nature of the pull-back operation. Be
    sure to work through all the problem exercises presented on pages 42
    through 45 of this section.  
        
     Reading this section and working through the exercises should take
    approximately 4 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.4 Integration of 1-forms** <span id="3.4"></span> 
**3.4.1 Definition and Elementary Properties of the Integral** <span
id="3.4.1"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 4, Section 1: Definition and
    Elementary Properties of the Integral” and “Chapter 4, Section 2:
    Integration of Exact 1-forms”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 4, Section 1: Definition and
    Elementary Properties of the
    Integral”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF) and[“Chapter 4, Section 2: Integration of Exact
    1-forms”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 1 and Section 2 on pages 47 through 51,
    and stop when you reach the section entitled “The Global Angle
    Function and the Winding Number.”  
        
     This section is concerned with integrating 1-forms along smooth
    curves. You will learn about the geometric interpretation of this
    integral and prove some of its basic properties. The text presents
    the results concerning the integral of 1-forms in relation to the
    Fundamental Theorem of Calculus. It is very important that you
    understand this analogy, since the main purpose of the remainder of
    this unit of the course is to generalize the Fundamental Theorem of
    Calculus.  
        
     Reading these sections should take approximately 30 minutes.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.4.2 The Global Angle Function and the Winding Number** <span
id="3.4.2"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 4, Section 3: The Global Angle
    Function and the Winding Number”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 4, Section 3: The Global Angle
    Function and the Winding
    Number”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 3, entitled “The Global Angle Function
    and the Winding Number,” on pages 51 through 56.  Work through all
    of the exercises presented on pages 53 through 56.  
        
     This section will introduce you to the concept of the winding
    number, a geometric notion associated with curves that can be used
    to solve many problems. You will see it at work as you work through
    the exercises that accompany this section.  
        
     Reading this section and working through the exercises should take
    approximately 4 hours and 30 minutes.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.5 Integration and Stokes' Theorem** <span id="3.5"></span> 
**3.5.1 Integration of Forms Over Chains** <span id="3.5.1"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 5, Section 1: Integration of Forms
    Over Chains”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 5, Section 1: Integration of Forms
    Over
    Chains”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 1, entitled “Integration of Forms Over
    Chains,” on pages 57 through 59, and stop when you reach the section
    entitled “The Boundary of a Chain.”  
        
     This section will generalize the integral of a 1-form to the
    integral of a k-form for arbitrary, non-negative k. When integrating
    k-forms, it is very convenient to introduce the notion of chains,
    which are also discussed in this reading. The text examines in great
    detail some concrete examples of these concepts for low values of k.
    It is important for you to thoroughly understand these cases in
    order to develop your intuition regarding these concepts before you
    continue with the rest of this unit.  
        
     Reading this section should take approximately 30 minutes.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.5.2 Cycles and Boundaries of Chains** <span id="3.5.2"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 5, Section 2: The Boundary of a Chain”
    and “Chapter 5, Section 3: Cycles and Boundaries”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 5, Section 2: The Boundary of a
    Chain”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF) and [“Chapter 5, Section 3: Cycles and
    Boundaries”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 2 and Section 3 on pages 59 through 62,
    and stop when you reach the section entitled “Stokes’ Theorem.”  
        
     This section deals with the intricacies of higher dimensions and
    introduces you to cycles and boundaries for chains, allowing you to
    examine how chains of various dimensions interact with each other.
    The text also includes helpful illustrations that explain the
    geometric meaning of the algebraic concepts of boundary and cycle
    – aides that will help you understand and follow the proofs
    presented on these pages.  
        
     Reading these sections should take approximately 1 hour.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**3.5.3 Stokes' Theorem** <span id="3.5.3"></span> 
-   **Reading: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: “Chapter 5, Section 4: Stokes’ Theorem”**
    Link: Cornell University: Dr. Reyer Sjamaar’s *Manifolds and
    Differential Forms*: [“Chapter 5, Section 4: Stokes’
    Theorem”](http://www.math.cornell.edu/~sjamaar/papers/manifold.pdf)
    (PDF)  
        
     Instructions: Read Section 4, entitled “Stokes’ Theorem,” on pages
    63 through 65. Work through all the exercises presented on these
    pages.  
        
     This final reading of the course is concerned with the statement
    and proof of Stokes’ Theorem, also known as the Fundamental Theorem
    of Calculus. With all the mathematical machinery in place, after all
    the hard work you have done in the previous units of this course,
    the final statement of Stokes’ Theorem that is presented here comes
    across as being elegant, with the proof itself very short – almost
    trivial.  
        
     Reading this section and working through the exercises should take
    approximately 2 hours and 30 minutes.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**Final Exam** <span id="4"></span> 
-   **Final Exam: The Saylor Foundation's “MA242 Final Exam”**

    Link: The Saylor Foundation’s [“MA242 Final
    Exam”](http://school.saylor.org/mod/quiz/view.php?id=1395)

     

    Instructions: You must be logged into your Saylor Foundation School
    account in order to access this exam. If you do not yet have an
    account, you will be able to create one, free of charge, after
    clicking the link.


