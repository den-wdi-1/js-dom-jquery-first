# The DOM (Document Object Model)

# Learning Objectives

- Explain what the DOM is and how it is structured
- Select and target DOM elements using DOM methods
- Select and target DOM elements using a query selector
- Create, read, update, and delete DOM elements
- Change the attributes or content of a DOM element

# Framing (5 min)

The [**D**ocument **O**bject **M**odel](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction) is a programming interface for HTML.

An HTML *document* is available for us to manipulate as an object, and this object is structured like a tree:

![DOM diagram](dom-tree.png)

Or this:

```text
html
└── head
│   ├──title
│   ├──meta
│   ├──link[rel="stylesheet"]
|   └──script[type="text/javascript"]
|
└── body
    ├── header
    │   ├── h1
    │   └── nav
    └── section.simplicity
    |   └── h2
    │   └── article
    ├── section.life
    |   └── h2
    │   └── article
    │       └── block_quote
    │       └── block_quote
    └── footer
```

# Traversing the DOM

## You Do: Explore the DOM

1. Go to the deployed version of the [Tic Tac Toe](http://ga-wdi-exercises.github.io/tic_tac_toe/) exercise.
2. Open the Chrome console (Command + Option + J)
3. Use jQuery to select the square with the class of "board"
4. Save the board to a variable
5. `console.dir` the variable
6. Use your mouse to expand the `0` property of the variable. This is the DOM object representation of the game board's element

> To access the element with "vanilla" JS, you would use `document.querySelector(".board")`

### Answer:

- How many properties can you find on the board's DOM object that refer to other elements? (I count at least 13)
- What's the difference between a "Node" and an "Element"?

### Bonus

- `console.dir(document)`
- `console.dir(window)`. Try not to gasp.

## You Do: JS DOM Quotes, Part 1: Selector review

**Checkout the `jquery` branch.**

[Link](https://github.com/ga-wdi-exercises/js-dom-quotes/tree/jquery#part-1)

## You Do: JS DOM Quotes, Part 2: DOM Traversal

**Checkout the `jquery` branch.**

[Link](https://github.com/ga-wdi-exercises/js-dom-quotes/tree/jquery#part-2)

# Manipulating the DOM

## You do: Hijack a webpage

Here's an artist's interpretation of true beauty:

<img id="true_beauty" src="mona.jpg" alt="Mona" style="display:block;margin:0 auto;" />

It's rather inadequate. Go to [Nicholas Cage's Wikipedia page](https://en.wikipedia.org/wiki/Nicolas_Cage) and copy the URL of your favorite image on the page. Then, use your browser's console and jQuery to replace the image above with the image of Nic Cage.

## You do: Cheat with Javascript

Go to [CookieClicker](http://orteil.dashnet.org/cookieclicker/). Click the cookie a few times.

Ain't nobody got time for this.

1. Save the cookie element to a variable.
2. Use Javascript to [simulate a click](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/click) on the cookie.
3. Use a timing function to make Javascript click the cookie once every millisecond.
4. Now bookmark CookieClicker to save it for later, close the page, and pay attention in class.

## Building Math Minute

[Watch this series of videos on making Math Minute](https://www.youtube.com/playlist?list=PLae1he6d1WIkQW5WyBlbmx8pnkM5DYuTY)

[Play with it here](http://ga-wdi-exercises.github.io/math-minute/)

[Here's the Repo](https://github.com/ga-wdi-exercises/math-minute)

# References

<script src="jquery.min.js"></script>
