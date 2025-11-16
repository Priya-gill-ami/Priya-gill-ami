
<!--
  Lavender & Black theme — using color names (Lavender, Black, Thistle) instead of hex codes.
  Banner is an inline SVG so it renders on GitHub.
-->

## <img alt="Lavender & Black banner" src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='1200' height='220'><rect width='1200' height='220' fill='black'/><rect x='24' y='24' width='1152' height='172' rx='14' fill='lavender' opacity='0.12'/><text x='60' y='108' font-size='38' fill='lavender' font-family='Segoe UI, Arial, sans-serif'>Priya Gill — Always learning, always building</text><text x='60' y='150' font-size='16' fill='thistle'>One commit at a time • Lavender & Black profile</text></svg>" />

# Hi there 👋

Welcome! I updated this README with a professional layout inspired by your LinkedIn profile and common elements that professionals add to GitHub profiles. Colors in the header and accents use named colors (Lavender, Black, Thistle) to match your request.

---

## Professional Snapshot

- Current role: Head of Global Marketing, SurveyMonkey — growth-oriented marketing leader with a cross-functional background across product, engineering, and marketing.
- Location: San Francisco Bay Area
- Summary: Seasoned marketing executive with experience in product-led growth, team leadership, and data-driven strategy. Comfortable bridging technical and GTM teams to drive measurable outcomes.
- Education: MBA — UCLA Anderson School of Management; B.S. Computer Engineering — UC Irvine

---

## Skills & Tools

- Product Marketing • Growth Strategy • Go-to-Market
- Cross-functional Leadership • Team Building • Mentorship
- Product Management • Program Management • Systems Engineering
- Data-driven Decision Making • Analytics • A/B Testing
- Tools: Git • GitHub • Google Analytics • Mixpanel • Figma • Notion • Slack • JIRA

---

## Professional Links & Badges

- LinkedIn: https://www.linkedin.com/in/priyagill07/
- Email: (add your preferred contact email)
- Resume: (link to your resume or Google Drive)

Badges (examples you can copy):
- ![LinkedIn](https://img.shields.io/badge/LinkedIn-Priya%20Gill-lavender)
- ![Available to collaborate](https://img.shields.io/badge/Status-Open%20to%20Collaboration-thistle)
- ![Top languages](https://img.shields.io/badge/Top%20Languages-JavaScript%20%7C%20TypeScript-lavender)

(Shields badges accept color names — adjust text and links to suit.)

---

## Featured Projects

### Random Joke Generator
A small, friendly project that demonstrates fetching from an external API and rendering results in a minimal UI. Great for showcasing async fetch, error handling, and simple frontend design.

Node example:
```js
// Node 18+ or with a fetch polyfill
async function getRandomJoke() {
  try {
    const res = await fetch('https://v2.jokeapi.dev/joke/Any?type=single');
    if (!res.ok) throw new Error(`HTTP ${res.status}`);
    const data = await res.json();
    return data.joke || `${data.setup} — ${data.delivery}`;
  } catch (err) {
    console.error('Failed to fetch a joke:', err);
    return 'No jokes available right now. Try again later!';
  }
}

getRandomJoke().then(joke => console.log('Joke:', joke));
```

Browser (vanilla) example:
```html
<button id="jokeBtn">Tell me a joke</button>
<p id="jokeText"></p>
<script>
document.getElementById('jokeBtn').addEventListener('click', async () => {
  const p = document.getElementById('jokeText');
  p.textContent = 'Loading...';
  try {
    const res = await fetch('https://v2.jokeapi.dev/joke/Any?type=single');
    const data = await res.json();
    p.textContent = data.joke || `${data.setup} — ${data.delivery}`;
  } catch {
    p.textContent = 'Could not fetch a joke right now.';
  }
});
</script>
```

---

## What professionals commonly include (added here)

- Clear "Current role" + short summary (done above)
- Skills / Tools section (done above)
- Pinned or featured projects (Random Joke Generator + add others)
- Links: LinkedIn, personal website/portfolio, resume, email
- Contribution / collaboration status (Open to collaboration / Mentorship / Speaking)
- Badges: repo stats, top languages, social links
- How to contact or contribute: simple CONTRIBUTING guide or "How to run this project" sample
- Optional: blog posts, talks, certificates, publications

---

## Open to
- Mentorship and advising early-stage product/marketing teams
- Collaboration on product-led growth experiments, developer tooling, and small web UI projects
- Speaking on growth, product-marketing alignment, and building cross-functional teams

---

## Contact & Next Steps

- GitHub: @priya-gill-ami
- LinkedIn: https://www.linkedin.com/in/priyagill07/
- Email: (please add)

If you'd like, I can:
- Create a small demo folder (static HTML + one JS file) for the Random Joke Generator and a README-runner script.
- Add dynamic GitHub stats and language cards below the banner.
- Generate a CONTRIBUTING.md and simple issue / PR templates for community contributions.

---

Thank you — I drafted this README update to be ready to copy/paste into your repository. If you want, I can now create the demo project files (HTML/CSS/JS) with the Lavender & Black theme and show how to deploy them via GitHub Pages.
