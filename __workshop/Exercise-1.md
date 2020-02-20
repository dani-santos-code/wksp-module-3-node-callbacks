# Questions

**With a partner**, answer these questions as completely as possible. Feel free to look at past lecture notes, the web, anything.

Take the time to explain it to each other.

The power of this exercise is in the act of _formulating_ and _explaining_ the concepts to someone else (your teammate).

## One

Run the app. Write out the steps, the _pseudo code_, required to create this app. It doesn't have to be totally accurate, or in the right order.

Only move on to the next question when you have enough detail that you would be able to start coding it yourself.

```
// First, let's set up Express server and create an endpoint for the homepage. On a  get // request, show home page that includes the partials (header, footer)
// Create an endpoint for form submission handling (getItem). The handler
// will push the item to a global empty array and the handler should send the array.length -1.
// the homepage appends the item of the array to the div (with a list items)


```

## Two - `server.js`

Take a look at the `server.js` file.

We have a new module in there, `body-parser` that is required on line `4`. What is it for? What is its use-case? What other lines are related to this module?

_The NPM site might be a good place to start. Feel free to provide links as relevant._

```
// The body-parser allows to access all values in  a form via req.body and creates a JS object


```

## Three - `server.js`

Look at lines `23` and `24`. Explain the methods used. How are they different? What are the usecases for each?

```
// 23 - get is a user request for a page
// 24 - post is when a user manipulates the data somehow ( in this case, adding)

```

## Four - `server.js`

Line `6`. That's new. What do you think it's for?

```
// To make the code more DRY.

```

## Five - `handlers.js`

Explain line `1`. Where, why and how is `items` being used?

```
//  It's the empty array that will hold the items. It will be updated on each post request

```

## Six - `handlers.js`

Why is there `redirect` on line `11`;

```
// A response needs to be sent to the client, or else the client will waiting forever,
// so we can redirect to the same page or send a code, like 200

```

## Seven - `handlers.js`

The `handle404` function is a more complex than we've seen thus far, what is the extra functionality for?

```
// It is a middleware that provides 3 types of reponse, depending on what's passed via headers. So, it doesn't only accept html, but json or plain text

```

## Eight - `ejs`

Take a look at `homepage.ejs` and `todoInput.ejs`. What is happening in there? Explain line-by-line...

```
// It includes the header and the todoInput as well as the footer.
// content container that's iterating through the items array and adding an item to the list on each form submission. Each submission re-renders the page, because we're perfomring a get when redirecting the user to "/"

```

## Nine - `styles.scss`

What are lines `2` to `7` for this file? Where are these values being used? Take a look at `_homepage.scss` as well? What do you notice?

```
// They are global SASS variables that can be accessed/used in all scss files

```

## Ten - `_homepage.scss`

Line `16`. See if by searching the Sass documentation, you can determine what _exactly_ is going on here. That `#{}` notation very specific to this use-case. Why?

```
// It's used for Sass Interpolation

```







