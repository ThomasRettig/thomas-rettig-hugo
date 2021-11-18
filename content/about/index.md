---
title: "About me"
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

  label {
    font-family: var(--code-font);
  }

  .about-slider {
  	  -webkit-appearance: none;
      background: #afedcd;
      border-radius: 10px;
      width: 100%;
      height: 3.5px;
      outline: none;
  }

  .about-slider::-webkit-slider-thumb {
      -webkit-appearance: none;
      appearance: none;
      border-radius: 100%;
      width: 22px;
      height: 22px;
      background: black;
      cursor: ew-resize;
      transition: 0.2s;
  }

  .about-slider::-webkit-slider-thumb:hover {
  	width: 30px;
  	height: 30px;
  }


  .about-slider-container input {
  	margin-bottom: 1rem;
  	width: 100%;
  }

  .about-copy section {
  	display: none;
  }

  .about-copy section.visible {
  	display: block;
  }

  .infobox, .background-box {
      background: radial-gradient(#ffffff 0%, #e5fff1 85%);
      padding: 2ch;
      border-radius: 10px;
      box-shadow: 0px 4px 15px 3px #c2edd785;
      margin-bottom: 5vh;
  }

  .text-center {
    text-align: center;
  }

</style>

<p class="text-center">↓ Use the slider below to determine how much you would like to know about me ↓</p>

<div class="about-slider-container">
  <input type="range" min="1" max="5" value="3" step="1" class="about-slider" id="aboutRange" role="slider" title="Slide horizontally!">
  <label class="about-min">Less</label>
  <label class="about-max">More</label>
</div>

<div class="about-copy">
  <section value="1" style="font-size: 35px;user-select:none;">
    <p aria-label="Boy emoji, waving hand emoji, school building emoji, books emoji, and man technologist emoji">👦🏻👋🏻🏫📚👨🏻‍💻</p>
  </section>

  <section value="2">
    <p>Hi! I am a Secondary One student in Singapore. I love programming and graphic design. I am currently learning about web development. I have an email address: <a href="mailto:thomas.rettig.11@gmail.com" title="email link">thomas.rettig.11@gmail.com</a></p>
  </section>

  <section class="visible" value="3">
   	<p>Hello! I’m Thomas. I am a Secondary One student in Singapore. I love programming and graphic design. Currently, I am learning <a href="https://gohugo.io/">Hugo</a>, <a href="https://nextjs.org/">Next.js</a>, and other front-end frameworks. I’m always on the lookout for cool <smcp>CSS</smcp> and <smcp>HTML</smcp> tricks. You should probably contact him here for random <em>or</em> not-so-random messages — <a href="mailto:thomas.rettig.11@gmail.com">thomas.rettig.11@gmail.com</a></p>
  </section>

  <section value="4">
   <p>Hello! I’m Thomas and am a Secondary One student in Singapore, studying in Catholic High School. I love programming (more specifically, web development) and graphic design (more specifically, typography). Currently, I am learning <a href="https://gohugo.io/">Hugo</a>, <a href="https://nextjs.org/">Next.js</a>, and other front-end frameworks. I’m always on the lookout for cool <smcp>CSS</smcp> and <smcp>HTML</smcp> tricks. Contact me here for random <em>or</em> not-so-random messages — <a href="mailto:thomas.rettig.11@gmail.com" title="email link">thomas.rettig.11@gmail.com</a></p>
  </section>

  <section value="5">
    <p>Hello! Thanks for sliding all the way to the end!</p>
    <p>I’m Thomas, and am a Secondary One student in Singapore, studying in Catholic High School. I love programming (more specifically, web development) and graphic design (more specifically, typography). I do not have a favourite typeface. Currently, I am learning <a href="https://gohugo.io/">Hugo</a>, <a href="https://nextjs.org/">Next.js</a>, and other front-end frameworks. I’m always on the lookout for cool <smcp>CSS</smcp> and <smcp>HTML</smcp> tricks.</p>
    <p>In school, I am in the Music Elective Programme <smcp>(MEP)</smcp>, which I enjoy thoroughly. My co-curricular activity is <smcp>ION</smcp>, which is an infocomm technology society. It’s fun, but also has its <a href="../posts/my-awful-cca-trainer/">downsides</a>. Contact me here for random <em>or</em> not-so-random messages — <a href="mailto:thomas.rettig.11@gmail.com" title="email link">thomas.rettig.11@gmail.com</a>. If you’re interested in reading some stuff that I wrote, check my <a href="..">blog</a>.</p>
  </section>
</div>

<div class="infobox">
<h2>Colophon<span role="note">A note on the type</span></h2>
<p>The body text is set in the default system font. On MacOS, this is San Francisco; on Windows, this is Segoe UI. If you are seeing Comic Sans, please contact me urgently.
<p>Article headings are set in <a href="https://www.nan.xyz/fonts/nan-jaune/" target="blank">NaN Jaune Maxi</a>, a lively sans-serif by Jérémy Landes of <a href="https://studiotriple.fr/" target="blank">Studio Triple</a>. Visit the <a href="http://www.sanssheriff.wtf/" target="blank">excellent microsite</a> to learn more!</p>
</div>

<div class="infobox">
<h2>License<span role="note">Can I reproduce parts of this blog?</span></h2>
  <p>Unless otherwise stated, all <em>source code</em> is licensed under <a href="https://www.gnu.org/licenses/agpl-3.0.en.html" target="blank">GNU AGPL version 3.0</a>. The <b>main thing you cannot do</b> is to publish your modified work under a different license.</p>
  <p>All other blog content is licensed under the <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/" target="blank">Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)</a> license.</p>
</div>

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