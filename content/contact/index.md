---
title: Contact Me
draft: false
---
<style>
  body {
    background: #ebd1ff;
  }

  button[type=submit]:hover {
      background: rebeccapurple;
  }

  ::selection {
    background: #d9aaff;
    color: black;
  }

  ::placeholder {
      color: #113341;
      opacity: 0.5;
      font-weight: 500;
      font-size: inherit;
  }
</style>
For longer messages, consider sending me an email instead. This form is mainly for brief messages 🙃

<form name="contact" id="form" netlify>
    <p><label>Choose a subject:</label>
      <select name="subject" required>
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
    <button type="submit">Submit</button>
  </p>
</form>