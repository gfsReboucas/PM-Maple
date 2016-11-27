===============================================
       Perturbation Methods with Maple
            
       Ali H. Nayfeh and Char-Ming Chin

Email: anayfeh@vt.edu    cchin@vt.edu
Website: http://www2.esm.vt.edu/~nayfeh/
===============================================
     Copyright 1999 by Dynamics Press, Inc.


    (* Version 1.0 for Maple V Release 4 *)


This README includes the following information:

    *    Legal Information
    *    Table of Contents
    *    Bug Reports
    *    Developers Note


*****************
Legal Information
*****************

Copyright (c) 1999 Ali H. Nayfeh and Char-Ming Chin

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (Perturbation Methods
with Maple), to deal in the Software without restriction, including 
without limitation the rights to use, copy, modify, merge, publish, distribute, 
sublicense, and/or sell copies of the Software, and to permit persons to 
whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY
OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT 
LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS 
BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, 
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE 
OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Permission Department, Dynamics Press, Inc., 
300 Murphy Street, Blacksburg, VA 24060.

Maple is a registered trademark of Waterloo Maple, Inc..

  
*****************
Table of Contents
*****************

-----------------------
Chapter 1: Introduction
-----------------------
   1.1 Preliminary Remarks
   1.2 Symbolic Computation
      1.2.1 Assigning Names to Expressions
      1.2.2 Expressions
      1.2.3 Expression Manipulation
      1.2.4 Evaluation Rules

-------------------------------
Chapter 2: The Duffing Equation
-------------------------------
   2.1 The Duffing Equation
   2.2 Straightforward Expansion
   2.3 The Lindstedt-Poincaré Technique
   2.4 The Method of Multiple Scales
      2.4.1 Second-Order Real-Valued System
      2.4.2 First-Order Real-Valued System
      2.4.3 First-Order Complex-Valued System
   2.5 Variation of Parameters
   2.6 The Method of Averaging

----------------------------------------------------------
Chapter 3: Systems with Quadratic and Cubic Nonlinearities
----------------------------------------------------------
   3.1 Nondimensional Equation of Motion
   3.2 Straightforward Expansion
   3.3 The Lindstedt-Poincaré Technique
   3.4 The Method of Multiple Scales
      3.4.1 Second-Order Real-Valued System
      3.4.2 First-Order Real-Valued System
      3.4.3 First-Order Complex-Valued System
   3.5 The Method of Averaging
   3.6 The Generalized Method of Averaging
   3.7 The Krylov-Bogoliubov-Mitropolsky Technique
   3.8 The Method of Normal Forms

------------------------------------------------------
Chapter 4: Forced Oscillations of the Duffing Equation
------------------------------------------------------
   4.1 Straightforward Expansion
   4.2 The Method of Multiple Scales
      4.2.1 Preliminaries
      4.2.2 Primary Resonance
      4.2.3 Secondary Resonances Due to Cubic Nonlinearities
      4.2.4 Secondary Resonances Due to Quadratic Nonlinearities
      4.2.5 First-Order Real-Valued System
      4.2.6 First-Order Complex-Valued System
      4.2.7 The Procedure MMS1
   4.3 The Generalized Method of Averaging
   4.4 The Method of Normal Forms

--------------------------------------------------
Chapter 5: Higher-Order Approximations for Systems 
           with Internal Resonances
--------------------------------------------------
   5.1 Euler-Lagrange Equations
   5.2 Method of Multiple Scales
      5.2.1 Second-Order Real-Valued System
      5.2.2 First-Order Real-Valued System
      5.2.3 First-Order Complex-Valued System
   5.3 Method of Normal Forms
   5.4 Generalized Method of Averaging

---------------------------------------------
Chapter 6: Forced Oscillators of Systems with 
           Finite Degrees of Freedom
---------------------------------------------
   6.1 Externally Excited Linearly Uncoupled Systems
   6.2 Parametrically Excited Linearly Coupled Systems

-------------------------------------------------------
Chapter 7: Continuous Systems with Cubic Nonlinearities
-------------------------------------------------------
   7.1 Solvability Conditions and the Concept of Adjoint
   7.2 Hinged-Clamped Beam
      7.2.1 EOM and BC's
      7.2.2 Direct Attack of the Continuous Problem
      7.2.3 Discretization of the Continuous Problem
      7.2.4 Method of Time-Averaged Lagrangian
   7.3 Cantilever Beam
      7.3.1 EOM and BC's
      7.3.2 Direct Attack of the Continuous Problem
      7.3.3 Discretization of the Continuous Problem
      7.3.4 Method of Time-Averaged Lagrangian

------------------------------------------------
Chapter 8: Continuous Systems with Quadratic and 
           Cubic Nonlinearities
------------------------------------------------
   8.1 Buckled Beams
      8.1.1 Postbuckling Deflection
      8.1.2 Perturbation Analysis
      8.1.3 The Procedure MMSDirect11
      8.1.4 Three-to-One Internal Resonances Between the First Two Modes
      8.1.5 One-to-One and Three-to-One Internal Resonances Between 
            the First and Third Modes
      8.1.6 One-to-One and Three-to-One Internal Resonances Between 
            the First and Fourth Modes
   8.2 Circular Cylindrical Shells
      8.2.1 First-Order Solution
      8.2.2 Second-Order Solution
      8.2.3 Solvability Conditions
   8.3 Near-Square Plates
      8.3.1 First-Order Solution
      8.3.2 Second-Order Solution
      8.3.3 Solvability Conditions
      8.3.4 Mixed Approach

------------------------------------------------------
Chapter 9: Higher Approximations of Continuous Systems 
           Having Two-to-One Internal Resonances
------------------------------------------------------
   9.1 Two-Mode Interactions in Buckled Beams
      9.1.1 First-Order Solution
      9.1.2 Second-Order Solution
      9.1.3 Solvability Conditions
   9.2 Four-Mode Interactions in Suspended Cables
      9.2.1 First-Order Solution
      9.2.2 Second-Order Solution
      9.2.3 Solvability Conditions


***********
Bug Reports
***********

If you experience something you think might 
be a bug in the book, please report it by 
sending a message to cchin@vt.edu. 
Describe what you did, what happened, any error messages
Maple gave, what kind of computer you have, 
which operating system you're using,
and anything else you think might be relevant.
Dr. Chin will respond to you as soon as he can.


****************
Developer's Note
****************

From time to time, everyone comes up with 
an idea they'd like to see how that can be 
implemented in Maple.
If you come across an idea that you think 
might make a nice enhancement to the upcoming versions
of dynamics related books with Maple, 
your input is always welcome.  Please send 
any suggestions or requests for new features 
to cchin@vt.edu.

All the inputs you provide to Dynamics Press, Inc. will
be considered in the upcoming books or packages so that
we all can share with everyone else's experiences.
We offer free consultation for Maple related problems.
Please feel free to contact Dr. Char-Ming Chin (cchin@vt.edu)
in this regard.

