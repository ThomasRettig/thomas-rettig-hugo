---
title: Online spot healing — better than I thought
draft: false
date: 2021-11-12
---

[Cleanup.pictures](https://cleanup.pictures/) does exactly what it does: It cleans up pictures. You draw over areas of an image and it automagically removes that part. Yes, it’s like Photoshop’s spot healing brush tool, except that it’s a website and it’s free. And unlike primitive spot healing tools which rely on surroundings to “import” textures, Cleanup.pictures uses artificial intelligence. The science is complex; AFAIK, its network architecture uses Fourier convolutions. But of course, I don’t really know what that is, and no one really cares about that.

Here’s a before-after example from their [Github repo](https://saic-mdal.github.io/lama-project/):

{{< figure src="https://raw.githubusercontent.com/senya-ashukha/senya-ashukha.github.io/master/projects/lama_21/ezgif-4-0db51df695a8.gif" >}}

That was spooky, wasn’t it? I was a bit sceptical, so I tried it out myself just for good measure:

{{< figure src="https://res.cloudinary.com/cloudinary-sucks-so-fucking-much/image/upload/v1636704470/cleanup-test.webp" title="Before and after comparison" >}}

Amazing. It also finished processing faster than I thought, considering how
- [Cleanup.pictures](https://cleanup.pictures/) is a web app
- I was using a high-resolution image
- I had selected a big area to heal

Admittedly, [Cleanup.pictures](https://cleanup.pictures/) is a trifle slower than Photoshop and [Snapseed](https://en.wikipedia.org/wiki/Snapseed), but considering how this is based on a highly developed neural network, I am not too terribly bothered—accuracy is more important than speed. Another downside is that the website partially resizes my image to speed up processing on their servers. I suppose if I built the entire thing from the Github server I could ditch the resizing part, but I don’t run a supercomputer and my humble PC could possibly crash.

I’m sure the technology still has many flaws, especially in very specific use cases. So, while my experience trying out the app could be positive, it may not be for everyone else, in particular those who rely on it on a daily basis.

That said, just like Waifu2x-Extension-GUI, the photo/video upscaling software I [recently reviewed](../waifu2), I really look forward to using this in the future. Photobombers, beware! It would also be super interesting to have some sort of “who-heals-the-best” software competition. Not to mention, [Cleanup.pictures](https://cleanup.pictures/) has a really nice how-did-they-snag-that-url domain, just like [remove.bg](https://remove.bg/) and [clipdrop.co](https://clipdrop.co/). Top find of the week!

Note: The website is created by [Cyril Diagne](https://twitter.com/cyrildiagne), and is a direct implementation of this [scientific paper](https://arxiv.org/pdf/2109.07161.pdf).