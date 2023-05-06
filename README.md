Download Link: https://assignmentchef.com/product/solved-ee4371-assignment3a-stacks-recursion
<br>



<ol>

 <li>Read Chapter 3 of Tanenbaum</li>

 <li>Read Chapter 2 of Aho, Hopcroft and Ullman</li>

 <li>Consider the knapsack problem in Aho:</li>

</ol>

Given a set of objects with weights, we need to select a subset of these objects so that their total weight is exactly <em>W</em>. <em>W </em>and <em>w<sub>i </sub></em>are positive integers, and <em>N </em>is given.

(a) Following the pseudocode below from Aho, write the C code to implement this problem.

Boolean knapsack(int W,int i){ if W==0

return True

else if W&lt;0 or i&gt;=N

return False

else if knapsack(W-w[i],i+1)

print w[i] return True

else return knapsack(W,i+1)

end }

<ul>

 <li>Use a static scalar integer, count, to accumulate the number of times knapsack is called.</li>

 <li>Write a main program that randomly generates 10<sup>4 </sup><em>N </em>(uniform in 1 to 20), <em>W </em>(uniform in 0 to <em>N</em><sup>2</sup><em>/</em>2) and the <em>w<sub>i </sub></em>values (uniformly random in 0 to <em>N</em>). For each such set, determine the number of times knapsack was called. Write out a table as follows:</li>

</ul>

<table width="123">

 <tbody>

  <tr>

   <td width="35"><em>N</em></td>

   <td width="42">Min</td>

   <td width="45">Max</td>

  </tr>

  <tr>

   <td width="35">1</td>

   <td width="42">1</td>

   <td width="45">1</td>

  </tr>

  <tr>

   <td width="35">…</td>

   <td width="42">…</td>

   <td width="45">…</td>

  </tr>

  <tr>

   <td width="35">20</td>

   <td width="42">?</td>

   <td width="45">?</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>In the report, include the output of Min and Max vs <em>N </em>shown above. Determine the scaling (is it logarithmic, polynomial (if so order), or exponential (exponent?)) Can you justify the scaling?</li>

</ul>