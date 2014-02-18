questions
=========

- [TypeError: Object #<HTMLDivElement> has no method 'addClass'](http://stackoverflow.com/questions/6409039/jquery-each-this)
   - Erroring Code: <code>$('div')[0].addClass('hi') </code>
   - <code> $('div') </code> returns a Jquery object. The jquery object has a list of html elements. <code> [0] </code> selects an html element.  You cannot add a class to this html element because addClass is a jquery object method and <code> $('div')[0] </code> is no longer a jquery object.  To turn <code> $('div')[0] </code> back into a jquery object, wrap it in <code> $() </code>.  So it looks like this: <code> $($('div')[0]) </code>.  You can now do <code> $($('div')[0]).addclass('hi') </code>.  
   - This is horribly unreadable. I recommend setting $('div')[0] to mydiv and doing $(mydiv).addClass('hi')  
   - What exactly does wrapping an html element inside $() do?  What is the concept behind this magic formula? 

- [Show only the first line of a git commit in the log]()
   - <code> git log --pretty=oneline </code>
   - Method for finding out: <code> git log --help </code>  
      - This is the log manual. It is an intimidating wall of text. To find stuff, when in the log, press <code> /oneline </code> to find all of the times  'oneline' appears.  
      - I prefer <code git log --help | grep online </code>  This is a minature google:  <code> | grep oneline </code> finds all of the lines containing the word online.

- [Find information on Jquery](http://jquery.com/)
  - The best place for jquery documentation.
  - This is intimidating and I need more practice reading it. 
 
- [Find information on Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
   - This is the best place for javascript documentation (according to Alyssa) 

- [get an href inside list element]() 
  - translation: use jquery traversal methods children(), first()
  - [tree traversal](https://api.jquery.com/category/traversing/tree-traversal/)
  - analogy: A webpage is like a really annoying prank present given to you by friends with way too much time on their hands.  Why? Because they give you a giant box which is actually filled with more boxes, some of which are filled with more boxes.  For some reason, they decided to call this setup a tree, because to mathemeticains the process of opening boxes within boxes is sort of like watching a squirrel run up and down different branches of a tree.  So...in order to get to the href, I need to get to the the li box that it is in, open the li box, find the a box, open the a box, and find the href widget inside the box. Fortunatley I have a robot called Jquery to do this for me, and all I have to tell him is "get me the first li, get get it's first child, and tell me what is in the href!
 

- [how to launch google chrome on ubuntu](http://ubuntuforums.org/showthread.php?t=1385182)
  - <code>google-chrome www.girlgenius.com</code>
  - New question: how to launch google chrome with local webpage? 
 
- [how do I debug a sinatra skeleton?](https://github.com/tararoys/DBC_Sinatra_Skeleton)
   -zach: use the following gems.
   - In Gemfile: 
      
        gem 'pry'
        gem 'pry-nav'
       
      
   - In config/environment.rb
      
        require 'pry'
        require 'pry-nav'
      
   - In the place you wish do debug, 
    
        binding.pry #dumps you into a console at that exact point in your program.


- [how do you do error driven development (EDD) with sinatra routes?]()
   - Workflow
     - Set up a route that returns a view
     - check in the browser to see if that route returns that view
     - read the error.
     - Click on buttons
     - read the error
   - Is there a more efficient way of doing this?  Zach: This is called integration testing, and the framework to test this is called Selinuium. 

- [How do you quickly find the solutions to problems you know you've solved before?]()
   - Zach: [pocket stores things so that you can read it later](http://getpocket.com/) 

- [How do you go about googling]()
  - Zach: Get as specific as you can with your thorough debugging process.



