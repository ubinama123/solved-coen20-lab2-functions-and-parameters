Download Link: https://assignmentchef.com/product/solved-coen20-lab2-functions-and-parameters
<br>



<em>Topics: Passing parameters, function return values, nested functions, preserving and restoring registers across function calls, calling C functions from assembly.  </em>

Prerequisite Reading: Chapters 1-3

Create an assembly language source code file containing four functions. If the functions were written in C, they would look like the following. (Functions Square and SquareRoot are provided in the main program.)

<table width="623">

 <tbody>

  <tr>

   <td width="312">int32_t Add(int32_t a, int32_t b){return a + b ;}</td>

   <td width="312">int32_t Less1(int32_t a){return a – 1 ;}</td>

  </tr>

  <tr>

   <td width="312">int32_t Square2x(int32_t x){return Square(x + x) ;}</td>

   <td width="312">int32_t Last(int32_t x){return x + SquareRoot(x) ;}</td>

  </tr>

 </tbody>

</table>

Test your functions using the main program downloaded from <a href="http://www.cse.scu.edu/~dlewis/book3/labs/Lab2aMain.c">here</a><a href="http://www.cse.scu.edu/~dlewis/book3/labs/Lab2aMain.c">.</a>  If you code works correctly, the display should look like the image on the right. Press the blue pushbutton to cycle through all the test cases to verify that everything is correct. Color is used to indicate the status of a function:

<table width="78">

 <tbody>

  <tr>

   <td width="78">Gray</td>

  </tr>

  <tr>

   <td width="78">Yellow</td>

  </tr>

  <tr>

   <td width="78">Orange</td>

  </tr>

  <tr>

   <td width="78">Green</td>

  </tr>

  <tr>

   <td width="78">Red</td>

  </tr>

 </tbody>

</table>

<table width="307">

 <tbody>

  <tr>

   <td width="307"><strong>IMPORTANT – The </strong><strong>.thumb_func</strong><strong> directive: </strong>The “.thumb_func” assembler directive specifies that the <u>next</u> label is the entry point of a function that contains instructions from the Thumb subset of the ARM processor and causes the binary representation of instructions that branch to that label to be generated somewhat differently. Thus in a source code file that contains more than one function, it is imperative that you place a .thumb_func directive immediately before the entry point label of <u>every</u> function.</td>

  </tr>

 </tbody>

</table>

Function never called.             Function given in main program.       Function never returns.

Function returning correct value.        Function returning incorrect value.


