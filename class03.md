# React Docs - lists and keys

**what does .map() return?** <br>
return a new array that has the same length of previous array <br> <br>
**If I want to loop through an array and display each value in JSX, how do I do that in React?** <br>
use map().
Each list item needs a unique  Key. <br> <br>
**What is the purpose of a key?** <br>
help React identify which items have changed, are added, or are removed. <br><br>

## The Spread Operator

**What is the spread operator?** <br>
the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments. <br><br>
**List 4 things that the spread operator can do.**
<ol>
<li>
 spreads the array into separate arguments
</li>
<li>
Copying an array ,Concatenating or combining arrays
</li>
<li>
Using Math functions
</li>
<li>
Using an array as arguments
</li>
</ol> <br> <br>

**Give an example of using the spread operator to combine two arrays.**
const firstName = [ "o","s","a","m","a"]
const lastName = ["m","a","h","e","r"]
const fullName = [...firstName,...lastName] <br><br>

**Give an example of using the spread operator to add a new item to an array.** <br>

const fruits = ['🍏','🍊','🍌']
const juicyFruits = ['🍉', '🍍','🍑' ...fruits]
console.log(juicyFruits) <br><br>
**Give an example of using the spread operator to combine two objects into one.** <br>
const helloObj = {hello: "🙂"}
const worldObj = {world: "😇"}
const fullSen = {...helloObj, ...worldObj, love: "🥰"}
