Download Link: https://assignmentchef.com/product/solved-met-cs-622-assignment-1
<br>
YOUR PROJECT TITLE AND ACRONYM REPLACE THIS

e.g., PANTRACK: A System for Tracking Pandemics in Iceland

YOUR NAME REPLACES THIS

Assignment 1

For this assignment, you will describe and implement release 1 of your term project. You will incorporate <em>an abstract class</em>, <em>inheritance</em>, <em>upcasting or downcasting</em>, and <em>polymorphism</em>. You are free to choose a project that interests you but if you prefer, the instructor and your facilitator will be happy to suggest a topic. If you are already an experienced developer, this is an opportunity to build a challenging application (check with your facilitator if it requires significant API’s) or discuss research with the instructor. It is OK to name a project with much more scope than you can accomplish in the course (as in the example above): we will not hold you to completing everything associated with it. What we do expect is that you specify and implement a set of do-able requirements within such scope.




Submit this completed Word document. Replace as indicated. Please observe and retain the gray text. Your materials—in black 12-point Times New Roman—should not exceed 5 pages excluding references, figures, and appendices. Use the Appendix sections for additional material if you need to. These will be read only on an as-needed basis.




We want you to develop in Eclipse preferably or else IntelliJ (talk to your facilitator about exceptions). As you code, use JUnit tests whenever possible but certainly by week 2—package-by-package, class-by-class, and method-by-method, except for trivial methods and those requiring I/O. Use non-Junit classes for testing the latter. Keep the evaluation criteria in mind, listed at the end.




For this assignment, you do not need to read data from a file—you can build all data into the code.




Include a ReadMe file describing where to run the application from, and including necessary execution notes. All JUnit tests will be assumed runnable.




<h1>1.1 SUMMARY DESCRIPTION <em>EVALUATION CRITERION (i) APPLIES</em></h1>

One- or two-paragraph overall description of your proposed term project—half-page (12-point Times New Roman) limit. By the end, term projects will incorporate most of the techniques discussed in the course. To do this, you may need to alter the direction of your project or introduce an additional project in future. You may alter this or even replace it as the semester progresses. You will probably find it useful to use your project acronym.

Your response should replace this sentence, as well as the example below.

This project concerns a system for students to learn written material that is between a paragraph and several pages in length. To use the system, called <em>Knowla</em>, students respond to a question by selecting from and ordering a set of fragments (typically sentences). Since material that’s more than a page in length contains too many sentences to re-order, we envision a system that first requires ordering paragraph topics, and after that the sentences within each paragraph. The focus of the term project is the automatic grading of solutions to Knowla tests. This grading system will be called <em>K-Grade</em>.

<h2>1.2 I/O EXAMPLE FROM <em>PROJECTED</em> COMPLETED PROJECT <em>EVALUATION CRITERION (i) APPLIES</em></h2>

Provide an example of projected <em>concrete</em> output for designated input. You will not be held to fulfilling exactly this—it is just explanatory at this point, to indicate where your project is going. We recognize that project direction and details will change as the term progress. This section refers to the project as a whole, not just to what you will produce this week, so we can gain an idea of what you have in mind overall.

Your response should replace this sentence, as well as the example below.




Here is an example of a simple Knowla test.




<strong>Knowla</strong>:

Reconstruct “Humpty Dumpty” from the following set of fragments, inserting punctuation and capitalization. You need to provide only the correct order, e.g., 5, 3, 1, 2

<ol>

 <li>all the king’s horses and all the king’s men</li>

 <li>to glue him back up</li>

 <li>couldn’t put Humpty together again</li>

 <li>Humpty Dumpty sat on a wall</li>

 <li>never were able</li>

 <li>Humpty Dumpty had a great fall</li>

</ol>




<strong>User</strong>: 4, 5, 2




<strong>System</strong>:

Your answer is:

Humpty Dumpty sat on a wall.

Never were able

to glue him back up.




You are correct that line 1 should be fragment 4 (+30%).

Even though “never were able” and “to glue him back up” are not in the poem, you get credit for ordering them correctly (+2%).

Fragment 5 (“never were able”) is not part of the poem. (It is similar to part of the real third line “couldn’t put Humpty together again.”) (-1%)

Fragment 2 (“to glue him back up”) is not part of the poem. (It is similar to part of the real third line “couldn’t put Humpty together again.”) One clue is that “up” does not rhyme with any other ending. (-1%)

