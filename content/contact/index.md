---
title: Contact Me
draft: false
---
For longer messages, consider sending me an email instead. This form is mainly for brief messages 🙃

<form name="contact" id="form" netlify>
    <p><label>Choose a subject:</label>
      <select name="subject" title="click to view dropdown" required>
        <option value="Website issue">Website issue</option>
        <option value="Something else">Something else</option>
      </select>
    </p>
    <p>
      <label>What’s your name?<input type="text" name="name" placeholder="eg Donald Trump" required /></label>
    </p>
    <p>
      <label>Email <small>(optional)</small><input type="email" name="email" placeholder="eg trump@gmail.com" /></label>
    </p>
    <p>
      <label>Your message<textarea type="text" name="message" required placeholder="Your message…" /></textarea>
    </p>
  </section>
  <p>
    <button type="submit"><span>S</span><span>e</span><span>n</span><span>d</span><span>!</span></button>
  </p>
</form>