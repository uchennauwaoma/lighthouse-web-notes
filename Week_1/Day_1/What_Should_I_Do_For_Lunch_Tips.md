###Tips

```javascript
function whatToDoForLunch(hungry, availableTime) {
  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
}
```
```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  if (!hungry) {
    console.log("Wait until you're hungry.");
  } else if (availableTime < 20) {
    console.log("Pick up a snack or grab something you have ready at home.");
  } else if (availableTime <= 30) {
    console.log("Take time to cook a tasty meal. You deserve a break!");
  } else {
    console.log("This is an intense program, reconsider spending more than 30 minutes on lunch.");
  }
};
/*
 * This is some test runner code that's simply calling our whatToDoForLunch function
 * defined above to verify we're making the right decisions. Do not modify it!
 */

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
whatToDoForLunch(true, 15);
```
