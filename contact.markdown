---
layout: page
title: Contact
permalink: /contact/
---

<div class="form-container">
  <form name="contact" method="POST" data-netlify="true" netlify-honeypot="bot-field" action="/success">
    <input type="hidden" name="form-name" value="contact">
    
    <div class="form-group">
      <label for="name" class="required-field">Name</label>
      <input type="text" id="name" name="name" placeholder="John Smith" required>
      <span class="help-text">Who are you?</span>
    </div>
    
    <div class="form-group">
      <label for="email" class="required-field">Email</label>
      <input type="email" id="email" name="email" placeholder="john.smith@example.com" required>
      <span class="help-text">I will never share your email without permission.</span>
    </div>
    
    <div class="form-group">
      <label for="subject" class="required-field">Subject</label>
      <input type="text" id="subject" name="subject" placeholder="A subject to be discussed" required>
      <span class="help-text">What's on your mind?</span>
    </div>
    
    <div class="form-group">
      <label for="message" class="required-field">Message</label>
      <textarea id="message" name="message" placeholder="Tell me more..." required></textarea>
      <span class="help-text">How can I help you?</span>
    </div>
    
    <p style="display:none">
      <label>Don't fill this out if you're human: <input name="bot-field"></label>
    </p>
    
    <button type="submit" class="submit-btn">Submit</button>
  </form>
</div>
