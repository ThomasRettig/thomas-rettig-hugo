---
title: Stop using Tailwind CSS
draft: false
date: 2021-11-19
---

Stop using [Tailwind CSS](https://tailwindcss.com/). Or [Bulma.io](https://bulma.io/), [Bootstrap](https://getbootstrap.com/docs/3.4/css/), or [Atomic CSS](https://acss.io/) for the matter. If you are using it, stop. If you haven’t, avoid it.

## 1. HTML is HTML <span>it’s not CSS</span>

Directly adding CSS into HTML sounds awful, looks awful, and _is_ awful. HTML is a markup language for semantically structuring documents, not a dumping ground for obscure utility classes attached to elements. It prevents readability. It’s bad for you, the user, and the search engine—it sucks. Some front-end designers share my same distaste:

<blockquote>Indeed, the ultimate reason for the invention of CSS, the whole point of the entire enterprise of CSS... was specifically so that you could seperate content from presentation.</blockquote>

<cite>—[Bryan Boyko](https://dev.to/brianboyko/tailwindcss-adds-complexity-does-nothing-3hpn) on Tailwind CSS</cite>

Chris Coyier agrees, too:

<blockquote>
I don’t like all the classes. I like to express my styles in CSS because I find CSS… good.    
</blockquote>

<cite>—[Chris Coyier](https://css-tricks.com/reimagine-atomic-css) on Atomic CSS</cite>

## 2. There are more efficient ways to write CSS <span>SASS, Less, Stylus</span>

If you are looking for an efficient way to write CSS, stop using Tailwind and start using preprocessors. These include <abbr title="Syntactically Awesome Style Sheets">SASS</abbr>, [Less](https://lesscss.org/), and [Stylus](https://stylus-lang.com/). They are effective because they readable, as compared to bulky Tailwind. And they also have much more functionality. The best part is that they are seperated from the HTML, ensuring high readability. Just look at this image below showing the amount of Tailwind syntax needed to style a button:

{{< figure src="/tailwind-netlify.webp" caption="Image by [Aleksandr Hovhannisyan](https://www.aleksandrhovhannisyan.com/)" alt="Alt text" >}}

## 3. Tailwind is unreadable <span>Nightmarishly complex syntax</span>

No one can understand what you’re doing in Tailwind. That’s because the syntax is nightmarishly complex and incomprehensible. It adds unnecessary bulk. If I pass you an HTML file with Tailwind CSS jargon inside, would you be able to immediately modify and understand it? Probably not. Tailwind’s syntax is vague and quirky, requiring a lot of time spent in understanding it. And even if you master it, chances are, Tailwind is still not the smartest option around. Yes, you can purge it or generate it just-in-time, but is it worth all the hassle? I still prefer working with plain CSS files. Therefore, if you are concerned about the ease of reading, Tailwind just isn’t right.

## Conclusion

Tailwind is _not_ HTML, there are more efficient ways to write CSS, such as using preprocessors, and Tailwind is unreadable to humans. The bottom line: Avoid it. It does more harm than good.
