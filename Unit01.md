---
layout: default
title: "MA242: Real Analysis II"
course_description: "A further study of real numbers, their real-valued functions, and integration and differentiation of these functions through the analysis of Manifolds."
next: ../Unit02
previous: ../Intro
---
**Unit 1: Differentiation on R<sup>n</sup>** <span id="1"></span> 
***A note about the mathematical notation used in this course:
Throughout this course, we will be concerned with the space***
R<sup>n</sup>***. Some authors refer to this space as***
E<sup>n</sup>***. As such, some of the resources provided in this course
use one notation, while others use the other notation. For all intents
and purposes, you may treat these two notations as interchangeable names
used for the same space.***  
    
 *The derivative of a function
![](https://resources.saylor.org/archived/wp-content/uploads/2013/05/MA242-Unit1Description-Eq1.jpg)
at a point p, as developed in*
[MA241](http://www.saylor.org/courses/ma241/)*, can be thought of as the
slope of the line (if it exists) tangent to the graph of the function f
at the point (p,f(p)). But generalizing this idea to a function
![](https://resources.saylor.org/archived/wp-content/uploads/2013/05/MA242-Unit1Description-Eq2.jpg)
is not straightforward. To see why, consider a function
![](https://resources.saylor.org/archived/wp-content/uploads/2013/05/MA242-Unit1Description-Eq3.jpg). Its
graph is an object in four dimensions and it is not at all clear what a
tangent line would be for such an object.  
    
 Recall that in MA241 you learned how the derivative of a function at a
point, which is just a single real number, can be used to discern quite
a lot of information about the function *<span
style="font-size: 12pt; font-family: Arial, sans-serif; background-position: initial initial; background-repeat: initial initial;">–</span>* at
least in a small interval containing the given point. For instance, you
saw that the derivative can be used to locate local maxima and minima of
the function, to determine whether the function increases or decreases,
to determine whether a function is locally invertible, and, through
repeated derivations and Taylor’s Theorem, to obtain powerful
approximations of the function.  
    
 In the first unit of this course, you will explore how to extend these
techniques to functions of several real variables. Indeed, a
fundamentally different idea is required in order to describe what the
correct analog of the derivative of a function is for functions of
several variables. You will learn that the correct notion to use is that
of the differential of a function, which is nothing but a linear map. By
approaching multivariable functions in this way, you will build a strong
bridge between multivariable analysis and linear algebra. You will see
how the techniques of differential calculus from MA241 can be developed
further to obtain powerful techniques in higher dimensions. In
particular, you will learn how to use the differential map to determine
local maxima and minima and local invertiblity, how to generalize
Taylor’s Theorem, and how to apply the technique of Lagrange multipliers
to solve more general problems, such as locating extremal points.  
    
 From the very beginning of this unit, you will see that higher
dimensions introduce many new difficulties and subtleties* – *complex
aspects that will accompany you throughout this course. As you approach
these subtleties, it may be helpful to keep the following analogy in
mind: Riding a bicycle is relatively easy, since generally there are
only two directions one can fall in* – *to either side of the wheels.
But riding a unicycle is far more difficult, since there are now
infinitely many directions one can fall in. The transition of going from
single-variable functions to multivariable functions is comparable to
learning to ride a unicycle when, up to this point, you have learned
only how to ride a bicycle.*

**Unit 1 Time Advisory**  
Completing this unit should take you approximately 66 hours.  
    
 ☐    Subunit 1.1: 4 hours  
    
 ☐    Subunit 1.2: 6 hours  
    
 ☐    Subunit 1.3: 8 hours  
    
 ☐    Subunit 1.4: 5 hours  
    
 ☐    Subunit 1.5: 7 hours  
    
 ☐    Subunit 1.6: 6 hours  
    
 ☐    Subunit 1.7: 10 hours  
    
 ☐    Subunit 1.8: 8 hours  
    
 ☐    Subunit 1.9: 6 hours  
    
 ☐    Subunit 1.10: 6 hours

**Unit1 Learning Outcomes**  
Upon successful completion of this unit, you should be able to:  
-   define and compute directional and partial derivatives;

<!-- -->

-   prove properties of the directional and partial derivatives;

<!-- -->

-   summarize the role of matrices in the theory of differentiation;

<!-- -->

-   define differentiable functions;

<!-- -->

-   prove properties of the differential;

<!-- -->

-   state, use, and prove the chain rule and the Cauchy invariant rule;

<!-- -->

-   compute and prove properties related to repeated differentiation;

<!-- -->

-   use and prove Taylor’s Theorem in higher dimensions;

<!-- -->

-   define, compute, and prove properties related to the Jacobian;

<!-- -->

-   state, prove, and use the Inverse Function Theorem;

<!-- -->

-   define and use the technique of a Baire category;

<!-- -->

-   locate local and global maxima and minima; and

<!-- -->

-   apply the method of Lagrange multipliers to locate conditional
    maxima and minima.

**1.1 Directional and Partial Derivatives** <span id="1.1"></span> 
-   **Reading: Professor Elias Zakon’s Mathematical Analysis: Volume II:
    “Chapter 6, Section 1: Directional and Partial Derivatives”**
    Link: Professor Elias Zakon’s *Mathematical Analysis: Volume II*:
    [“Chapter 6, Section 1: Directional and Partial
    Derivatives”](http://www.trillia.com/zakon-analysisII.html) (PDF)  
        
     Instructions: Scroll down to the “Download the Book” section and
    download your preferred version by clicking the appropriate “I
    accept” link. Read Section 1, “Directional and Partial Derivatives,”
    and stop on page 7. You will return to this textbook throughout this
    unit, so you may prefer to save this PDF to your computer for quick
    reference.  
        
     The idea behind the directional derivative is to eliminate
    dimensions so as to obtain a function of a single variable.
    Following this step, you immediately can apply the techniques of
    differential calculus that you encountered in
    [MA241](http://www.saylor.org/courses/ma241/). In this reading, you
    will explore how to reduce to one dimension and establish the first
    properties of the directional derivative. Be sure to follow
    carefully the examples presented in this reading and to work through
    all the problem exercises presented on pages 6-7.  
        
     Reading this section and completing the exercises should take
    approximately 4 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above. 

**1.2 Linear Maps, Functionals, and Matrices** <span id="1.2"></span> 
-   **Reading: Professor Elias Zakon’s Mathematical Analysis: Volume II:
    “Chapter 6, Section 2: Linear Maps and Functionals. Matrices”**
    Link: Professor Elias Zakon’s *Mathematical Analysis: Volume II*:
    [“Chapter 6, Section 2: Linear Maps and Functionals.
    Matrices”](http://www.trillia.com/zakon-analysisII.html) (PDF)  
        
     Instructions: Read Section 2, “Linear Maps and Functionals.
    Matrices,” and stop on page 16.  
        
     The directional derivative that you encountered in subunit 1.1 is
    not, on its own, a sufficient tool for approaching
    higher-dimensional differential calculus. In preparation for a more
    refined notion of differentiable functions, this reading
    concentrates on those properties of linear maps that are relevant to
    the coming definitions you will encounter in this unit of the
    course. Please note that some aspects of this reading will be a
    review of concepts you already know
    from [MA211](http://www.saylor.org/courses/ma211/) Linear Algebra.
    Be sure to work through all the problem exercises presented on pages
    14-16 of this reading.  
        
     Reading this section and completing the exercises should take
    approximately 6 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above. 

**1.3 Differentiable Functions** <span id="1.3"></span> 
-   **Reading: Professor Elias Zakon’s Mathematical Analysis: Volume II:
    “Chapter 6, Section 3: Differentiable Functions”**
    Link: Professor Elias Zakon’s *Mathematical Analysis: Volume II*:
    [“Chapter 6, Section 3: Differentiable
    Functions”](http://www.trillia.com/zakon-analysisII.html) (PDF)  
        
     Instructions: Read Section 3, titled “Differentiable Functions,”
    stopping on page 28.  
        
     This section introduces you to the heart of differential calculus.
    In sharp contrast with the case in
    [MA241](http://www.saylor.org/courses/ma241/) – in which the
    derivative of a function at a point was simply a real number – the
    consequences of higher dimensions prohibit this kind of simplicity
    for the differentiability of functions of higher dimensions.
    Instead, you will see that the correct notion of the differential at
    a point for higher dimensional functions is a linear map that
    satisfies certain properties. Some aspects of this reading may not
    be easy to understand at first, but the concepts presented here are
    absolutely crucial for you to follow and comprehend. Be sure to
    review along the way, as necessary, and work through all the problem
    exercises presented on pages 25-28 of this reading.  
        
     Reading this section and completing the exercises should take
    approximately 8 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**1.4 The Chain Rule and the Cauchy Invariant Rule** <span
id="1.4"></span> 
-   **Reading: Professor Elias Zakon's Mathematical Analysis: Volume II:
    “Chapter 6, Section 4: The Chain Rule. The Cauchy Invariant Rule”**
    Link: Professor Elias Zakon's *Mathematical Analysis: Volume II*:
    [“Chapter 6, Section 4: The Chain Rule. The Cauchy Invariant
    Rule”](http://www.trillia.com/zakon-analysisII.html) (PDF)  
        
     Instructions: Read Section 4, titled “The Chain Rule. The Cauchy
    Invariant Rule,” and stop on page 35.  
        
     Recall that in [MA241](http://www.saylor.org/courses/ma241/) you
    learned about the chain rule for computing the derivative of a
    composite function. This section focuses on the generalization of
    this result to the composition of functions in higher dimensions.
    You will see that while the chain rule from MA241 requires only the
    multiplication of two numbers to obtain the correct derivative,
    acquiring the result for higher dimensions is somewhat more
    intricate. However, you may remember the essence of this process
    with a helpful slogan: The differential of a composite function is
    the composite of the differential functions. Be sure to work through
    all the problem exercises presented on pages 33-35.  
        
     Reading this section and completing the exercises should take
    approximately 5 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**1.5 Repeated Differentiation and Taylor’s Theorem** <span
id="1.5"></span> 
-   **Reading: Professor Elias Zakon’s Mathematical Analysis: Volume II:
    “Chapter 6, Section 5: Repeated Differentiation. Taylor’s Theorem”**
    Link: Professor Elias Zakon’s *Mathematical Analysis: Volume
    II*: [“Chapter 6, Section 5: Repeated Differentiation. Taylor’s
    Theorem”](http://www.trillia.com/zakon-analysisII.html) (PDF)  
        
     Instructions: Read Section 5, titled “Repeated Differentiation.
    Taylor’s Theorem,” and stop on page 47.  
        
     In this reading, you will encounter your first application of
    differentiation in higher dimensions. Recall that in
    [MA241](http://www.saylor.org/courses/ma241/) you worked with
    Taylor’s Theorem, which enables the approximation of functions by
    repeatedly computing their derivatives at a point. This section
    focuses on extending this technique to higher dimensions. The
    generalization presented here is a direct one. The only difficulties
    lie in keeping track of the indices, of which there are many due to
    the high number of dimensions. Be sure to work through all the
    problem exercises presented on pages 44-47.  
        
     Reading this section and completing the exercises should take
    approximately 7 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above. 

**1.6 Determinants, Jacobians, and Bijective Linear Operators** <span
id="1.6"></span> 
-   **Reading: Professor Elias Zakon’s Mathematical Analysis: Volume II:
    “Chapter 6, Section 6: “Determinants. Jacobians. Bijective Linear
    Operators”**
    Link: Professor Elias Zakon’s *Mathematical Analysis: Volume II*:
    [“Chapter 6, Section 6: “Determinants. Jacobians. Bijective Linear
    Operators”](http://www.trillia.com/zakon-analysisII.html) (PDF)  
        
     Instructions: Read Section 6, titled “Determinants. Jacobians.
    Bijective Linear Operators,” and stop on page 57.  
        
     Because the differential of a function is a linear map and because
    linear maps are closely related to matrices, the differential
    calculus in higher dimensions is also closely related to matrices.
    This section introduces you to the concept of the Jacobian of a
    function and then studies some of the Jacobian’s properties. In the
    next subunit, you will use these properties to establish the very
    important Inverse Function Theorem. Be sure to work through all the
    problem exercises presented on pages 55-57.  
        
     Reading this section and completing the exercises should take
    approximately 6 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**1.7 Inverse and Implicit Functions; Open and Closed Maps** <span
id="1.7"></span> 
-   **Reading: Professor Elias Zakon’s Mathematical Analysis: Volume II:
    “Chapter 6, Section 7: Inverse and Implicit Functions. Open and
    Closed Maps”**
    Link: Professor Elias Zakon’s *Mathematical Analysis: Volume II*:
    [“Chapter 6, Section 7: Inverse and Implicit Functions. Open and
    Closed Maps”](http://www.trillia.com/zakon-analysisII.html) (PDF)  
        
     Instructions: Read Section 7, titled “Inverse and Implicit
    Functions. Open and Closed Maps,” and stop on page 70.  
        
     In [MA241](http://www.saylor.org/courses/ma241/), you learned that
    if a function has a non-zero derivative at a point, then it is
    invertible, at least in a small open interval containing that point.
    This case is an example of how you can infer local information about
    a function from knowledge of its derivative at just one single
    point. This section takes this technique further, focusing on the
    generalization of this result (and some related results) and its
    application to higher dimensions. Be sure to work through all the
    problem exercises presented on 67-70.  
        
     Reading this section and completing the exercises should take
    approximately 10 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**1.8 Baire Categories; More on Linear Maps** <span id="1.8"></span> 
-   **Reading: Professor Elias Zakon’s Mathematical Analysis: Volume II:
    “Chapter 6, Section 8: Baire Categories. More on Linear Maps”**
    Link: Professor Elias Zakon’s *Mathematical Analysis: Volume II*:
    [“Chapter 6, Section 8: Baire Categories. More on Linear
    Maps”](http://www.trillia.com/zakon-analysisII.html) (PDF)  
      
     Instructions: Read Section 8, titled “Baire Categories. More on
    Linear Maps,” and stop on page 79.  
        
     This section introduces you to a powerful concept in analysis, the
    notion of a Baire category. It was introduced and first used by the
    French mathematician René-Louis Baire, and it constitutes a
    fundamental tool in modern analysis. A Baire category is a
    topological and set theoretic concept and thus constitutes a
    technique with a somewhat different flavor from what you have seen
    so far in this course. This section will guide you through the
    concepts that you need to understand and illustrate the
    applicability of a Baire category. Be sure to work through all the
    problem exercises presented on pages 76-79 of this reading.  
        
     Reading this section and completing the exercises should take
    approximately 8 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.

**1.9 Local Extrema, Maxima, and Minima** <span id="1.9"></span> 
-   **Reading: Professor Elias Zakon’s Mathematical Analysis: Volume II:
    “Chapter 6, Section 9: Local Extrema. Maxima and Minima”**
    Link: Professor Elias Zakon’s *Mathematical Analysis: Volume II*:
    [“Chapter 6, Section 9: Local Extrema. Maxima and
    Minima”](http://www.trillia.com/zakon-analysisII.html) (PDF)  
        
     Instructions: Read Section 9, titled “Local Extrema. Maxima and
    Minima,” and stop on page 87.  
        
     As you saw in [MA241](http://www.saylor.org/courses/ma241/), the
    derivative of a function is a very powerful tool that can be used to
    locate maxima and minima of a function. Locating extremal values of
    a function is crucial for solving many problems in science, since
    often a problem can be stated as finding a maximum or a minimum of a
    function. Moreover, historically such problems have constituted one
    of the main driving forces in developing the calculus. In this
    reading, you will learn how to apply the techniques developed so far
    in this course to help you locate the extremal values of a function
    in higher dimensions. Be sure to work through all the problem
    exercises presented on pages 84-87.  
        
     Reading this section and completing the exercises should take
    approximately 6 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above. 

**1.10 More on Implicit Differentiation and Conditional Extrema** <span
id="1.10"></span> 
-   **Reading: Professor Elias Zakon’s Mathematical Analysis: Volume II:
    “Chapter 6, Section 10: More on Implicit Differentiation.
    Conditional Extrema”**
    Link: Professor Elias Zakon’s *Mathematical Analysis: Volume II*:
    [“Chapter 6, Section 10: More on Implicit Differentiation.
    Conditional Extrema”](http://www.trillia.com/zakon-analysisII.html)
    (PDF)  
      
     Instructions: Read Section 10, titled “More on Implicit
    Differentiation. Conditional Extrema,” stopping on page 96.  
        
     This section establishes further the technique of implicit
    differentiation and introduces you to the technique of using
    Lagrange multipliers. This technique is a very powerful method for
    obtaining extremal points of a function whose variables are
    conditioned on some smaller subset in the higher-dimensional space.
    This is a new phenomenon that you did not see in
    [MA241](http://www.saylor.org/courses/ma241/) – simply because when
    considering only one dimension, such restrictions are useless. In
    contrast, when considering higher dimensions, these are very
    relevant problems. The technique of using Lagrange multipliers
    – named after the eighteenth-century French-Italian mathematician
    Joseph-Louis Lagrange – is a general method that may be used for
    solving such problems. This section represents the culmination point
    of the first unit of this course, which has focused on
    differentiation.  
        
     For this reading, it is recommended that you read carefully through
    the text to understand each and every detail and concentrate on the
    proofs and examples provided. Following your reading, work through
    the exercises at the end of the section, on pages 94-96, reviewing
    the text as needed. Complete as many of the exercises as you feel
    are needed for you have a good understanding of how the method of
    Lagrange multipliers works.  
        
     Reading this section and completing the exercises should take
    approximately 6 hours.  
        
     Terms of Use: Please respect the terms of use and copyright
    displayed on the webpage above.


