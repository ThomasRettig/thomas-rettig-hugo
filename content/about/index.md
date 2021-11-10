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
    transition: 0.2s;
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
    <p aria-label="Boy emoji, waving hand emoji, school building emoji, books emoji, and man technologist emoji"><span style="margin-right: -6px;">👦🏻</span>👋🏻🏫📚👨🏻‍💻</p>
  </section>

  <section value="2">
    <p>Hi! I am a Secondary One student in Singapore. I love programming and graphic design. I am currently learning about web development. I have an email address: <a href="mailto:thomas.rettig.11@gmail.com">thomas.rettig.11@gmail.com</a></p>
  </section>

  <section value="3">
   	<p>Hello! I’m Thomas. I am a Secondary One student in Singapore. I love programming and graphic design. Currently, I am learning <a href="https://gohugo.io/">Hugo</a>, <a href="https://nextjs.org/">Next.js</a>, and other front-end frameworks. I’m always on the lookout for cool <smcp>CSS</smcp> and <smcp>HTML</smcp> tricks. You should probably contact him here for random <em>or</em> not-so-random messages — <a href="mailto:thomas.rettig.11@gmail.com">thomas.rettig.11@gmail.com</a></p>
  </section>

  <section class="visible" value="4">
   <p>Hello! I’m Thomas and am a Secondary One student in Singapore, studying in Catholic High School. I love programming (more specifically, web development) and graphic design (more specifically, typography). Currently, I am learning <a href="https://gohugo.io/">Hugo</a>, <a href="https://nextjs.org/">Next.js</a>, and other front-end frameworks. I’m always on the lookout for cool <smcp>CSS</smcp> and <smcp>HTML</smcp> tricks. Contact me here for random <em>or</em> not-so-random messages — <a href="mailto:thomas.rettig.11@gmail.com">thomas.rettig.11@gmail.com</a></p>
  </section>

  <section value="5">
    <p>Hello! Thanks for sliding all the way to the end!</p>
    <p>I’m Thomas, and am a Secondary One student in Singapore, studying in Catholic High School. I love programming (more specifically, web development) and graphic design (more specifically, typography). I do not have a favourite typeface. Currently, I am learning <a href="https://gohugo.io/">Hugo</a>, <a href="https://nextjs.org/">Next.js</a>, and other front-end frameworks. I’m always on the lookout for cool <smcp>CSS</smcp> and <smcp>HTML</smcp> tricks.</p>
    <p>In school, I am in the Music Elective Programme <smcp>(MEP)</smcp>, which I enjoy thoroughly. My co-curricular activity is <smcp>ION</smcp>, which is an infocomm technology society. It’s fun, but also has its <a href="../posts/my-awful-cca-trainer/">downsides</a>. Contact me here for random <em>or</em> not-so-random messages — <a href="mailto:thomas.rettig.11@gmail.com">thomas.rettig.11@gmail.com</a>. If you’re interested in reading some stuff that I wrote, check my <a href="..">blog</a>.</p>
  </section>
</div>

<details>
<summary title="Click to expand or close">Accessibility <span role="note">Accessibility issues?</span></summary>
<p>I take accessibility seriously, and have tried my best to make this site as accessible as I can. Images come with descriptive titles and focus states are clearly highlighted. Please refer to the table below if you want to feedback on specific aspects of accessibility.</p>

| Conditions                                | Common symptoms                                              |
| ----------------------------------------- | ------------------------------------------------------------ |
| Assistive technology (such as voice over) | Trouble viewing a particular part of this website, like video, audio and embedded ```iframes```. |
| Colour-blind and/or sight-impaired        | Colour contrast or font legibility issues.
| Caret browsing users                      | An interactive element is unintendedly uninteractive. |

If what you are experiencing matches the above, please contact me in the “contact form” section below.
</details>

<details>
  <summary title="Click to expand or close">Colophon<span role="note">A note on the type</span></summary>
<p>The body text in this site is set in <smcp><a href="https://github.com/adobe-fonts/source-serif">Source Serif 4</a></smcp>, an open-source text typeface designed by Frank Grießhammer. It is a transitional serif face inspired by the types of <a href="https://en.wikipedia.org/wiki/Pierre_Simon_Fournier). In particular, I am using the caption optical size to optimise legibility">Pierre-Simon Fournier</a>.</p>

Type nerds may read the release notes [here](https://github.com/adobe-fonts/source-serif/releases/tag/4.004R), or check out [Adobe’s official blog post](https://blog.adobe.com/en/publish/2021/03/04/source-serif-gets-optical-sizes.html#gs.6de1ff). Support open-source!

Article headings are set in [Mānuka](https://klim.co.nz/retail-fonts/manuka/), designed by Klim Type Foundry. Mānuka a condensed display typeface with inspired by historical German wood type. Kris Sowersby, its principal designer, describes it beautifully:

<blockquote>“Mānuka is new growth from old wood. With deviant details pilfered from Teutonic timber type, Mānuka grafts a contemporary antipodean aesthetic onto 19th century German root-stock.”</blockquote><figcaption>—Kris Sowersby, <cite><a href="">Mānuka design notes</a></cite></figcaption>

Users who have system-wide dark mode turned on would also notice the article title painted with a vibrant gradient.
</details>

<details>
  <summary title="Click to expand or close">Contact Form<span role="note">Leave a short note for me</span></summary>
<form name="contact" id="form" netlify>
  <section class="contact">
    <p>
      <label>Name <input type="text" name="name" /></label>
    </p>
    <p>
      <label>Email <input type="email" name="email" /></label>
    </p>
    <p>
      <label>Your message <input type="text" name="message" style="height: 100px;width: 80%;" /></label>
    </p>
  </section>
  <p>
    <button type="submit">Send!</button>
  </p>
</form>
</details>


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