Download Link: https://assignmentchef.com/product/solved-final-exam-programming
<br>
<h2><a id="user-content-timing-and-general-instructions" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final#timing-and-general-instructions" aria-hidden="true"></a>Timing and general instructions</h2>

You have <strong>1 hour 50 minutes</strong> to complete the programming part of the final exam. This is a closed notes exam so you should not open any website other than the Titanium exam page. Do not communicate with your classmates or look at their screens. Direct all your questions to the instructor or lab assistant only.

You are allowed to view your own study guide and use paper for scratch work that will be provided for you.

You are free to use any editor and the command line on Tuffix to write, compile, and test your program. The instructors will use <code>clang++</code> to check your programs so make sure your code works with that compiler.

You are expected to have used the programming environment during our lab sessions so instructors and lab assistants will not answer questions regarding interpretting syntax errors or debugging code.

<h2><a id="user-content-problem-and-points" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final#problem-and-points" aria-hidden="true"></a>Problem and points</h2>

There are three programming problems that you need to complete.

<ol>

 <li>Courses (<em>15 points</em>)</li>

 <li>Organization (<em>25 points</em>)</li>

 <li>Student (<em>10 points</em>)</li>

</ol>

<h1><a id="user-content-submission" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final#submission" aria-hidden="true"></a>Submission</h1>

Your answers will be submitted through GitHub. You can push your code as many times as you want before the end of the final exam. We will check the last version that you pushed.

When you are done, verify you have pushed your code properly on GitHub. Simply refresh your GitHub repo and click on the individual files to see if they have been changed.

On Titanium, click on the <code>Add submission</code> button in the midterms page. Provide the URL for your GitHub repo containing the final exam and click on <code>Save changes</code>. Finally click on <code>Submit assignment</code>.

Before leaving the room, please approach the instructor who will verify that you submitted your exam properly. Also turn in your scratch paper and study guide to the instructor.




<h1>Course Registration</h1>

<h2><a id="user-content-course" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob01#course" aria-hidden="true"></a>Course</h2>

Implement the class named <code>Course</code> which has the private variables (data members) <code>int course_num_</code>, <code>std::string course_name_</code>, and <code>std::string department_</code>.

Please note that the <code>course_name_</code> and <code>department_</code> are of arbitrary length and can contain spaces (i.e. Computer Science). Include accessor and mutator functions for each variable (data member).

Create an overload constructor (nondefault constructor) that takes in three parameters to set the values for <code>course_num_</code>, <code>course_name_</code>, and <code>department_</code>. Create a default constructor that assigns <code>121</code> to <code>course_num_</code>, <code>"Object oriented programming"</code> to <code>course_name_</code> and <code>"Computer Science"</code> to <code>department_</code>.

Create a <code>display</code> member function that shows on screen information about the course. Below is an example of how it might look like:

<pre><code>Course number: 121Course name: Object oriented programmingDepartment: Computer Science</code></pre>

Place your class in <code>course.hpp</code>. No need to create <code>course.cpp</code>.

<h2><a id="user-content-dynamic-memory-allocation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob01#dynamic-memory-allocation" aria-hidden="true"></a>dynamic memory allocation</h2>

In the <code>main</code> function, you are asked to dynamically allocate an array of <code>Course</code> objects whose size depends on the user’s input. It will also ask the user to provide values for each course, that you will use to set the values of the <code>Courses</code> inside your array. Finally, it will ask you to display information about each course added by the user to the screen.

More detailed instructions are found inside <code>main.cpp</code>.

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob01#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this problem. Assuming you have pulled the code inside of <code>/home/student/final</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd final</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code in <code>main.cpp</code> into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp -o main./main</code></pre>

<h1><a id="user-content-submission" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob01#submission" aria-hidden="true"></a>Submission</h1>

<ol>

 <li>When everything runs correctly, let’s copy your code into the Github repository. The first step is to add your code to what is called the staging area using git’s <code>add</code> command. The parameter after <code>add</code> is the name of the file you want to add.<pre><code>git add main.cpp course.hpp</code></pre></li>

 <li>Once everything is in the staging area, we use the <code>commit</code> command to tell git that we have added everything we need into the staging area.<pre><code>git commit</code></pre></li>

 <li>In case it asks you to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and Github username.<pre><code>git config --global user.email "<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="116564777768517262643f77647d7d7463657e7f3f747564">[email protected]</a>"git config --global user.name "Tuffy Titan"</code></pre>When you’re done, make sure you type <code>git commit</code> again.</li>

 <li>Git will ask you to describe what you have added to the staging area. By default, you will use a command-line based editor called <em>nano</em>. Go ahead and provide a description then press <kbd>Ctrl</kbd> + <kbd>x</kbd> to exit. Press <kbd>Y</kbd> to confirm that you want to make changes and then press <kbd>Enter</kbd>.</li>

 <li>Lets push all changes to the Github repository using git’s <code>push</code> command. Provide your Github username and password when you are asked.<pre><code>git push</code></pre></li>

 <li>When you finish the exercise, go back to Titanium and click on the <code>Add submission</code> button in the lab exercise page. Provide a short message in the text area such as “finished lab exercise” and click on <code>Save changes</code>. Finally click on <code>Submit assignment</code> to inform your instructor that you are done.</li>

