Download Link: https://assignmentchef.com/product/solved-cta200-assignment-2
<br>






Submit all of your code in a .ipynb file. Please clear all output before commiting your file to Github. You will also submit a .tex file, as described in Question 4. You can see the .tex file for this assignment as a sample of how to get started. I also suggest that those of you new to Latex try out the Overleaf cloud based Latex editor.

<h1>[2] Question 1</h1>

The numerical approximation of the derivative of a mathematical function <em>f </em>evaluated as <em>x</em><sub>0 </sub>can be written as:

Where <em>h </em>is some small “step”. This is found by looking at the Taylor series of <em>f</em>(<em>x</em>) and taking <em>h </em>→ 0. A better approximation, when <em>h </em>is finite (rather than infinitessimal) is:

Make a python function that has the form def deriv(f, x0, h) that takes in a python function, and returns the approximation of the derivative at x0 using stepsize h for each of the methods. Use your functions to take the derivative of the function <em>f</em>(<em>x</em>) = <em>sin</em>(<em>x</em>) for <em>x</em><sub>0 </sub>= 0<em>.</em>1 using a variety of values of <em>h &lt; </em>1. Plot the error compared to the analytical derivative (ie abs(d numerical – d analytic) / d analytic) as a function of <em>h </em>for each method on the same loglog plot. What do you notice? What does the slope represent?

<h1>[3] Question 2</h1>

For each point in the complex plane <em>c </em>= <em>x</em>+<em>iy</em>, with −2 <em>&lt; x &lt; </em>2 and −2 <em>&lt; y &lt; </em>2, set <em>z</em><sub>0 </sub>= 0 and iterate the equation <em>z<sub>i</sub></em><sub>+1 </sub>= <em>z<sub>i</sub></em><sup>2 </sup>+ <em>c</em>. Note what happens to the <em>z<sub>i</sub></em>’s: some points will remain bounded in absolute value |<em>z</em>|<sup>2 </sup>= &lt;(<em>z</em>)<sup>2 </sup>+=(<em>z</em>)<sup>2</sup>, while others will run off to infinity. Make an image in which your points <em>c </em>that diverge are given one color and those that stay bounded are given another. Make a second image where the points are coloured by a colourscale that indicates the iteration number at which the given point diverged.

<h1>[3] Question 3</h1>

The SIR model is a simple mathematical model of disease spread in a population. The model divides a fixed population of size <em>N </em>into three groups, which vary as a function of time, <em>t</em>:

<ul>

 <li><em>S</em>(<em>t</em>) is those that are susceptible but not yet infected • <em>I</em>(<em>t</em>) is the number of infected individuals</li>

</ul>

1

<ul>

 <li><em>R</em>(<em>t</em>) is those individuals that have recovered and are now immune</li>

</ul>

The model can be described by a set of 3 first order differential equations for each of the variables as

(1)

(2)

(3)

Using the ODE integrator of your choice (must be callable in Python, we recommend using Scipy as will be covered in lecture on Friday), integrate the equations with <em>N </em>= 1000 from <em>t </em>= 0 to <em>t </em>= 200 for various values of <em>γ </em>and <em>β </em>(at least 3-4 values, justify your choices physically).

Use the initial condition <em>I</em>(0) = 1<em>,S</em>(0) = 999<em>,R</em>(0) = 0 (you can also experiment with other initial conditions if you wish). Plot the curves for <em>S,I,R </em>on the same figure with a legend. make separate plots for each choice of the parametersi (hint: use the subplots() command).

Bonus (+0.5 mark): Add a 4th parameter <em>D </em>for deaths and justify the addition of a 4th differential equation as well as any RHS terms that must be changed on the initial 3 equations. Integrate the new set of equations for some choice of parameters and comment on the results compared to the SIR model.

<h1>[2] Question 4</h1>

To practice using the LaTex, markup language, we would like you to writeup your results in a .tex file and submit both the LaTex code and the associated PDF. For each of the questions, save and insert your figures into a tex file and write a 1 paragraph methods section, which briefly describes what you did as well as a 1 paragraph analysis section which describes what you see in the results.


