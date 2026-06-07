---
layout: default
title: Contact
---

<div class="contact-container">
    <header class="contact-header">
        <h1>Get in <em>touch.</em></h1>
        <p class="subtitle">Have a question about the resources or just want to say hello? I'd love to hear from you.</p>
    </header>

    <div class="contact-form-wrapper">
        <form action="https://api.web3forms.com/submit" method="POST" id="form">
            <input type="hidden" name="access_key" value="YOUR_ACCESS_KEY_HERE">
            <input type="hidden" name="subject" value="New Contact from Timeless Guide">
            <input type="checkbox" name="botcheck" id="" style="display: none;">

            <div class="form-group">
                <label for="name">Full Name</label>
                <input type="text" name="name" id="name" placeholder="Your name" required>
            </div>

            <div class="form-group">
                <label for="email">Email Address</label>
                <input type="email" name="email" id="email" placeholder="email@example.com" required>
            </div>

            <div class="form-group">
                <label for="message">Message</label>
                <textarea name="message" id="message" rows="5" placeholder="How can I help?" required></textarea>
            </div>

            <button type="submit" class="btn-sage form-submit">Send Message</button>
            <div id="result"></div>
        </form>
    </div>
</div>