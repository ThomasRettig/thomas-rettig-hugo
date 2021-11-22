---
title: "“Hello world” in CSS?"
date: 2021-11-06
draft: false
---

Yes, you can! Thanks to this [insightful article](https://css-tricks.com/is-css-a-programming-language/) by Chris Coyier over at CSS-Tricks—athough this is more of an edge case. Here’s what he says:

<smcp>CSS</smcp> can’t do that! Um, well, unless you write `body::after { content: "Hello, World!"; }` in ```style.css``` file and open a web page that loads that <smcp>CSS</smcp> file. So <smcp>CSS</smcp> does execute, in its own special way. It’s a domain-specific language (<smcp>DSL</smcp>) rather than a general-purpose language (<smcp>GPL</smcp>). In that browser context, the way <smcp>CSS</smcp> is told to run (`<link>`, usually) isn’t even that different from how JavaScript is told to run (```<script>```, usually).

So, to sum up:

```css
body::after {
    content: "Hello World!";
}
```

can produce something like this:

<iframe height="300" style="width: 100%;" scrolling="no" title="CSS Hello World" src="https://codepen.io/ThomasRettig/embed/QWMmEGQ?default-tab=css%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true"></iframe>

This is pretty obvious, but it just goes to show that... <smcp>CSS</smcp> _can_ in fact print ```Hello World```. Of course, <smcp>CSS</smcp> But the larger argument that Chris makes, is that, while CSS might not be the first candidate for Turing completeness, it does in fact contain some programming concepts inside.

## CSS is a programming language! <span>Here’s why</span>

- <smcp>CSS</smcp> selectors are simply ```if``` statements running over loops of matches
- ```calc()``` is a direct implementation of math ([check this!](https://medium.com/buildit/hardcore-css-calc-bdfb0162993c))
- Media queries are switches
- Custom properties are a place to store states
- ```:checked``` is a boolean

And, my own contribution: Aren’t ```!important``` and ```@supports``` both proof that <smcp>CSS</smcp> is a programming language, in its own, albeit special, way?

Chris asserts that the bigger picture is about pay. His concern: If <smcp>CSS</smcp> is not regarded as a true programming language, would <smcp>CSS</smcp> specialists get lower pay than their counterparts?

## Direct link

[https://css-tricks.com/is-css-a-programming-language/](https://css-tricks.com/is-css-a-programming-language/)