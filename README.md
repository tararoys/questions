questions
=========

- [TypeError: Object #<HTMLDivElement> has no method 'addClass'](http://stackoverflow.com/questions/6409039/jquery-each-this)
   - Code: $('div')[0].addClass('hi')
   - $('div') returns a Jquery object. The jquery object has a list of html elements. [0] selects an html element.  You cannot add a class to this html element because addClass is a jquery object method and $('div')[0] is no longer a jquery object.  To turn $('div')[0] back into a jquery object, wrap it in $().  So it looks like this: $($('div')[0]).  You can now do $($('div')[0]).addclass('hi').  
   - This is horribly unreadable. I recommend setting $('div')[0] to mydiv and doing $(mydiv).addClass('hi')  

[Show only the first line of a git commit in the log]()
   - <code> git log --pretty=oneline </code>
   - Method for finding out: <code> git log --help </code>  
      - This is the log manual. It is an intimidating wall of text. To find stuff, when in the log, press <code> /oneline </code> to find all of the times  'oneline' appears.  
      - I prefer <code git log --help | grep online </code>  This is a minature google:  <code> | grep oneline </code> finds all of the lines containing the word online.