</ol>

5/5 - (1 vote)

<main id="js-repo-pjax-container" data-pjax-container="">







</main>

<article class="markdown-body entry-content p-5">

 <h1>Organization Positions</h1>

 Create a program that stores and manages information about the positions in an organization.

 <h2><a id="user-content-person" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob02#person" aria-hidden="true"></a>Person</h2>

 First, create a <code>Person</code> class that has name, address, and phone number data members.

 Create a nondefault constructor that accepts the values that will be assigned to name (<code>std::string</code>), address (<code>std::string</code>), and phone number (<code>std::string</code>) as parameters to the corresponding data members.

 Create a default constructor that sets name to <code>"Unidentified"</code>, address to <code>"Somewhere"</code>, and phone number to <code>1-800-000-0000</code>.

 Provide accessors and mutators for all of the class’ data members.

 Create a <code>display</code> member function that displays information about the <code>Person</code> on the console. Take note that it does not take any parameters and does not return any value. For example, the default constructor might show the following information on screen:

 <pre><code>UnidentifiedSomewhere1-800-000-0000</code></pre>

 <h2><a id="user-content-organization" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob02#organization" aria-hidden="true"></a>Organization</h2>

 Create an <code>Organization</code> class that has a name, president, vice president and treasurer as data members. The positions president, vice president, and treasurer are all <code>Person</code> objects.

 Create a non-default constructor that accepts a value that will be assigned to the name (<code>std::string</code>) of the organization.

 Create a default constructor that sets name to <code>"Unknown"</code>.

 Create accessors and mutators for all data members (i.e., name, president, vice president and treasurer).

 <h3><a id="user-content-get_position" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob02#get_position" aria-hidden="true"></a>get_position</h3>

 In the <code>Organization</code> class, create a <code>get_position</code> member function that accepts a name (<code>std::string</code>) parameter. The member function will check whether the name provided is the name of the president, vice president or treasurer and return an <code>std::string</code> describing the position. That means, it will return <code>"president"</code>, <code>"vice president"</code> or <code>"treasurer"</code>. However, if the name is not any of the three positions, it should return <code>"not an officer"</code>.

 <h2><a id="user-content-other-instructions" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob02#other-instructions" aria-hidden="true"></a>Other instructions</h2>

 Complete the <code>main</code> function as described in the comments inside the file.

 Place your classes in <code>organization.hpp</code>. Member functions that take more than five lines or use complex constructs should have their function prototype in <code>organization.hpp</code> and implementation in <code>organization.cpp</code>.

 <h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob02#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

 Open the terminal and navigate to the folder that contains this problem. Assuming you have pulled the code inside of <code>/home/student/final</code> and you are currently in <code>/home/student</code> you can issue the following commands

 <pre><code>cd final</code></pre>

 You also need to navigate into the problem you want to answer. To access the files needed to answer problem 2, for example, you need to issue the following command.

 <pre><code>cd prob02</code></pre>

 When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob02</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob03</code> for example.

 <pre><code>cd ..cd prob03</code></pre>

 Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code saved in<code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

 <pre><code>clang++ -std=c++17 main.cpp organization.cpp -o main./main</code></pre>

 <h1><a id="user-content-submission" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob02#submission" aria-hidden="true"></a>Submission</h1>

 <ol>

  <li>When everything runs correctly, let’s copy your code into the Github repository. The first step is to add your code to what is called the staging area using git’s <code>add</code> command. The parameter after <code>add</code> is the name of the file you want to add.<pre><code>git add main.cpp organization.hpp organization.cpp</code></pre></li>

  <li>Once everything is in the staging area, we use the <code>commit</code> command to tell git that we have added everything we need into the staging area.<pre><code>git commit</code></pre></li>

  <li>In case it asks you to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and Github username.<pre><code>git config --global user.email "<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="f3878695958ab3908086dd95869f9f9681879c9ddd969786">[email protected]</a>"git config --global user.name "Tuffy Titan"</code></pre>When you’re done, make sure you type <code>git commit</code> again.</li>

  <li>Git will ask you to describe what you have added to the staging area. By default, you will use a command-line based editor called <em>nano</em>. Go ahead and provide a description then press <kbd>Ctrl</kbd> + <kbd>x</kbd> to exit. Press <kbd>Y</kbd> to confirm that you want to make changes and then press <kbd>Enter</kbd>.</li>

  <li>Lets push all changes to the Github repository using git’s <code>push</code> command. Provide your Github username and password when you are asked.<pre><code>git push</code></pre></li>

  <li>When you finish the exam, go back to Titanium and click on the <code>Add submission</code> button in the lab exercise page. Provide a short message in the text area such as “finished lab exercise” and click on <code>Save changes</code>. Finally click on <code>Submit assignment</code> to inform your instructor that you are done.</li>

 </ol>

