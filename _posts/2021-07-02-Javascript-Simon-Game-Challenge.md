<h2><em> Objective: </em></h2>
  Simon game. The computer flashed one random button a time. User needs to remember the flash sequence from the first one as level goes up. As soon as the user pushed the wrong button, the game annouces user lose.

<h2><em> Problem statement: </em></h2>
  <ul>
  <li>
  I first waited for all the buttons clicked (userClicked.Length === gamePattern.Length) before comparing the arrays. It is easier to facilitate but not what the game wanted.
  </li>
  <li>
    Then I started to struggle with the <em> sequence of the events</em> . I tried to put all the comparison activities inside the $button.click() event. But if the game fails, it will restart automatically without trigger. 
    I thought the comparison got triggered at the wrong time, so I started to add more and more "if" before the trigger, such as (game.started, userClicked.length > 0 and < gamePattern.length, etc.) until it get so complicated that I gave up.
  </li>
</ul>

<h2><em> Solution: </em></h2>
  The checkAnswer(currentIndex) function needs to be created. The comparison of current click (userClicked[currentIndex]) with the gamePattern[currentIndex] will be happened outside the button.click event. So, once a button is clicked, the function will check the current input. 
  The function will also check if the user finished the clicks, and proceed to the next sequence if necessary.
  Since the user needs to input the whole sequence every time, the reset of the userClicked array needs to be put inside the nextSequence() function, instead of checkAnswer function, or button.click event. 
  
<h2><em> Takeaway: </em></h2>
  Even though I am following the instructions step by step, because I did not think the sequence through or fully understand the problem before diving into the coding (usual mistake for me!), I spent so much time sorting the algorithm during debug. There are a lot of back and forth trying to sort the events sequence right. Especially with the button.click event, I need to practice more to understand better what's needed to be included in the event, and what activities need to be separated. 
