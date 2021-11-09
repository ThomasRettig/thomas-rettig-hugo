---
title: "Hi, I’m Thomas."
draft: false
---
<style>
.about-slider-container {
	display: flex;
	flex-wrap: wrap;
	justify-content: space-between;
	margin: 4rem auto;
	width: 100%;
	font-family: var(--body-font);
}

.about-slider {
	-webkit-appearance: none;
    width: 100%;
    height: 1px;
    background: #ddd;
    outline: none;
}

.about-slider::-webkit-slider-thumb {
    -webkit-appearance: none;
    appearance: none;
    border-radius: 100%;
    width: 16px;
    height: 16px;
    background: black;
    cursor: grab;
}

.about-slider::-webkit-slider-thumb:hover {
	width: 20px;
	height: 20px;
	border-radius: 100%;
}


.about-slider-container input {
	margin-bottom: 1rem;
	width: 100%
}

.about-copy section {
	display: none
}

.about-copy section.visible {
	display: block
}

label {
	user-select: none;
	font-family: var(--code-font);
}

.background-box {
	border-radius: 10px;
	padding: 15px;
	background: #ececec;
}

@media (prefers-color-scheme: dark) {
	.about-slider::-webkit-slider-thumb {
		background: white;
	}

	.background-box {
		background: #113341;
	}
}

</style>

<p class="background-box">Use the slider below to determine how much you would like to know about me.</p>

<div class="about-slider-container">
  <input type="range" min="1" max="5" value="3" step="1" class="about-slider" id="aboutRange" role="slider">
  <label class="about-min">Less</label>
  <label class="about-max">More</label>
</div>

<div class="about-copy">
  <section value="1" style="font-size: 35px;user-select:none;">
    <p aria-label="Boy emoji, waving hand emoji, school building emoji, books emoji, and man technologist emoji">👦🏻👋🏻🏫📚👨🏻‍💻</p>
  </section>

  <section value="2">
    <p>Hi! I am a Secondary One student in Singapore. I love programming and graphic design. I am currently learning about web development. I have an email address: <a href="mailto:thomas.rettig.11@gmail.com">thomas.rettig.11@gmail.com</a></p>
  </section>

  <section value="3">
   	<p>Hello! I’m Thomas. I am a Secondary One student in Singapore. I love programming and graphic design. Currently, I am learning <a href="https://gohugo.io/">Hugo</a>, <a href="https://nextjs.org/">Next.js</a>, and other front-end frameworks. I’m always on the lookout for cool <smcp>CSS</smcp> and <smcp>HTML</smcp> tricks. You should probably contact him here for random <em>or</em> not-so-random messages — <a href="mailto:thomas.rettig.11@gmail.com">thomas.rettig.11@gmail.com</a></p>
  </section>

  <section class="visible" value="4">
   <p>Hello! I am a Secondary One student in Singapore, studying in Catholic High School.</p>
   <p>I love programming (more specifically, web development) and graphic design (more specifically, typography). Currently, I am learning <a href="https://gohugo.io/">Hugo</a>, <a href="https://nextjs.org/">Next.js</a>, and other front-end frameworks. I’m always on the lookout for cool <smcp>CSS</smcp> and <smcp>HTML</smcp> tricks. Contact me here for random <em>or</em> not-so-random messages — <a href="mailto:thomas.rettig.11@gmail.com">thomas.rettig.11@gmail.com</a></p>
  </section>

  <section value="5">
    <p>Hello! Thanks for sliding all the way to the end!</p>
    <p>I am a Secondary One student in Singapore, studying in Catholic High School. I love programming (more specifically, web development) and graphic design (more specifically, typography). I do not have a favourite typeface. Currently, I am learning <a href="https://gohugo.io/">Hugo</a>, <a href="https://nextjs.org/">Next.js</a>, and other front-end frameworks. I’m always on the lookout for cool <smcp>CSS</smcp> and <smcp>HTML</smcp> tricks.</p>
    <p>In school, I am in the Music Elective Programme <smcp>(MEP)</smcp>, which I enjoy thoroughly. My co-curricular activity is <smcp>ION</smcp>, which is an infocomm technology society. It’s fun, but also has its <a href="../posts/my-awful-cca-trainer/">downsides</a>. Contact me here for random <em>or</em> not-so-random messages — <a href="mailto:thomas.rettig.11@gmail.com">thomas.rettig.11@gmail.com</a>. If you’re interested in reading some stuff that I wrote, check my <a href="..">blog</a>.</p>
  </section>
