# 🎨 Customization Guide

All customization happens inside `index.html`. Here's exactly where to find each section.

---

## Colors & Theme Tokens

Find the `:root` block near the top of `<style>`:

```css
:root {
  --gold:        #d4a843;   /* Primary accent — change to your brand color */
  --gold-light:  #f0c96a;
  --gold-dark:   #a87e28;
  --charcoal:    #1a1a1a;   /* Dark background */
  --text-primary:#f5f0e8;   /* Main text */
  /* ... */
}
```

---

## Profile Photo

Replace the `src` of the `<img class="profile-avatar">` tag:

```html
<img
  src="https://0.gravatar.com/avatar/YOUR_HASH?size=256"
  alt="Your Name profile photo"
  class="profile-avatar"
/>
```

Or use a local image:
```html
src="assets/images/profile.jpg"
```

---

## Hero Text

```html
<h1 class="hero-name">
  <span class="highlight">Your First</span><br />LastName
</h1>
<p class="hero-tagline">Your Title Here</p>
<p class="hero-description">Your bio paragraph...</p>
```

---

## Stats Numbers

```html
<span class="profile-stat-n" data-counter="5">0</span>
<!-- Change the data-counter value — the JS animates to this number -->
```

---

## Projects

Each project card follows this pattern — duplicate or edit as needed:

```html
<article class="glass-card project-card reveal">
  <div class="project-icon"><i data-lucide="ICON_NAME" size="22"></i></div>
  <h3 class="project-title">Project Title</h3>
  <p class="project-desc">Project description here.</p>
  <div class="project-tags">
    <span class="chip">Tag1</span>
  </div>
  <a href="YOUR_GITHUB_URL" class="project-link">
    View Repository <i data-lucide="arrow-right" size="14"></i>
  </a>
</article>
```

Browse available Lucide icons at [lucide.dev](https://lucide.dev).

---

## Certifications Carousel

Add or remove `.glass-card.cert-card` divs inside `#certTrack`:

```html
<div class="glass-card cert-card">
  <div class="cert-icon"><i data-lucide="award" size="28"></i></div>
  <div class="cert-title">Certificate Name</div>
  <div class="cert-issuer">Issuing Body · Date</div>
</div>
```

---

## Pricing

Update the prices and feature lists in the three `.pricing-card` divs under `#pricing`.

---

## FAQ

Add more FAQ items by copying this block inside `.faq-list`:

```html
<div class="faq-item">
  <button class="faq-question" aria-expanded="false">
    Your question here?
    <span class="faq-icon"><i data-lucide="plus" size="14"></i></span>
  </button>
  <div class="faq-answer" hidden>
    <p>Your answer here.</p>
  </div>
</div>
```

---

## Social Links

Update the `href` values in the `.social-links` sections (both hero and footer).

---

## Google Maps Location

In `#contact`, replace the iframe `src` with your location:

```html
<iframe
  src="https://maps.google.com/maps?q=YOUR+CITY,COUNTRY&output=embed"
  ...
></iframe>
```

---

## Fonts

In the `<head>`, change the Google Fonts import URL to your preferred fonts, then update the CSS variables:

```css
--font-display: 'Your Display Font', serif;
--font-body:    'Your Body Font', sans-serif;
--font-mono:    'Your Mono Font', monospace;
```
