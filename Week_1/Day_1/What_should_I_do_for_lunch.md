### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.


```const whatToDoForLunch = function(hungry, availableTime) {
  if (hungry === true) {
    if (availableTime <= 20) {
      console.log("Pick something up and eat it in the lab.");
    } else if (availableTime > 20 && availableTime <= 30) {
      console.log("Try a place nearby.");
    } else if (availableTime > 30) {
      console.log("We're in a bootcamp and we should consider how much time we have.");
    }
  } else if (hungry === false) {
    console.log("Not hungry, continue working.");
  } else {
    console.log("I don't know what to do!");
  }
};


console.log("I'm hungry and I have 20 minutes for lunch.");
whatToDoForLunch(true, 20);
console.log("---");

console.log("I'm hungry and I have 50 minutes for lunch.");
whatToDoForLunch(true, 50);
console.log("---");

console.log("I'm not hungry and I have 30 minutes for lunch.");
whatToDoForLunch(false, 30);
console.log("---");

console.log("I'm hungry and I have 15 minutes for lunch.");
whatToDoForLunch(true, 15);```