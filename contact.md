---
title: Contact Us
permalink: /contact.html
---

<form action="https://formspree.io/your@email.com"
      method="POST">
    <input type="text" name="name">
    <input type="email" name="_replyto">
    <input type="hidden" name="_next" value="{{ site.baseurl }}" />
    <input type="text" name="_gotcha" style="display:none" />
    <input type="submit" value="Send">
</form>