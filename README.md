# Just an old proof of concept

It's an old piece of code I made when I wanted to know more about some of the lesser-used Javascript features.
The idea was to get familiar with the idea of template litterals string tags.

This piece of codes makes a template litteral string tag function that transforms an HTML string to the appropriate HTMLELement object.

It's used as follow :
```js
  const myLink = html`
  <a href="https://prologin.org/">
    Cliquez ici ! <img src="./cute-cat.jpg" alt="Un chat trop mignon !"> 
  </a>`;
```

The concept is similar to what Google's `lit-html` library is achieving.

## Known Limitation
Though there's no limitation on the number of child elements, you should only have one top-level element in the provided HTML, as the function is made to output a single HTML element, not an array of HTML elements.
