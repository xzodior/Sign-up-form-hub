# Sign-up-form-hub

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)

## Overview

This project was created to display my current knowledge of form controls and validation from TOP (The Odin Project) and display what I've learnt. This was also the first time I used media queries this extensively to the point I start with structuring and designing for mobile before the desktop.

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page
- Receive an error message when the `form` is submitted if:
  - Any `input` field is empty. The message for this error should say *"[Field Name] cannot be empty"*
  - The email address is not formatted correctly (i.e. a correct email address should have this structure: `name@host.tld`). The message for this error should say *"Looks like this is not an email"*

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

I initially started with semantic html which is the first time i've done that albeit there's not much really semantics needed for this project. I have two main sections which needed to be separated so I focused on centering the two elements on the page but apply spacing betweeen them so they don't intertwine. As for the form controls, like I said in the overview, this was the first time using it and it really doesn't require me to do much apart from styling and applying required tags to each input element. 

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I learnt how to use Pseudo-classes more efficiently and also chain together multiple classes together to improve an invalid state without using JS. One problem with :invalid class is that when loading a page with it, it immediately tells the user hasn't inputted a valid element before they even had the chance to type. A work-around to this was to chain pseudo-classes together by using the :not class to prevent items from being selected.

An example of this: 

```css
#first-name:not(:focus):not(:placeholder-shown):invalid {
    border: 2px solid red;
    background: url(./images/icon-error.svg) no-repeat 95%;
}

#first-name:not(:focus):not(:placeholder-shown):invalid ~ #help-1 {
    display: inline-block; 
}
```

### Continued development

I want to focus on responsiveness as mobile phones have the highest traffic amongst website usage so it's important for my projects to be visible and user friendly to mobile users. By doing this, I would need to become more experienced with media queries but also want to become more familiar with pseudo selectors as they were helpful in this project.