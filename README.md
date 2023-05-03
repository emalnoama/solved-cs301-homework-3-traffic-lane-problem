Download Link: https://assignmentchef.com/product/solved-cs301-homework-3-traffic-lane-problem
<br>
Traffic lane problem Consider a roadway with three traffic lanes, each consisting of cells as shown in the figure below.

The lanes are denoted by columns <em>c</em><sub>1</sub>, <em>c</em><sub>2 </sub>and <em>c</em><sub>3</sub>. Each lane is marked with levels <em>l</em><sub>1</sub>, <em>l</em><sub>2</sub>, …, <em>l<sub>n</sub></em>, so the cells are denoted by pairs of lanes and levels. For instance, (<em>l</em><sub>1</sub><em>,c</em><sub>2</sub>) denotes the cell at level 1 of the traffic lane 2. The roadway has some obstacles; the cells covered by these obstacles are colored as red in the figure.

Initially, there is a car at cell (0<em>,</em>1) of this roadway. The car can move forward with the goal of reaching a cell at level <em>l<sub>n</sub></em>, obeying the following rules:

Rule 1 The car can not move through the cells covered by obstacles.

Rule 2 The car has to move forward to a neighboring cell at the next level. For instance, if the car is located at a cell (<em>l<sub>i</sub>,c</em><sub>0</sub>) then it has to move straight to (<em>l<sub>i</sub></em><sub>+1</sub><em>,c</em><sub>0</sub>) or diagonally to (<em>l<sub>i</sub></em><sub>+1</sub><em>,c</em><sub>1</sub>).

Therefore, the car cannot move between the cells at the same level, and it cannot go back to a cell at the previous level.

Rule 3 The car cannot jump over cells. Therefore, it cannot go from <em>c</em><sub>0 </sub>to <em>c</em><sub>2 </sub>or from <em>c</em><sub>2 </sub>to <em>c</em><sub>0 </sub>in one step. It cannot jump from level <em>l<sub>i </sub></em>to <em>l<sub>j </sub></em>where <em>j &gt; i </em>+1 or <em>j &lt; i </em>−1.

Note that, according to these rules, the car can move to one of the three cells at the next level only if it is at <em>c</em><sub>1</sub>.

The traffic lane problem aims to find a route for the car to reach one of the cells at the last level, so as to minimize the number of traffic lane changes.

Submit PDF          Write a report including the following:

<ul>

 <li>Recursive formulation of the traffic lane problem: Identify the subproblems,observe the optimal substructure property and the overlapping computations, and then define the problem recursively.</li>

 <li>Pseudocode of a naive recursive algorithm based on your recursive formulation, and its complexity analysis (i.e., the asymptotic time and space complexity).</li>

 <li>Pseudocode of a recursive algorithm that builds solutions to your recurrencefrom top down with memoization, and its complexity analysis (i.e., the asymptotic time and space complexity).</li>

 <li>Pseudocode of an iterative algorithm that builds solutions to your recurrencefrom bottom up, and its complexity analysis (i.e., the asymptotic time and space complexity).</li>

 <li>Experimental evaluations of these three algorithms: plot the results in a graph,and discuss the results (e.g., are they expected or surprising? why?)</li>

</ul>

<h1>Submit Python Code, and Benchmarks</h1>

<ul>

 <li>Implement in Python the three algorithms above, designed to solve the trafficlane problem.</li>

</ul>

The roadway will be presented as an input matrix of size <em>n </em>×3. The entry at the <em>i</em>’th row and <em>j</em>’th column of the matrix is 0, if the cell (<em>l<sub>i</sub>,c<sub>j</sub></em>) is a free cell (i.e., not occupied by an obstacle); otherwise, it is 1.

<ul>

 <li>Create a benchmark suite to test the correctness of your Python programs: take into account the functional testing methods (e.g., white box and lack box testing) while constructing the instances, and test your programs with these instances.</li>

 <li>Create a benchmark suite to test the performance of your Python programs: construct instances of different sizes (e.g., relative to the number of levels), evaluate the performance of your programs in terms of computation times, and plot the results within a graph.</li>

</ul>

Demos Demonstrate that your Python programs correctly compute solutions for your benchmark instances, and for the instances that will be provided by us. Demo day will be announced.

2