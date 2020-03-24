# 100 Days Of Code - Log

### Day 1: March 10, 2020 (HTML + JS)

**Today's Progress**: Worked on the Deli Lab on Learn.co, had to build a function currentLine that accepts the current line of people and returns the current line as a string. Also started working on a new website, just did the beginning and inputted a picture and a form with two input fields.

**Thoughts:** It is really difficult for me to understand the blank canvas, when i see the finished solution it is easy for me to explain what was used and why, but actually coming up with the solution is a real struggle for me still.

**Code Snippet:** 

//1) I declared the function and passed two parameters into it. 2) Declared let key word containing the lines length + 1, meaning that when the line has + 1 added to it is starts the funtion. 3) i then pass the current.length as an object and equals it to a newName everytime a new number is taken 4) I then declared the Welcome message with let temp and passed the new parameters of newName and num into the welcome message. 5) I used return to display the welcome message.

function takeANumber(current, newName) {
  let num = current.length + 1;
  current[current.length]=newName;
  let temp = "Welcome, " + newName + ". You are number " + num + " in line.";
  return temp;
}

//1) I declared the function and passed one parameter into it. 2) I delcared let temp as an empty string. 3) I used if as when the line is empty or undefined it would return the message. 4) I used else to accept the current line of people 5) then shift to remove the person who is currently being served.6) used return to show the string + the name of the person currently being served.

function nowServing(katzsDeliLine) {
  let temp = "";
  if(katzsDeliLine[0] === undefined){
    return "There is nobody waiting to be served!";
    }
  else{
    temp = katzsDeliLine[0];
    katzsDeliLine.shift();
    return "Currently serving " + temp + ".";
  }
}

function currentLine(current) {
  let list= "The line is currently: ";
  if(current[0]===undefined){
    return "The line is currently empty."
  }
  else {
    for(let i=0;i<current.length;i++){
      let num = i+1;
      if(i===0){
        list = list + num +". " + current[i];
      }
      else{
        list = list + ", " + num + ". " + current[i];
      }
  }
  return list;
}
}

### Day 2: March 11, 2020 (HTML + CSS)

**Today's Progress**: 
Continuing to work on my login page today using HTML and CSS with a lot of help from 
@wwwschools. Added my first mediaquery, which was really cool when it finally worked.

**Thoughts:** 
Learned today that my CSS text is twice as long as my HTML everytime .. Thinking faceEnjoyed playing around with different styles and adding img, links and onclick to the pages.Rocket

**Code Snippet:** 
<!DOCTYPE html>
<html>
    <head>
        <title>Sign Up Page</title>
        <link rel="stylesheet" type="text/css" href="regstyle.css">
    </head>
    
    <body>
        <div id="login-box">
            <div class="center">
                <h1>Sign Up</h1>
                
                <input type="text" name="username" placeholder="Username" />
                <input type="text" name="email" placeholder="E-mail" />
                <input type="password" name="password" placeholder="Password" />
                <input type="password" name="password2" placeholder="Retype Password">
                
                <input type="submit" name="signup_submit" value="Sign me up" />
                <h4><a href='#'>Return to Login Screen</a></h4>
            </div>
        </div>     
    </body>
</html>

### Day 3: March 12, 2020 (Little bit of HTML + Lots of CSS Challenges)

**Today's Progress**: 
Working on setting up the homepage for my site today, going to work on the header and footer in HTML first and then style it with an external CSS sheet.

**Thoughts:** 
Today I had a full on silent(mostly silent !%#@£!) war with CSS. Was trying to create a central search button(worked) and then a simple header with a few menu button which was top right central.(50% working)

**Code Snippet (CSS):** 
body {
    margin: 0;
    padding:0;
    background-image: url(http://wannagosurfing.com/wp-content/uploads/2015/11/awesome-surf-surfing-widescreen-high-definition-wallpaper-for-desktop-background-images.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center center;
    background-attachment: fixed;
}

@media only screen and (max-width:767px) {
    body{
        background-image: url(https://mcdn.wallpapersafari.com/medium/66/85/qbZQFL.jpg);
    }
 }


#homeBanner {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, 50%);
    width: 25rem;
    
}

form {
    position: flex;
    align-items: center;
    justify-content: center;
}

input {
    text-align: center;
    box-sizing: border-box;
    margin-bottom: 20px;
    padding: 4px;
    width: 400px;
    height: 40px;
    border: none;
    border-bottom: 1px solid #AAA;
    font-family: sans-serif;
    font-weight: 400;
    font-size: 15px;
    transition: 0.2s ease;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.4);
}

.pageHeader {
    background: #659DBD;
    display: block;
    height: 120px;
    min-width: 120px;
    color: #fff;
    text-shadow: #000 0 0 .2em;
}

.headerButton {
    margin: 1%;
    text-align: center;
    box-sizing: border-box;
    margin-bottom: 20px;
    padding: 2px;
    width: 90px;
    height: 20px;
    border: none;
    font-family: sans-serif;
    font-weight: 400;
    font-size: 12px;
    transition: 0.2s ease;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.8);
    background-color: #659DBD;
    color: white
        
}

