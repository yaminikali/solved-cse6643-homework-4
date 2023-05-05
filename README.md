Download Link: https://assignmentchef.com/product/solved-cse6643-homework-4
<br>



Notice: For the computational problems, you must design your own ways, such as using tables and plots etc, to present the results you obtain. And you must show the procedure you take, and explain the results you get, and draw conclusions if you have any. Computer code is not considered as an explanation. Please upload your code in T-square, and return your HW in class on or before the Due date.

<ul>

 <li><strong>Problem 1</strong>: If one writes the following MATLAB script,</li>

</ul>

[<em>U,S,V </em>] = <em>svd</em>(<em>A</em>); <em>S </em>= <em>diag</em>(<em>S</em>); <em>tol </em>= <em>max</em>(<em>size</em>(<em>A</em>)) ∗ <em>eps</em>;

<em>r </em>= <em>sum</em>(<em>S &gt; tol</em>);

<em>S </em>= <em>diag</em>(<em>ones</em>(<em>r,</em>1)<em>./S</em>(1 : <em>r</em>));

<em>X </em>= <em>V </em>(:<em>,</em>1 : <em>r</em>) ∗ <em>S </em>∗ <em>U</em>(:<em>,</em>1 : <em>r</em>)<sup>0</sup>;

What does this program compute? You must show the steps on how you get your answer. Here <em>eps </em>is the machine precision used in MATLAB. For this question, you may use MATLAB help to find out the meaning of each built-in function if you are not familiar with MATLAB.

<ul>

 <li><strong>Problem 2</strong>: Given two matrices</li>

</ul>

<em> .</em>

If one uses Jacobi iteration to solve linear systems <em>A~x </em>= <em><sup>~</sup>b </em>and <em>B~x </em>= <em><sup>~</sup>b </em>respectively, does it converge? What about Gauss-Seidel? You must justify your answer.

<ul>

 <li><strong>Problem 3</strong>: Let <em>~r<sub>j </sub></em>be the residual vector computed in the steepest descent algorithm, show that <em>~r<sub>j </sub></em>and <em>~r<sub>j</sub></em><sub>+1 </sub>are orthogonal.</li>

 <li><strong>Problem 4</strong>: Use the symmetric <em>m</em>×<em>m </em>Toeplitz matrix <em>T </em>given in Problem 4 of HW2 to perform the following computations. Write your own code for Jacobi, Gauss-Seidel and SOR (with different relaxation parameter <em>ω</em>) iterations to solve the linear system</li>

</ul>

with <em>µ </em>= 5 and <em>µ </em>= −5 respectively. <em>b </em>is a randomly generated <em>m</em>-dimensional vector. Compare the solutions and the speed for <em>m </em>= 100<em>,</em>200<em>,</em>400<em>,</em>800<em>,</em>···.

<ul>

 <li><strong>Problem 5</strong>: Use the matrix <em>A</em>, with <em>λ </em>= 0 and <em>λ </em>= 2 respectively, and the vector <em><sup>~</sup>b </em>from of Problem 5 in HW1 to finish the following work. Solve the linear system</li>

</ul>

<em>A~x </em>=<em><sup>~</sup>b</em>

by the following methods:

<ul>

 <li>Steepest Descent Method,</li>

 <li>Conjugate Gradient Method.</li>

</ul>

You need to test your code with different size (<em>n </em>= 100<em>,</em>200<em>,</em>400<em>,</em>800<em>,</em>1600<em>,</em>3200 or larger if your computer permits) for both parts and comment on the results you obtain.

Hint: you must find ways to demonstrate how the computation cost is associated the size of the system, and how to compare the numerical solutions with the exact solution if you can find it.

2