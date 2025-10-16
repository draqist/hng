
======================================================================
README – Accessible Profile Card (HTML + Tailwind CSS)
======================================================================

📘 OVERVIEW
------------
This HTML file implements a fully accessible, responsive, and aesthetically 
pleasing **Profile Card** built with **Tailwind CSS**. It uses semantic HTML, 
keyboard-accessible navigation, and WCAG-compliant contrast levels. The layout 
is inspired by the design principles of modern component libraries like Shadcn/UI.

The profile card displays:
- Avatar
- Name and dynamic time (auto-updating every 100 ms)
- Short biography
- Social media links (GitHub, LinkedIn)
- Two lists: Hobbies and Dislikes

🧩 KEY FEATURES
---------------
✅ 100% standalone — no build tools or frameworks required  
✅ Responsive design (mobile → desktop)  
✅ Live timestamp in milliseconds (`Date.now()`) auto-refreshing  
✅ Accessible focus styles for keyboard users  
✅ SVG icons (no external icon fonts)  
✅ Semantic markup with ARIA labels and test-friendly `data-testid` attributes  
✅ Graceful fallback for avatar load errors  

🎨 DESIGN NOTES
---------------
- Uses **Tailwind CSS** via CDN (`https://cdn.tailwindcss.com`)
- Defines a few custom CSS variables:
  --primary: accent color
  --primary-light: focus/hover color
  --text-color: base text color
- Rounded corners, subtle shadows, and balanced whitespace
- “Connect” section contains external links with smooth hover transitions

⚙️ HOW IT WORKS
---------------
1. The `<script>` at the bottom updates the `Current Time (ms)` display.
2. The function `updateTime()` runs immediately, then every 100 ms.
3. The base64ToArrayBuffer() helper is included (for potential extensions)
   but unused in this simple card.
4. The avatar `<img>` has an inline `onerror` fallback to a placeholder
   in case the primary image fails to load.

🧭 ACCESSIBILITY
----------------
- Every link, image, and heading has descriptive text or `aria-label`.
- Keyboard users get visible focus outlines (`outline: 3px solid var(--primary-light)`).
- Lists use custom bullet indicators, not images, for screen-reader clarity.
- High-contrast text ensures readability (meets WCAG AA).

🧑‍💻 TESTABILITY
----------------
Each important element is tagged with `data-testid` attributes for automated
testing (e.g., Playwright, Cypress, or Jest DOM).

🪄 CUSTOMIZATION
----------------
To personalize this card:
- Replace the avatar URL in `<img src="...">`
- Change user name, bio, hobbies, dislikes, and social links
- Update color palette by editing `:root { --primary: ... }` in `<style>`

🚀 DEPLOYMENT
--------------
This file runs entirely client-side — it can be hosted:
- On any static web server (GitHub Pages, Netlify, etc.)
- Directly from a local file (double-click to open)

Author: Abdullah Abdulfatah (Draq The Beast)

======================================================================
END OF README
======================================================================

