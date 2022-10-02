# React State and Props

the differences between props and state and how to use both

## React Lifecycle

<ol>
<li>
Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? <br> <br> <b>
Render </b></li>

<li>
What is the very first thing to happen in the lifecycle of React?<br> <br> <b>
the constructor
</b>
</li>

<li>
Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates <br> <br><b>
Constructor then Render then React Updates then  componentDidMount then componentWillUnmount</b>
</li>
<li>
What does componentDidMount do?
<br> <br> <b>
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions.</b>
</li>
</ol>

# React State vs Props

<ol>

<li>
What types of things can you pass in the props? <br> <br>
<b> Props is an object, you can pass any attribute or properties in any valid javascript data type</b>
</li>

<li>
What is the big difference between props and state? <br><br>
<b>
Props Get passed into a Component as argument Props are read-only. <br>
on the other hand state is used to manage data unlike props, components cannot pass data with state, but they can create and manage it internally.
</b>
</li>
<li>
When do we re-render our application? <br><br><b>
whenever there is a change in their state or props

</b>
</li>
<li>
What are some examples of things that we could store in state? <br><br><b>
data which may be a string , number or any complex object .</b>

</li>

</ol>
