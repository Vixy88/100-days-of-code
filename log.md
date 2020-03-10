# 100 Days Of Code - Log

### Day 0: March 10, 2020 (Example 1)

**Today's Progress**: Worked on the Deli Lab on Learn.co, had to build a function currentLine that accepts the current line of people and returns the current line as a string

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
