# Project Reflection — Nexora Bootstrap 5 Website

_A personal reflection on how I planned and built this project._

---

## 1. Project Planning

Before writing any code, I spent time thinking about what the site needed to be. The brief asked for a modern startup/business theme, so I chose a **software company** called Nexora — it gave me plenty of realistic content to work with (services, a team, testimonials, and so on) without being generic.

I sketched a rough plan on paper first:

- Decide on three pages: Home, About, and Contact.
- List the sections each page needed.
- Pick a small, consistent color palette (indigo primary, a soft grey background, and a dark footer).
- Choose fonts — I went with Plus Jakarta Sans for headings and Inter for body text because they pair nicely and feel modern.

Having this plan up front made the actual build much smoother, because I wasn't inventing the structure as I went.

---

## 2. Bootstrap Components Explored

I wanted to use a good range of Bootstrap 5 components rather than just the grid. In the end I worked with:

- **Navbar** with a collapsible toggler and a CTA button.
- **Grid system** for every layout — this did most of the responsive heavy lifting.
- **Cards** for features, services, testimonials, the team, and the "why choose us" section.
- **Accordion** for the FAQ sections.
- **Forms and validation** on the contact page.
- **Progress bars** for the skills section.
- **Badges, alerts, and buttons** in various places.
- A large number of **utility classes** for spacing, flexbox, and typography.

Exploring the utilities was probably the most useful part — I realized how much I could style with classes alone before reaching for custom CSS.

---

## 3. How the Pages Were Designed

I designed the **Home page** to tell a story from top to bottom: grab attention with the hero, build trust with features and stats, explain what we do with services, add social proof with testimonials, answer doubts with the FAQ, and finish with a call to action.

The **About page** was about personality — the company story, mission and vision, a timeline of milestones (which I built with custom CSS), the team, and a skills section with progress bars.

The **Contact page** focused on making it easy to get in touch. I put the validated form front and center, with company info cards, a map placeholder, and social links alongside it.

To keep everything feeling like one product, I reused the same navbar, footer, card styles, section headings, and spacing rhythm across all three pages.

---

## 4. Challenges Faced

A few things slowed me down:

- **Keeping the design consistent** across three pages without copying and pasting messy code.
- **Custom components** like the timeline and the stats band, which Bootstrap doesn't provide out of the box.
- **Form validation** — getting the Bootstrap validation styles to trigger correctly and showing a success message.
- **Responsiveness** — a couple of sections looked cramped on tablets and needed adjusting.
- **Images** — I wanted illustrations but didn't want to rely on random external files.

---

## 5. How They Were Solved

- For **consistency**, I created a set of shared CSS classes (cards, section headings, icon badges) and used CSS variables for colors and shadows, so a single change updates the whole site.
- For the **timeline and stats**, I wrote small, focused pieces of custom CSS on top of the Bootstrap grid rather than fighting the framework.
- For **form validation**, I used the standard Bootstrap `needs-validation` pattern with a tiny inline script, and added a success alert that appears once the form is valid.
- For **responsiveness**, I tested at common breakpoints and added a small `@media` section at the bottom of my stylesheet to fine-tune padding and font sizes.
- For **images**, I created my own lightweight **SVG illustrations and avatars** so the project has zero external image dependencies and still looks polished.

---

## 6. Bootstrap Documentation Used

I leaned on the official Bootstrap 5 docs throughout, especially the pages on:

- Navbar
- Grid and layout
- Cards
- Forms and validation
- Accordion
- Progress bars
- Utilities (spacing, flex, colors, shadows)

The utilities reference in particular became something I kept open in a browser tab the whole time.

---

## 7. AI Assistance Used Responsibly

I used an AI assistant as a helper — to explain Bootstrap concepts I was unsure about, suggest a sensible section order, and review my markup for cleaner ways to do things. I made sure to understand every piece of code before including it, rather than pasting things blindly. The design decisions, content, and overall structure are my own, and I treated the AI like a knowledgeable tutor rather than a shortcut.

---

## 8. Approximate Time Taken

All in, the project took me around **8–10 hours**, roughly broken down as:

- Planning and choosing the theme — ~1 hour
- Building the Home page — ~3 hours
- Building the About and Contact pages — ~3 hours
- Custom CSS, images, and polish — ~2 hours
- Testing responsiveness and writing the docs — ~1 hour

---

## Final Thoughts

This was a really satisfying project. I came away much more comfortable with the Bootstrap grid and utilities, and more confident about layering custom CSS on top of a framework without making a mess. If I revisited it, I'd like to add a light/dark theme toggle and some scroll-based animations — but I'm happy with how clean and consistent the current result feels.
