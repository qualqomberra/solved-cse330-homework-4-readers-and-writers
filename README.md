Download Link: https://assignmentchef.com/product/solved-cse330-homework-4-readers-and-writers
<br>



<strong>1.Readers and Writers:</strong>

Using the semaphores you have implemented, implement the Readers and Writers Problem.

<strong>2.Test case:</strong>

Have a global variable <em>int i</em> and set it to 0 initially.

The readers should read the variable value and print the current value of the variable. Each reader should print the variables twice. The writers should write their ids in the variable. The writer should write in one go and then verify that the correct Id is written into the variable.

Readers and writers do not run in infinite loop, but reader reads twice while writer writes and then again verifies.

The reader yields after one read and then finishes after the second read.

<ul>

 <li>On the <em>first</em> read the reader prints:

  <ul>

   <li><em>Printf(“
 This is the %d th reader reading value i = %d for the first time 
”, readerID, i );</em></li>

  </ul></li>

 <li><em>On the second </em>read the reader prints:

  <ul>

   <li><em>Printf(“
 This is the %d th reader reading value i = %d for the second time 
”, readerID, i );</em></li>

  </ul></li>

</ul>

The writer yields after the first write and then exits after the verification step.

<ul>

 <li>On the <em>first</em> write the writer prints:

  <ul>

   <li><em>Printf(“
 This is the %d th writer writing value i = %d 
”, writerID, i );</em></li>

  </ul></li>

 <li>On the <em>verification</em> loop the writer should print:

  <ul>

   <li><em>Printf(“
 This is the %d th writer verifying value i = %d 
”, writerID, i );</em></li>

  </ul></li>

</ul>

The test case will be in the following format

2,2

1

-1

2

-2

The first line will have number of readers and number of writers consecutively, followed by R+W numbers showing the ready Q. The positive numbers are readers, the negative numbers are writers. Always have the initial scratch pad variable i = 0;

In this case the output will be

This is the 1 th reader reading value i = 0 for the first time




This is the 1 th reader reading value i = 0 for the second time




This is the 1 th writer writing value i = 1




This is the 1 th writer verifying value i = 1




This is the 2 th reader reading value i = 1 for the first time




This is the 2 th reader reading value i = 1 for the second time




This is the 2 th writer writing value i = 2




This is the 2 th writer verifying value i = 2




Your project must consist of 5 files




<ol>

 <li>h (uses ucontext.h)</li>

</ol>




<ol start="2">

 <li>h (includes TCB.h)</li>

</ol>




<ol start="3">

 <li>h (includes q.h)</li>

</ol>




<ol start="4">

 <li>h (includes threads.h) if you have written one.</li>

</ol>




<ol start="5">

 <li>proj-4.c (includes threads.h)</li>

</ol>

(make sure the compile command, “gcc proj-4.c” does the correct compilation).




All 5 files are to be ZIPPED into one zip file and uploaded in Canvas. The name of this file should reflect the name of the student (abbreviated, do not make it too long).




<strong>Note: Grading is on Ubuntu. It is in your interest to make sure the program compiles and runs in the target test platform.</strong>

<strong> </strong>




<strong>Testing your code on grading test cases</strong>

Grading test cases are different from the test cases provided.

To test your code against grading testcases follow these steps:




Put the four files q.h tcb.h threads.h and proj-4.c in one zip file and name the file




YOUR LAST NAMEProject4.zip (no gaps)

The resulting file should be YOUR LAST NAMEProject4.zip

Make sure there are no folders inside the zip

For example BanerjeeProject4.zip