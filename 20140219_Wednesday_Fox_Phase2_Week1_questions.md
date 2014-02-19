#Questions



- [What is an ActiveRecord BeforeSave callback?](http://api.rubyonrails.org/classes/ActiveRecord/Callbacks.html)
  Jess: it is something that happens before a record is saved into the database. 

- [How do you generate a unique yet still short random string?](http://stackoverflow.com/questions/88311/how-best-to-generate-a-random-string-in-ruby)
  Jess: (this is stuff)[http://stackoverflow.com/questions/88311/how-best-to-generate-a-random-string-in-ruby]Create an array of 0 to nine, a to z, sample six characters, then have our database check to see if it is unique. 

- [What is a concrete analogy for sessions and cookies?]
    Kevin: Parking Validation.  

- [How are cookies useful?]()
   user authentication.

- [Important points: Keven: NEVER EVER EVER EVER SAVE PASSWORDS AS PLAIN TEXT IN THE DATABASE]()
   - Find a library that you want to use. Scramble the password.  Remove password from logfiles. DO NOT STORE PASSWORDS IN PLAINTEXT. 

- [typing each parameter individually into the Activerecord create is long and boring.]()
   - stick all of the attributes you need into a params hash subhash and just pass in the subhash. 
   - The google keywords are: ActiveRecord Mass Commits
   
- [Is there such a think as committing too much?](https://github.com/tararoys/url_shortener/commits/master)
      - Review of our commit history. 
      - When committing in your own branch, you cannot quit too much. 
      - When doing a pull request, you do a squash.  This allows you to clean up the commit history to make it look clearner.  It may be good practice to clean up the commmits.
      - Whatever your team decides to do is more important that a personal preference.  
      - Good, meaningful comit message. 
      -  One line, one blank line, full detailed message.   Top-line is subject line of e-mail, body is body of email. 
      -  How core do you think git is?  It is a very useful tool. 
      -  Pull request method is the best method.  Make sure you give current methods a fair shot.  
      -  Frame workflow issues  as 'let's do this better!' as opposed to 'You're doing it wrong."

- [How do you tackle the whole app process?]()
  
    - Wireframe
   - Migrations
   - Models
  
  Kevin: 
  - Wireframings are a great place to start.  
  - Start with a content overview.  
  - Then wireframe.  
   
  - You don't design the packaging until you know what is going in the box.  
  - Delays the step by asking what is going on the page, like what Jess did. 
  - Take some time to design.  But don't sit there and design too much. Get enough going so you

- [Why are sessions called cookies?]()
  - Sessions are on the client side.  
  - Cookies are on the browser.  The term cookie comes from the term magic cookie.  Where does magic cookie come from?  Probably from someplace like the ACM.  Wit! Fix it! 
  - Google cannot access DevBootcamp cookie information. But the user has the cookie, so the user can use his powers for evil. 
  


      
