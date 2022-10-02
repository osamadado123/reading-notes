# Thinkin in react
 ## **1- What is the single responsibility principle and how does it apply to components?**
this principle means that every component should have one function to do, if the component has more than one function then make subcomponents as children to it, every child will do one function. <br>
## **2-What does it mean to build a ‘static’ version of your application?**
that is means you will not be able to change your data. in another meaning; you will not use state into your components. <br>
## **3- Once you have a static application, what do you need to add?**
you have to make it dynamic, by using states into each component that needs to change its data. <br>
## **4- What are the three questions you can ask to determine if something is state?**
<ol>
<li>if is it able to move from its component(parent to child)? if not, maybe it is not state.</li>

<li>if its value still fixed over time? if yes, it is not state.</li>

<li>if it depends on other states and props? if yes, it is not state.</li>
</ol>

## **5- How can you identify where state needs to live?**
based on where it will be used and rendered? sometimes you have to pass this state from its component to another to render it there.

# Higher-order fucntions

## **1- What is a “higher-order function”?**
Higher-order functions allow us to abstract over actions, not just values. They come in several forms. For example, we can have functions that create new functions.

## **2- Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?**
It is equivalent of calling greaterThan(10)(11):

## 3- **Explain how either map or reduce operates, with regards to higher-order functions.**
Map operates on a list of values in order to produce a new list of values, by applying the same computation to each value on the other hand Reduce operates its builds a value by repeatedly taking a single element from the array and combining it with the current value.