Fragment 1, “All the king’s horses and all the king’s men,” should be line 3 in the poem, following “Humpty Dumpty had a great fall.” (-2%)

Fragment 3, “couldn’t put Humpty together again.” should be line 4 in the poem, following “all the king’s horses and all the king’s men.” (-2%)




Your grade is 26%.




<h2>1.3 REQUIREMENTS IMPLEMENTED IN THIS RELEASE <em>EVALUATION CRITERION (ii) APPLIES</em></h2>




Supply <a href="https://docs.google.com/document/d/1eU7eINLDxmrf793D4OF2yGT4ry_SW3GQGoVDYzecGHc/edit?usp=sharing">functional requirements</a> statement that you accomplished for this assignment, i.e., functionality that the application provides for the user. Please state requirement in declarative form, as illustrated in the examples, because here we want to know the functionality intended (<em>what</em>, not <em>how</em>). For example, the following is <em>not</em> a proper functional requirement: <em>TicTac will have a class for O’s and a class for X’s.</em> It is common to mistake design elements like this for requirements. To get started, state what the application will accept as input, like requirement 1.3.1 below.




Keep in mind that the implementation of your requirements will incorporate <em>an abstract class</em>, <em>inheritance</em>, <em>upcasting or downcasting</em>, and <em>polymorphism</em>; that will probably influence the requirements you choose to implement in this assignment. The example material supplied should be deleted before you submit.




<h3>1.3.1 &lt;Your requirement title replaces this&gt; Create Hierarchies</h3>

Your first requirement should replace this, as well as the example below

Knowla shall accept a hierarchy of heading and non-heading fragments (but currently in hard-coded form only).

<h3>1.3.2 &lt;Your requirement title replaces this &gt; Report Fragment Hierarchies</h3>

Your response should replace this, as well as the example below

Knowla shall report all of the heading fragments it possesses with their subheadings to the console.




<h2>1.4 ILLUSTRATIVE OUTPUT FROM IMPLEMENTATION <em>EVALUATION CRITERION (ii) APPLIES</em></h2>

<h3>Provide illustrative output from your implemented application (so far) showing that the requirements have been met. Explain what class.method(s) produce it.</h3>

Your response should replace this, as well as the example below.

The following is produced by <em>FragmentDisplayExample.displayFragmentHierarchyExample()</em>.  <em>HeadingFragment</em> and <em>NonHeadingFragment</em> objects are hard-coded data.

=========FragmentDisplayExample==========

========= Should display 8 items ==========

My Expenses Heading

Taxes Heading

Estate taxes

Income taxes

Housing Heading

Mortgage for housing

Maintenance for housing

Food




3 headings and 5 others.




<h2>1.5 YOUR DIRECTORY</h2>

<h3>Show a screenshot of your directory. This should include a parallel directory of JUnit tests where possible—package-by-package, class-by-class, and method-by-method, except for trivial ones.</h3>




Your response should replace this, as well as the example below.




All methods in the K-Grade example are trivial so far except for ones that perform displays, and these are not suitable for JUnit testing.







<h2>1.6 TECHNIQUES IMPLEMENTED <em>EVALUATION CRITERION (iii) APPLIES</em></h2>

Your implementation should include <em>inheritance</em>, <em>polymorphism</em>, and <em>either an abstract class or </em><em>interface</em> at least once, and in a manner that is useful to your application. Explain where and how you applied these, using the headings below.

<h3>1.6.1 Class model and Sequence Diagram</h3>

Identify where you included <em>inheritance</em>, <em>polymorphism</em>, and <em>abstract classes</em> or <em>interfaces</em> in your class model. Make classes and members <em>static</em> or not as per their intended usage. To do this use tools (e.g., Visio and Lucidchart), PowerPoint, or a combine models as in <a href="https://docs.google.com/spreadsheets/d/1vBmDVtWWh3EX0oehFFLRU0P6eR-fn4d0qVg1-XOUooM/edit?usp=sharing">this example</a> (which you are free to cut and paste from). Insert indications in red (as in <a href="https://docs.google.com/spreadsheets/d/1ZvkerE9FkWHWwVGdzuy7YMBU6oBMFGZbA4sotFETs8Y/edit?usp=sharing">this example</a>) to show where the three features below apply.

Your response should replace this, as well as the example below.




