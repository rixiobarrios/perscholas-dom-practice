# Accessing DOM Elements (Querying)

Let's start with some simple query selecting.

**Part 1**

DOM's personal website title is a bit wordy. Write a JavaScript statement that selects the ```#main-title``` ID element. Remember there are a couple of ways to query id. Change the text of the title to something shorter.

**Part 2**

Select the bodyand change the ```background-color``` to a new color of your choice.

**Part 3**

Select DOM's Favorite Things list and remove the last list item.

**Part 4**

Select all ```.special-title``` class elements and change their ```font-size``` to ```2rem```. Remember you might have to iterate through the list of elements

**Part 5**

Turns out DOM never raced in Chicago. Access the Past Races list and remove Chicago.

## Creating New DOM Elements

**Part 6**

Let's add to DOM's Past Races list. Create a new ```<li>``` element, change the new ```<li>``` text to the name of a city, and append it to the Past Races list.

**Part 7**

Create a new ```.blog-post``` corresponding to the new city added in Part 6. You will have to create a new ```<div>``` with class of ```.blog-post```, a new ```<h2>``` with text, and a new ```<p>``` with some text. Think about what order you want to create the elements, and what order you want to append them in.

## Event Handlers

**Part 8**

When you reload the page, the ```script.js``` file loads a random DOM quote. Let's play with the included function:

```
    const randomQuote = function() {
  document.querySelector('#quote-of-the-day').innerText = `"${quotes[Math.floor(Math.random() * quotes.length)]}"`;
};
```

Query select the ```#quote-titleID``` element and add a click event handler. That event handler should use the function randomQuotewhenever ```#quote-titleis clicked```.

**Part 9**

Select all ```.blog-post``` class elements. Iterate through the list of ```.blog-postclass``` elements and apply two event handlers to each node. The first event handler should be listening for mouseoutevents while the second handler should be listening for mouseenterevents.

The mouseouthandler should toggle the class ```.purple```
The mouseenterhandler should toggle the class ```.red```
Test it out!

### Hint:

Remember the document node property ```.classList``` and the document node method ```.toggle()```.