.menuButton {
    text-align: right;
    height: 120px;
    min-width: 120px;
    position: block;    
}

### Day 4: March 13, 2020 (Little bit of HTML + Lots of CSS Challenges)

**Today's Progress**: 
Today I "finished" the header on my homepage, spent most of the time reviewing my CSS and re classing my DIV elements, but it finally worked with just a simple (padding-top). Hooray!

**Thoughts:** 
That Git is much harder than first anticipated, struggling getting my Brackets files synced with git.

### Day 5: March 14, 2020 (HTML Course on Freecodecamp)

**Today's Progress**: 
Finished the Basic HTML and HTML 5 part of the @freeCodeCamp, enjoyed doing a course that is centered around the ide. Got a slight understanding of how data is passed on as well.

**Thoughts:** 
Starting to have a more structured understanding of HTML and how to apply the structures.

### Day 6: March 15, 2020 (CSS course on Freecodecamp)

**Today's Progress**: 
I Did 2 x 30 minutes today on @freeCodeCamp working on the CSS modules around padding and margin, which makes a lot more sense now.

**Thoughts:** 
Getting better at understanding CSS and where to use it.

### Day 7: March 17, 2020 (CSS Course + HTML and CSS writing)

**Today's Progress**: 
I had a very productive day, completing the CSS basic module and applying it to my homepage with a nice video and better styled search bar!

**Thoughts:** 
I make things overcomplicated and when I try and troubleshoot items I should try and break it down from the beginning.

### Day 8: March 18, 2020 (CSS Applied Visual Course + HTML and CSS clean up)

**Today's Progress**: 
I have been working through the applied visual course with @freecodecamp. I worked on my homepage file and removed the header and relating css from it as I think it needs to be simplified and I want to use a navbar tag instead.

**Thoughts:** 
i deleted 20% of my CSS without it actually changing much of the layout so i should try and write simpler code.

### Day 9-10: March 19-20, 2020 (HTML + CSS + JS)

**Today's Progress**: 
I worked on a dynamic header for the website and I started the creation of the search results page where I worked with rows and columns. Also looked into setting up a server less database with Azure. 

**Thoughts:** 
It was difficult working with JS and making the loop work, I still dont fully grasp how and why the loop works and when to use it but W3 school examples were good and I used them to make a dynamic header with buttons

### Day 11-12: March 21-22, 2020 (MYSQL, CRUD, CSS)

**Today's Progress**: 
 have started the SQL tutorial on 
@freeCodeCamp
 so that I can setup a database for the website which should hopefully help me with the search engine I am trying to create!

**Thoughts:** 
C.R.U.D (Create, Read, Update, Delete).
Difficult to find time with the kids and Abbie all in the house. But I am constantly thinking off how I can connect the searchbar with a database that can provide the results I need. I also found a place that has similar data to what I need(https://surfing-waves.com), so if I could get a crawler on that it would be perfect!!

### Day 13: March 23, 2020 (CSS)

**Today's Progress**: 
Worked on the Applied Visual Design course today. I did not get to do much on the SQL side, but will dedicate at least 1 hour for tomorrow morning.

**Thoughts:** 
Difficult day where I did not get much done due to laziness and having fun with the kids :)

### Day 14: March 24, 2020 (CSS)

**Today's Progress**: 
Got an hour and some done from the Database Management Basics and SQL course, learned to install mySQL and access it through the terminal plus how to change my password and setup a database in the terminal!

**Thoughts:** 
Felt good to create my first database on the command line! I am definitely going to use the popSQL editor as I like when it is visual. So will install it tomorrow and get started.