</article>

<ul class="list-style-none d-flex flex-wrap ">

 <li class="mr-3">© 2019 GitHub, Inc.</li>

 <li class="mr-3"><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>

 <li class="mr-3"><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>

 <li class="mr-3"><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>

 <li class="mr-3"><a href="https://githubstatus.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>

 <li><a href="https://help.github.com/" data-ga-click="Footer, go to help, text:help">Help</a></li>

</ul>

<ul class="list-style-none d-flex flex-wrap ">

 <li class="mr-3"><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact GitHub</a></li>

 <li class="mr-3"><a href="https://github.com/pricing" data-ga-click="Footer, go to Pricing, text:Pricing">Pricing</a></li>

 <li class="mr-3"><a href="https://developer.github.com/" data-ga-click="Footer, go to api, text:api">API</a></li>

 <li class="mr-3"><a href="https://training.github.com/" data-ga-click="Footer, go to training, text:training">Training</a></li>

 <li class="mr-3"><a href="https://github.blog/" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>

 <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

</ul>

<h1>Student Class</h1>

Create a class called <code>Student</code> which inherits from the <code>Person</code> class that you created in <em>prob02</em>. The <code>Student</code> class has the private variables (data members) <code>int student_id_</code> and <code>std::string major_</code>.

Create accessors and mutators for all data members in the <code>Student</code> class. Create a non-default constructor that accepts the following arguments in the given order: <code>std::string name</code>, <code>std::string address</code>, <code>std::string phone_num</code>, <code>int student_id</code>, <code>std::string major</code>

In the <code>Student</code> class, override the <code>display</code> member function to display all information about the student to the console as such:

<pre><code>Joan Smith123 N. Main St. Orange, CA 92874562-744-852412345Computer Science</code></pre>

In the <code>main</code> function, create a <code>Student</code> object by calling the non-default constructor with the same information as the example above. Extra points if you use dynamically allocate the <code>Student</code> object in the heap. Call the <code>display</code> member function to print information about the student to the console.

You need to create the <code>Student</code> class inside <code>person.hpp</code> and modify the <code>main</code> function inside <code>main.cpp</code>. You do not need to create other files aside from these two.

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob03#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this problem. Assuming you have pulled the code inside of <code>/home/student/midterm</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd midterm</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 3, for example, you need to issue the following command.

<pre><code>cd prob03</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob03</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob01</code> for example.

<pre><code>cd ..cd prob01</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code saved in <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp -o main./main</code></pre>

<h1><a id="user-content-submission" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/copy/Exams/Final/prob03#submission" aria-hidden="true"></a>Submission</h1>

<ol>

 <li>When everything runs correctly, let’s copy your code into the Github repository. The first step is to add your code to what is called the staging area using git’s <code>add</code> command. The parameter after <code>add</code> is the name of the file you want to add.<pre><code>git add main.cpp person.hpp</code></pre></li>

 <li>Once everything is in the staging area, we use the <code>commit</code> command to tell git that we have added everything we need into the staging area.<pre><code>git commit</code></pre></li>

 <li>In case it asks you to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and Github username.<pre><code>git config --global user.email "<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="5f2b2a3939261f3c2c2a71392a33333a2d2b3031713a3b2a">[email protected]</a>"git config --global user.name "Tuffy Titan"</code></pre>When you’re done, make sure you type <code>git commit</code> again.</li>

 <li>Git will ask you to describe what you have added to the staging area. By default, you will use a command-line based editor called <em>nano</em>. Go ahead and provide a description then press <kbd>Ctrl</kbd> + <kbd>x</kbd> to exit. Press <kbd>Y</kbd> to confirm that you want to make changes and then press <kbd>Enter</kbd>.</li>

 <li>Lets push all changes to the Github repository using git’s <code>push</code> command. Provide your Github username and password when you are asked.<pre><code>git push</code></pre></li>

 <li>When you finish the exercise, go back to Titanium and click on the <code>Add submission</code> button in the lab exercise page. Provide a short message in the text area such as “finished lab exercise” and click on <code>Save changes</code>. Finally click on <code>Submit assignment</code> to inform your instructor that you are done.</li>