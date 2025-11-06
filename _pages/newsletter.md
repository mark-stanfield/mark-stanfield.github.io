---
# _pages/newsletter.md
layout: default
title: Newsletter
---

# ALPFA Gotham City Newsletter

## Latest Updates

<!-- Example: Link to a specific newsletter post using Jekyll Collections -->
{% if site.newsletters.size > 0 %}
  <h2>Recent Issues</h2>
  <ul>
    {% for newsletter in site.newsletters limit: 5 %} <!-- Show last 5 newsletters -->
      <li><a href="{{ newsletter.url | relative_url }}">{{ newsletter.title }} - {{ newsletter.date | date: "%B %d, %Y" }}</a></li>
    {% endfor %}
  </ul>
{% endif %}

<!-- Example: Link to all newsletter posts -->
<p><a href="{{ '/newsletters/' | relative_url }}">View All Newsletters</a></p>

<!-- Example: Static content for the main newsletter page -->
<h2>Stay Informed</h2>
<p>Our newsletter keeps you updated on chapter events, member highlights, professional development opportunities, and news relevant to the Latino professional community.</p>

<!-- Example: Subscription Form (Placeholder - requires backend) -->
<form>
  <h3>Subscribe to Our Newsletter</h3>
  <label for="email">Email Address:</label>
  <input type="email" id="email" name="email" required>
  <button type="submit" class="btn">Subscribe</button>
</form>
