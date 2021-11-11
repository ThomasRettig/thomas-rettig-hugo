---
title: The genius of Waifu2x
draft: false
date: 2021-11-11
---

<link rel="stylesheet" href="https://unpkg.com/beerslider/dist/BeerSlider.css">

Yes, it’s an ungainly name. It has a gigantic file size of 3.5GB. It’s [user interface](https://res.cloudinary.com/cloudinary-sucks-so-fucking-much/image/upload/v1636614022/Waifu_Screenshot_q3o3xe.jpg) is a big mess. But [Waifu2x](https://github.com/AaronFeng753/Waifu2x-Extension-GUI), developed by Aaron Feng, is just genius—it uses artificial intelligence to “upscale” images. This idea isn’t the first of its kind, but it is easily the very best. And, it’s open-source! Take a look:

{{< figure src="https://res.cloudinary.com/cloudinary-sucks-so-fucking-much/image/upload/v1636615025/Waifu_Tree_Sample_gnjh3a.png" title="Sample Image—Nature" caption="A before-after comparison." >}}

Isn’t that amazing? Just to note:

- The first frame is the original unprocessed version
- The second frame is processed with the ```3D Real-life - Enlarge only - Fast``` preset
- The third frame is processed with the ```3D Real-life - Enlarge only - Highest Quality ``` preset

Waifu2x also scores excellently with 2D images, such as this Tom and Jerry photo. The lines are crisp, contour is accurate, and there are hardly any visual artifacts present!

{{< figure src="https://res.cloudinary.com/cloudinary-sucks-so-fucking-much/image/upload/v1636615996/Waifu_Anime_Sample_nieukq.png" title="Sample Image—Anime" caption="A before-after comparison." >}}

A side note though—Waifu2x does _not_ score terribly well when it comes to us earthlings. After shoving a 150px×150px Hide the Pain Harold picture into the app (sorry), this is what I got:

{{< figure src="https://res.cloudinary.com/cloudinary-sucks-so-fucking-much/image/upload/v1636616856/Waifu_Face_Test_cbe8ij.png" title="Sample Image—Human" caption="A before-after comparison." >}}

A bit unflattering, right? (Not that he was in the first place.) Just look at those eyes! Surprisingly, the “fast” preset (second frame) looks better than the “highest quality” preset (third frame). My hunch is that the presets were trained based on different datasets which led to such a big difference in output. However, there is still too much denoising present in both images. In fact, I would even argue that the original image looks even better despite being scaled up 5 times.

Either way, Waifu2x still manages to impress. It’s main advantages are:

- It’s offline (you get to ditch the upload process on online websites)
- It’s open-source
- It has advanced customisation options

I’ve just discovered it, and can’t wait to try it out in real-world settings. I haven’t even touched on its video upscaling abilities yet! In the future, I imagine a day when artificial intelligence gets so advanced that such upscaling software could be built into video conferencing apps on our everyday devices (though it will probably kill the entire webcam industry). Waifu2x is also built in [C++](https://en.wikipedia.org/wiki/C%2B%2B), so it would be interesting to see if similar software could be written in a different language. Maybe even a web app that upscales without server uploading with [Rust](https://www.rust-lang.org/) and <smcp>[WASM](https://webassembly.org/)</smcp>?
