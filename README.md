questions
=========

- [TypeError: Object #<HTMLDivElement> has no method 'addClass'](http://stackoverflow.com/questions/6409039/jquery-each-this)
   - Erroring Code: <code>$('div')[0].addClass('hi') </code>
   - <code> $('div') </code> returns a Jquery object. The jquery object has a list of html elements. <code> [0] </code> selects an html element.  You cannot add a class to this html element because addClass is a jquery object method and <code> $('div')[0] </code> is no longer a jquery object.  To turn <code> $('div')[0] </code> back into a jquery object, wrap it in <code> $() </code>.  So it looks like this: <code> $($('div')[0]) </code>.  You can now do <code> $($('div')[0]).addclass('hi') </code>.  
   - This is horribly unreadable. I recommend setting $('div')[0] to mydiv and doing $(mydiv).addClass('hi')  

 - [What are you doing when you stick an html object in $()?]()
  - You are giving a html object superpowers.  R2d2 is an html element.  He is much more powerful when inside an x-wing.  wrapping an html object in jquery is sticking R2D@ in an xwing.



- [Show only the first line of a git commit in the log]()
   - <code> git log --pretty=oneline </code>
   - Method for finding out: <code> git log --help </code>  
      - This is the log manual. It is an intimidating wall of text. To find stuff, when in the log, press <code> /oneline </code> to find all of the times  'oneline' appears.  
      - I prefer <code git log --help | grep online </code>  This is a minature google:  <code> | grep oneline </code> finds all of the lines containing the word online.

- [Find information on Jquery](http://jquery.com/) 
  - Where is the best place for beginner-level documentation?  Jess: Codecademy
  - The best place for jquery documentation for advanced people are the docs. 
  - This is intimidating and I need more practice reading it. 
  - jquery verbs...say what you are trying to do in English, and you'll probably find a method of the same name.  
 
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
 
- [How do you go about googling]()
  - Get as specific as you can with your thorough debugging process. 

- [No Method Error on Nil class](http://www.ruby-doc.org/core-2.1.0/NoMethodError.html)
  -really general errors are hard to debug.  

- [How to search with grep in a directory?](Ksolo)
    <code> grep -r READ -i ./ </code>

- [How to set up git so that commit messages say they are from me](http://git-scm.com/book/en/Getting-Started-First-Time-Git-Setup)
   -Thank you for the link, Jss 
      $ git config --global user.name "John Doe"
      $ git config --global user.email johndoe@example.com

- [What are sessions in Sinatra?]()
  -Analogy: A session is like a secret handshake. One person is the server. The other person is the client.  Both have to know the secret hanshake. 
  - History:  Once upon a time there were only links.  Through the links the internet was born. Then fatcats were like, how can we make money?  People like personalized service, so they said, let's make web more personal. If people thought the web knew them personally, they would spend more money.  The cookie was born.  The cookie is actually a session. The cookie stores information about your visit.  People were creeped out by the cookie because they found out that something was following them around and tracking them.  What if we renamed cookies to sessions?  
   - Where does the client person store information about how to store secret information?  
   - you can look in headers to find the cookie.  The cookie is where the client keeps his half of the secret handshake. 
   - you can use pry to see the client sending the cookie to the server.  In other words, the person is comming towards me with a grin and her part of the secret handshake, I have to know how to respond to that handshake, or I can't be a part of her club and can't watch what she does.  
   - Now, the cookie doesn't mean anything if the server doesn't know the secret handshake.  You enable sessions in the config.ru
   - Once the secret handshake happens, the server takes that as permission to follow the client around and watch their every move. This can be creepy or flattering, depending on the motives and if the client knows he/she is being watched. 

  

- [How does Zach the TA like to teach?]()
   - likes people to raise hands for questions. Don't shout-out. 
   - likes to randomly call on people 

- [no acceptor (port is in use or requires root privileges)](https://github.com/tararoys/SurveyDBC/blob/TLR/Tests/README.md#no-acceptor-port-is-in-use-or-requires-root-privileges)
     
         px ax | grep ruby #this command will find two processe

      -The output should look like this: there should be two things in the list 
  
         27235   ??  S      0:00.72 /Users/tlroys/.rvm/gems/ruby-1.9.3-p484/bin/shotgun      
         27393 s000  S+     0:00.00 grep ruby
   
     - The first one is the actual 'zombie server' you are looking for. The second thing is funny, because you are looking for all processes that contains the word ruby, and so it find the process that is looking for all processes that contain the word ruby. Haha. 
     
      - Kill the first process. with the following command: 
      
           kill -9 27235
          
         The number in this kill function is the process number. 
   
         
