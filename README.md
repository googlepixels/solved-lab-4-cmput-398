Download Link: https://assignmentchef.com/product/solved-lab-4-cmput-398
<br>
<h1>Objective</h1>

It this lab you will implement three versions of matrix multiplication. The first implementation will be a C version that runs on the CPU, the second will be basic dense matrix multiplication routine written in CUDA, and the third will be a tiled dense matrix multiplication routine using shared memory.

This lab will be submitted as one zipped file through <a href="https://eclass.srv.ualberta.ca/portal/">eclass</a><a href="https://eclass.srv.ualberta.ca/portal/">.</a> Details for submission are at the end of the lab.

<h1>Instructions</h1>

Edit the code where the TODOs are specified and perform the following:

<ul>

 <li>Allocate device memory</li>

 <li>Copy host memory to device</li>

 <li>Initialize thread block and kernel grid dimensions</li>

 <li>Invoke CUDA kernel</li>

 <li>Copy results from device to host</li>

 <li>Deallocate device memory</li>

 <li>Implement the CPU matrix-matrix multiplication routine</li>

 <li>Implement the basic GPU matrix-matrix multiplication routine</li>

 <li>Implement the matrix-matrix multiplication routine using shared memory and tiling</li>

</ul>




<h1>Local Setup Instructions</h1>

Steps:

<ol>

 <li>Download “Lab4.zip”.</li>

 <li>Unzip the file.</li>

 <li>Open the Visual Studios Solution in Visual Studios 2013.</li>

 <li>Build the project. Note the project has two configurations.

  <ol>

   <li>Debug</li>

   <li>Submission</li>

  </ol></li>

</ol>

But make sure you have the “Submission” configuration selected when you finally submit.

<ol start="5">

 <li>Run the program by pressing the following button:</li>

</ol>




Make sure the “Debug” configuration is selected and the project you wish to run is selected in the “Solution Explorer”. To select the project just make sure you click on it before you run. The title of the program is printed at the top of the output console if you are unsure.

Running the program in Visual Studios will run one of the tests located in “Dataset/Test”.

<h1>Testing</h1>

To test run all tests located in “Dataset/Test”, first build the project with the “Submission” configuration selected. Make sure you see the “Submission” folder and all three executables are in the folder: CPU_MatMul.exe, GPU_MatMul.exe, and OPT_MatlMul.exe.  If you are missing one of the executables because of build errors the test script should still work.

To run the tests, click on “Testing_Script.bat”. This will take a couple of seconds to run and the terminal should close when finished. The output is saved in “Marks.js”, but to view the calculated grade open “Grade.html” in a browser. If you make changes and rerun the tests, then make sure you reload “Grade.html”. You can double check with the timestamp at the top of the page.

In the test script if GPU_MatMul.exe fails then OPT_MatMul.exe will fail since the goal is to see the speed up between the basic matrix multiplication and the tiled matrix multiplication. See the Mark Breakdown for more information.


