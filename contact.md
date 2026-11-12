---
layout: default
title: "Contact"
permalink: /contact/
description: "Contact Dr. Soneya Binta Hossain and the AS²ERT Lab at UT Dallas."
---

{% include page-head.html eyebrow="AS²ERT Lab" title="Contact" lede="Have a question or want to collaborate? Reach out!" %}

<div class="wrap">
  <div class="contact-grid">

    <div class="contact-info">
      <dl>
        <dt>Email</dt>
        <dd><a href="mailto:{{ site.email }}">{{ site.email }}</a></dd>
        <dt>Address</dt>
        <dd>Department of Computer Science<br>The University of Texas at Dallas</dd>
      </dl>
    </div>

    <div class="form">
      <h2>Message me</h2>
      <form target="_blank" action="https://formsubmit.co/{{ site.email }}" method="POST">
        <div class="field">
          <label for="name">Name</label>
          <input type="text" name="name" id="name" required>
        </div>
        <div class="field">
          <label for="email">Email</label>
          <input type="email" name="email" id="email" required>
        </div>
        <div class="field">
          <label for="message">Message</label>
          <textarea name="message" id="message" rows="6" required></textarea>
        </div>
        <button class="btn btn-primary" type="submit">Send message</button>
      </form>
    </div>

  </div>
</div>
