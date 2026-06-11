# The Static — STV Radiomeltdown Hub

**Live home for all issues, exclusive interviews, and partner cards.**  
Built for STV Radiomeltdown · G4E Movement Studio · Lithonia, GA

---

## What This Is

`the-static-hub.html` is a single-file standalone website that houses:

- **The Static** newsletter issues as photo/video cards with story highlights
- **Month tabs** to filter issues by publish date
- **A B2B landing section** for churches and luxury brands interested in a dedicated player
- **Faire Fare Travels** partner card linking to `fairefaretravels.github.io/agent-sanecamack/`
- A full-screen hero powered by your broadcast video (`stvlogo.mpeg`)

---

## Files Required

Place all of these in the **same folder** before publishing:

| File | Purpose |
|---|---|
| `the-static-hub.html` | The site itself |
| `stvlogo.mpeg` | Hero background video |
| `mov-1.mp4` | Placeholder — Rick James Deep Cuts card |
| `mov-2.mp4` | Placeholder — DJ Mackinthedark card |
| `mov-3.mp4` | Placeholder — Tony Green / Vinyl Fest featured card |

Replace placeholder videos with real photos or clips as issues are published.

---

## How to Add a New Issue Card

Open `the-static-hub.html` and find the comment block:

```html
<!-- PLACEHOLDER: Add more cards below this line -->
```

Copy this block and paste it just above that comment:

```html
<article class="issue-card visible" data-month="mon-yyyy">
  <video autoplay muted loop playsinline>
    <source src="your-video-or-photo.mp4" type="video/mp4">
  </video>
  <!-- OR use an image instead: -->
  <!-- <img src="your-photo.jpg" alt="Description"> -->
  <div class="card-overlay">
    <span class="card-tag">Section · Month Year</span>
    <h3 class="card-title">Your Headline Here</h3>
    <p class="card-highlight">One or two sentences about the story. Keep it tight and punchy.</p>
    <p class="card-meta">Location · Date · Type</p>
  </div>
  <a href="https://your-link-here.com" target="_blank" class="card-read">Read →</a>
</article>
```

**To make a card span the full width** (featured/cover story), change the class to:

```html
<article class="issue-card featured visible" data-month="mon-yyyy">
```

---

## How to Add a New Month Tab

Find the `<div class="month-tabs">` section and add a button:

```html
<button class="tab-btn" data-month="jul-2026">Jul 2026</button>
```

The `data-month` value must match exactly what you put in the card's `data-month` attribute.

---

## Dedicated Player — B2B Section

The "For Organizations" section links to:  
`https://fairefaretravels.github.io/stvradiomeltdown-players/`

This pitches churches and luxury brands on a private, branded audio player separate from social media. Update the link if the player page URL changes.

---

## Publishing to GitHub Pages

1. Create a new repo (e.g. `stvradiomeltdown-static`)
2. Drop all files into the root of the repo
3. Go to **Settings → Pages → Source → main branch / root**
4. Your site will be live at `https://yourusername.github.io/stvradiomeltdown-static/`

---

## Links Referenced

| Destination | URL |
|---|---|
| STV Radiomeltdown | https://radiomeltdown.com |
| Dedicated Players | https://fairefaretravels.github.io/stvradiomeltdown-players/ |
| Faire Fare Travels | https://fairefaretravels.github.io/agent-sanecamack/ |
| Contact / Booking | https://formspree.io/f/mrbkljze |
| Kick Live Stream | https://kick.com/STVNETWORK |
| Phone | 678-433-8772 |

---

## Built By

STV Radiomeltdown · G4E Movement Studio  
Lithonia, GA · EST. MOVEMENT  
*Culture-driven. Community-built. Always live.*
