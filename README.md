# Maro Minds — Your Mind's Favourite Helping Hand

A responsive, single-page tutoring website for **Maro Minds**, a South African online tutoring service offering academic support for Grades 1–12.

---

## Overview

Maro Minds connects learners with experienced tutors across a wide range of subjects, aligned to both the CAPS and IEB curricula. The site allows prospective students and parents to explore subjects, view pricing, and submit a booking request — all from one page.

---

## Features

- **Responsive design** — fully optimised for desktop and mobile
- **Animated UI** — floating logo, slide-in hero text, and fade-in cards
- **Subjects section** — displays all offered subjects in a clean card grid
- **Pricing section** — three package tiers (Single, Monthly, Group) with a highlighted "Most Popular" card
- **Booking form** — collects learner details, subject selection, package choice, and availability; sends submissions via EmailJS
- **Confirmation modal** — displays a summary of the booking request on successful submission
- **Contact section** — phone and email links for direct enquiries

---

## Tech Stack

- **HTML5 / CSS3 / Vanilla JavaScript** — no frameworks required
- **[Google Fonts — Montserrat](https://fonts.google.com/specimen/Montserrat)** — typography
- **[EmailJS](https://www.emailjs.com/)** — client-side email delivery for the booking form (no backend required)

---

## Project Structure

```
index.html        # Single-file application — all HTML, CSS, and JS included
```

---

## Getting Started

Since this is a static single-page site, no build step is needed.

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/maro-minds.git
   cd maro-minds
   ```

2. **Open locally**
   ```bash
   open index.html
   ```
   Or simply drag `index.html` into your browser.

3. **Deploy** — upload `index.html` to any static host (GitHub Pages, Netlify, Vercel, etc.).

---

## EmailJS Configuration

The booking form uses [EmailJS](https://www.emailjs.com/) to send submissions without a backend.

To use your own EmailJS account:

1. Sign up at [emailjs.com](https://www.emailjs.com/) and create a service and email template.
2. In `index.html`, replace the following values with your own:

```js
emailjs.init('YOUR_PUBLIC_KEY');

emailjs.send('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', templateParams)
```

### Expected template variables

| Variable | Description |
|---|---|
| `from_name` | Learner's full name |
| `from_email` | Learner/parent email |
| `phone` | Contact phone number |
| `grade` | School grade |
| `subject` | Subject(s) selected |
| `package` | Chosen pricing package |
| `lesson_count` | Number of lessons (single-session bookings) |
| `availability` | Preferred session times |
| `additional_info` | Any extra notes |

---

## Pricing

| Package | Duration | Price |
|---|---|---|
| Single Lesson | 1 hour | R200 |
| Single Lesson | 1.5 hours | R300 |
| Monthly (2× per week) | 1 hour | R1,600 |
| Monthly (2× per week) | 1.5 hours | R2,400 |
| Group | 1 hour | R150 per learner |
| Group | 1.5 hours | R200 per learner |

---

## Subjects Offered

English HL · Afrikaans FAL · Mathematics · Accounting · Business Studies · Economics · Life Sciences · Physics · Computer Applications Technology (CAT) · NBT Preparation · Study Skills · Academic Coaching

---

## Contact

| | |
|---|---|
| 📞 Phone | [066 125 4466](tel:0661254466) |
| ✉️ Email | [marominds@gmail.com](mailto:marominds@gmail.com) |

---

## License

© 2026 Maro Minds. All rights reserved.
