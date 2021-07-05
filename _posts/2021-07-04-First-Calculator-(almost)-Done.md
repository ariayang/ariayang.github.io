After 3 days of work, I am (almost) done with my first Calculator website. This is one of the intermediate challenges from <em>Front End Mentor</em> website. Having experienced struggles last time with the Simon game project, I learned my lesson to break down the tasks into smaller parts. Much much smaller chunks.

<h2> The result </h2>
<a href = "https://ariayang.github.io/calculator-app-main/" target = "_black">My Calculator App </a>

<h2> The process </h2>
I started with the <strong>drawing</strong> of the page, dividing it into header (app name, toggle bar(2x2 grid for toggle bar and lables arrangement), result display, keypads (another grid), and footer divisions.

Then, <strong>HTML</strong> to layout the divisions and test it on the browser, including the responsive design. The toggle bar did not look aligned or even like a toggle bar yet. Since I would not work on the themes for a while, let's leave it there for now and change it later.

Next, <strong>css style</strong>. The specification asks for three theme colors. I started with one color to make sure it works as desired first. This almost took half a day. I decided not to worry about the other two themes at this point since I want to make sure I can implement the functions first.
  
<strong>The fun part: Javascript.</strong> <br>
I started with making sure the webpage can <strong><em>listen to the buttons, and recognize the button id/class</em></strong>. Test it in the browser Javascript console. Works.

Then, to make sure the screen can <strong><em>display the button</em></strong> I clicked. The numbers button worked. I left out the 'del' or 'reset' buttons at this point.

Next, to <em>form values from the buttons</em>. Up to this part, another half day of work.

The <strong>operators</strong> took me a while to figure out the sequence. I realized I can only add the values into the equation when I clicked an operator. A lot of tests in the browser console to test I got the sequence right, and consequtive clicks on operators did not get pushed into the equation over and over.

It also took me a while and discussion to dicide on using one array to store input values, and operators together.

After the operator part works, I moved on to the <strong><em>"=" button</em></strong>. At this moment, I do not want to worry about the order operation yet. Just making sure clicking "=" gives me the result right. And after showing the result, I can keep adding operators, or numbers to continue the calculation from the result or start fresh. This is almost another day's work.

Finally, the <strong><em>operation order</em></strong>. I tried many times on the iPhone calculator to see how it works, and at which point the disply changes values. It took me hours to figure out the flow chart. My partner gave me the hint that I can do the " * " times or " / " divide operation as soon as it happened. It definitely helped. Took me some time to debug the implementation. Used a lot of "console.log" to monitor the values and operators stored in the array.

I also made 'Reset' work since "=" operation also involves reset of the input.

At this point, <em>2 days of work</em> and it looks like an calculator. 

<strong> Day 3 </strong><br>
<ul>
  <li>Added the function that the calculator responds to keyboard too.</li>
<li>Found the right toggle bar design, and added it to HTML. Finally, it looked similar to the design spec.</li>
<li>Made the 'Del' operation work. Decided to added the 3 theme colors in Javascript. Debugging mainly involves identifying the right element for the JQuery operation.</li>
</ul>
<h3> The takeaway </h3>
Up to this point, I am pretty pround of myself on what I have achieved so far. 

It took a longer time than I expected. But I had a better understanding of module coding. Breaking bigger tasks into smaller parts are easier to debug, and satisfying along the way.

Always, always, think before code. Draw the flow chart. Understand how it should work. Use a lot of 'console.log' or debugger to see how the program works step by step. It is much easier to see where it got derailed from expectation. Typo, element class selected wrong, attribute typed wrong, or the flow chart error can all cause bugs.

At some point during the process, I started to make the program complicated, like condition within condition. When it happened, I realized there must be some logic wrong. The best to do is to step back, or pull myself away from the computer. Take a walk, or water the plant. Just do something else. When coming back, re-think the logic. Try something else. This way, most likely the problem will be solved faster than starting at the screen.

<h4> Still some todo </h4>
The display sometimes overflows, even though I set to hide the overflow.
The display to add ',' every 3 digits before decimal.
The way computer handles the double precision float number sometimes add something like 0.00000000001 to the end of the number. Needs to fix that in the result display.

<h5>Reference:</h5>
https://www.frontendmentor.io/challenges/calculator-app-9lteq5N29
