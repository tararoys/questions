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
    stick all of the attributes you need into a params hash subhash and just pass in the subhash. 


   
-[Is there such a think as committing too much?](https://github.com/tararoys/url_shortener/commits/master)
      -Review of our commit history. 
   
