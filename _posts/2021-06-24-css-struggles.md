## Lessons learned in CSS

  My biggest struggle today so far is with the style of the links. At first, my unordered links ''< ul >< li >'' on the navbar won't align in line. I have tried  
```
display: flex-inline;
```
  Nope, doesn't work. This only places the whole flex box (maybe that ''<div>, <section>'') "in-line" with the other objects. 
  
  Only After multiple tries, I found I need to define my <ul> (which contains <li>) class style:
  ```
    list-style-type: none;
  ```
  And then I can make this particle class of ''<ul>'' a "flexbox" to arrange my <li> elements. My mistakes earlier happened in placing this line not in the right place.
  
  Next challenge, remove the default "blue underline" style in my links. What I struggled the most is where to put the line:
  ```
  text-decoration: none;
  ```
  What I found eventually works is to assign it to the base style anchor style <a>. 
  It can also placed in other class or id that is directly defined for ''<a>'' element. 
  Putting it under ''<li>'' won't work.
  
  My next frustration happens when I try to change the 'hover' properties for the links.
  It turns out there are two ways. 
  ```
  li:hover a"
  ```
  or,
  ```
  a:hover
  ```
  ''<li>'' and ''<a>'' can be replaced by its defined class/id names.
  Takeaway: Be careful about the 'space'. There is no space around ":". That in particular messed up my 'hover' function for a while. 
    
  Takeaway for the day:
    - Always define a base style first for links, position, font, color and margin, etc.: ''<a>, <body>''. 
    - Really pay attention about where to define the styles. 
    For example, if ''<a>'' is not defined in specific, or 'text-docoration' is not set to 'none', it will not inherite the style of the block it belongs to.
    
  
  
