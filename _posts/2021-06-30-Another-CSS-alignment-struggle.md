Just had another day struggling with Navbar alignement again.

<h2><em> The goal: </em></h2> 
  Using bootstrap (version 5.0.2) for Navbar design, with collapse behavior when viewport is smaller.

<h2><em> Where I got stuck: </em></h2>
  Trying to follow the video using version Bootstrap version 4, the 'ml-auto' which works for justifying-content to the end in the flex box is not working.
  
<h2><em> The process </em></h2>
  After multiple tries in the developer tool, checking every element (navbar, navbar-nav, navbar-toggler, navbar-collapse, navbar, navbar-expand-lg) setting on margin, justify-contents, flex, etc. Nothing worked. 
  Searched online for solutions and did not get meaningful answers.
  Finally, searched the Q&A session of the video (The Complete 2021 Web Development Bootcamp) and found the answer.
  
<h2><em> Solution: </em></h2>
  'ms-auto' in the 'ul' class. 
  
<h2><em> Why: </em></h2>
  ml-auto (margin-left, together with mr becomes obsolete in the updated version. 'left' and 'right' becomes 's for start' and 'e for end' for setting margin(m) and padding(p). 
  Setting margin-start to auto, finally making my links items to the right of the screen. 