The class model for the K-Grade example is <a href="https://docs.google.com/spreadsheets/d/1vBmDVtWWh3EX0oehFFLRU0P6eR-fn4d0qVg1-XOUooM/edit?usp=sharing">here</a>. <em>Fragment</em> is abstract. Polymorphism occurs in the versions of <em>getType</em>(). The figure includes inheritance.

<h3>1.6.2 Code showing an abstract class or interface</h3>

Show the relevant code (only) and explain why an abstract class or interface is appropriate here. It should be clear where the code is located (class and method).

Your response should replace this, as well as the example below.




There are only two kinds of fragments, so there is no need for the <em>Fragment</em> base class to be concrete since there will be no generic Fragments.

<strong>package</strong> fragments;




// A portion of a text passage, such as a sentence

<table>

 <tbody>

  <tr>

   <td width="46"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>







<strong>public</strong> <strong>abstract</strong> <strong>class</strong> Fragment {

// Pedagogical: (1) Attributes (2) Constructors (3) Methods,

// alphabetically ordered within each.




<strong>protected</strong> String text = “text not determined yet”;




<strong>public</strong> Fragment() {

}




<strong>public</strong> Fragment(String someText) {

text = someText;

}




// Pedagogical: (expressive) names alone are often sufficient for abstract methods.

<strong>public</strong> <strong>abstract</strong> <strong>void</strong> display();

<strong>public</strong> <strong>abstract</strong> String getText(); // Pedagogical: “get..()” and “set…()” standard

<strong>public</strong> <strong>abstract</strong> String getType();

<strong>public</strong> <strong>abstract</strong> <strong>void</strong> setText(String someText);

}




<h3> 1.6.3 Code showing polymorphism</h3>

Show the relevant code (only) and explain why <em>polymorphism</em> is appropriate here. Recall that polymorphism is implemented in one of two ways – overriding methods in subclasses or overloading methods in the same class where the method signatures are different – and allowing the language runtime to dynamically invoke the correct method. It should be clear where the code is located (class and method).

Your response should replace this, as well as the example below.




The method <em>displayTypeCount</em>() iterates through Fragment’s and calls <em>getType</em>() on each. This is polymorphism. The relevant code is shown below.

<strong>static</strong> <strong>void</strong> displayTypeCount() {

// Postcondition: The counts of heading- and non-heading type fragments in

// theFragments are on the console




<strong>int</strong> headingCount = 0, nonHeadingCount = 0;

<strong>for</strong> (Fragment fragment : <em>theFragments</em>) {

<strong>if</strong> (fragment.getType() == “Heading fragment”) {

headingCount += 1;

}

<strong>else</strong> {

nonHeadingCount += 1;

}

}

…

}

<h3>1.6.4 Code showing upcasting or downcasting</h3>

Show the relevant code (only) and explain why upcasting or downcasting is appropriate here. It should be clear where the code is located (class and method).

Your response should replace this, as well as the example below




Some of the sub-fragments of a <em>HeadingFragment</em> are themselves <em>HeadingFragment</em>s. We need to cycle through all sub-fragments but identify <em>HeadingFragment</em>s so we can call <em>displayAll</em>(). Downcasting is needed from <em>Fragment</em> to <em>HeadingFragment</em>.

<strong>public</strong> <strong>class</strong> HeadingFragment <strong>extends</strong> Fragment {




<strong>private</strong> ArrayList&lt;Fragment&gt; theSubFragments = <strong>new</strong> ArrayList&lt;Fragment&gt;();




<strong>….</strong>




<strong>public</strong> <strong>void</strong> display() {

System.<strong><em>out</em></strong>.println(text);

}




<strong>public</strong> <strong>void</strong> displayAll() {




display();  // the heading itself




// display sub-headings and their sub-headings

<strong>for</strong>(Fragment fragment: theSubFragments) {

<strong>if</strong> (fragment <strong>instanceof</strong> HeadingFragment) {

((HeadingFragment)fragment).displayAll();

}

<strong>else</strong> {

fragment.display();

}

}

}










<h2>1.7 YOUR CODE</h2>

Unless your facilitator requests another method, copy your Eclipse project to your file system, zip it, and attach it. Please contact your facilitator in advance if you want to request an alternative means.

&lt;Your response here&gt;




<h2>1.8 EVALUATION OF ASSIGNMENT 1</h2>







<h2>Appendix 1 (if needed; should be referenced above, and will be read as-needed only)</h2>




<h2>Appendix 2 (if needed; should be referenced above, and will be read as-needed only)</h2>