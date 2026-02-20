---
layout: home
title: Home
---

# Innovate. Learn. Build.
Showcasing our products, sharing knowledge, and empowering creators.

---

### Our Products
<ul>
  {% for product in site.products %}
    <li>
      <strong><a href="{{ product.url | relative_url }}">{{ product.title }}</a></strong> 
      {% if product.price %} - {{ product.price }}{% endif %}
    </li>
  {% endfor %}
</ul>

### Latest Instructions
<ul>
  {% for guide in site.instructions %}
    <li>
      <a href="{{ guide.url | relative_url }}">{{ guide.title }}</a> 
      <small>(Multimedia Guide)</small>
    </li>
  {% endfor %}
</ul>

---

### Support
Found a bug or need help? [Report an Issue]({{ "/report-issue/" | relative_url }})
