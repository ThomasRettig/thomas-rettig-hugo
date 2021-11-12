---
title: Cleanup.pictures
draft: false
date: 2021-11-12
---

[Cleanup.pictures](https://cleanup.pictures/) does exactly what it does: It cleans up pictures. You draw over areas of an image and it automagically removes that part. Yes, it’s like Photoshop’s spot healing brush tool, except that it’s a website and it’s free. And unlike primitive spot healing tools which rely on surroundings to “import” textures, Cleanup.pictures uses artificial intelligence. The science is complex; it’s built using artificial intelligence. As far as I can tell, its network architecture uses Fourier convolutions. But of course, no one really cares about that nonsense.

Here’s an example from their [Github repo](https://saic-mdal.github.io/lama-project/):

{{< figure src="https://raw.githubusercontent.com/senya-ashukha/senya-ashukha.github.io/master/projects/lama_21/ezgif-4-0db51df695a8.gif" >}}

That was spooky, wasn’t it? I was a bit sceptical, so I tried it out myself just for good measure:

{{< figure src="https://res.cloudinary.com/cloudinary-sucks-so-fucking-much/image/upload/v1636704470/cleanup-test.webp" title="Before and after comparison" >}}

Amazing. It also finished processing faster than I thought, considering how
- cleanup.pictures is a web app
- I was using a high-resolution image
- I had selected a big area to heal

Just like Waifu2x-Extension-GUI, the photo/video upscaling software I [recently reviewed](../waifu2), I really look forward to using this in the future. Photobombers, beware! It would also be super interesting to have some sort of “who-heals-the-best” software competition. Not to mention, [Cleanup.pictures](https://cleanup.pictures/) has a really nice how-did-they-snag-that-url domain, just like [remove.bg](https://remove.bg/) and [clipdrop.co](https://clipdrop.co/). Top find of the week!

Note: The website is created by [Cyril Diagne](https://twitter.com/cyrildiagne), and is a direct implementation of this [scientific paper](https://arxiv.org/pdf/2109.07161.pdf).