</div>

<hr>

## Accessibility

I take accessibility seriously, and have tried my best to make this site as accessible as I can. Images come with descriptive titles and focus states are clearly highlighted. Please refer to the table below if you want to feedback on specific aspects of accessibility.

| Conditions                                | Common symptoms                                              |
| ----------------------------------------- | ------------------------------------------------------------ |
| Assistive technology (such as voice over) | If you are experiencing trouble viewing a particular part of this website, like video, audio and embedded ```iframes```, <a href="mailto:thomas.rettig.11@gmail.com" title="email link">contact me.</a> |
| Colour-blind and/or sight-impaired        | If you are having colour contrast or font legibility issues, <a href="mailto:thomas.rettig.11@gmail.com" title="email link">contact me.</a> |
| Caret browsing users                      | If an nteractive element is unintendedly uninteractive, please <a href="mailto:thomas.rettig.11@gmail.com" title="email link">contact me.</a> |

<hr>

## Colophon

The body text in this site is set in <smcp>[Source Serif 4](https://github.com/adobe-fonts/source-serif)</smcp>, an open-source text typeface designed by Frank Grießhammer published by Adobe Fonts. It is a transitional serif face inspired by the types of [Pierre-Simon Fournier](https://en.wikipedia.org/wiki/Pierre_Simon_Fournier). In particular, I am using the caption optical size to optimise legibility.

Type nerds may read the release notes [here](https://github.com/adobe-fonts/source-serif/releases/tag/4.004R), or check out [Adobe’s official blog post](https://blog.adobe.com/en/publish/2021/03/04/source-serif-gets-optical-sizes.html#gs.6de1ff). Support open-source! I am using self-hosted versions because Google Fonts has not (yet) upgraded their existing Source Serif Pro to the latest version.

Article headings are set in <smcp>[Mānuka](https://klim.co.nz/retail-fonts/manuka/)</smcp>, designed by Klim Type Foundry. <smcp>Mānuka</smcp> a condensed display typeface with inspired by historical German wood type. Kris Sowersby, its principal designer, describes it beautifully:

<blockquote>“Mānuka is new growth from old wood. With deviant details pilfered from Teutonic timber type, Mānuka grafts a contemporary antipodean aesthetic onto 19th century German root-stock.”</blockquote><figcaption>—Kris Sowersby, <cite><a href="">Mānuka design notes</a></cite></figcaption>

Users who have system-wide dark mode turned on would also notice the article title painted with a vibrant gradient.


  <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
  <script>

var rangeSlider = function(){
  var slider = $('.about-slider-container'),
      range = $('.about-slider'),
      value = $('.about-slider__value');

  slider.each(function(){

    value.each(function(){
      var value = $(this).prev().attr('value');
      $(this).html(value);
    });

    range.on('input', function(){
      var currentValue = $(this).val()
      // var previousValue = parseInt($(this).val()) - 1
      // var nextValue = parseInt($(this).val()) + 1

      var currentSection = $("section[value='" + currentValue + "']")
      // var previousSection = $("section[value='" + previousValue + "']")
      // var nextSection = $("section[value='" + nextValue + "']")

      currentSection.addClass("visible");
      $("section").not(currentSection).removeClass("visible");
      // nextSection.removeClass("visible");
      // previousSection.removeClass("visible");
    });
  });
};

rangeSlider();
</script>