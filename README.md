questions
=========

- [TypeError: Object #<HTMLDivElement> has no method 'addClass'](http://stackoverflow.com/questions/6409039/jquery-each-this)
   - Code: $('div')[0].addClass('hi')
   - $('div') returns a Jquery object. The jquery object has a list of html elements. [0] selects an html element.  You cannot add a class to this html element because addClass is a jquery object method and $('div')[0] is no longer a jquery object.  To turn $('div')[0] back into a jquery object, wrap it in $().  So it looks like this: $($('div')[0]).  You can now do $($('div')[0]).addclass('hi').  
   - This is horribly unreadable. I recommend setting $('div')[0] to mydiv and doing $(mydiv).addClass('hi')   
