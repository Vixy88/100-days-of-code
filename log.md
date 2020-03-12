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
