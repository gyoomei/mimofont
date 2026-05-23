# 🎨 MiMoFont
> AI Typography Critic & Font Pairing Advisor — powered by Xiaomi MiMo V2.5

🔗 [Live Demo](https://gyoomei.github.io/mimofont/) · 📂 [Repo](https://github.com/gyoomei/mimofont)

## What it does

Upload a screenshot or paste any website URL. MiMoFont detects every font in use, then Xiaomi MiMo V2.5 analyzes pairing harmony, readability, accessibility compliance, and suggests better alternatives — all in under 10 seconds.

```
You paste:    https://stripe.com
MiMo replies: Pairing: 92/100 · Readability: 88/100 · Accessibility: 85/100
              Recommended: Replace "Stripe Cursive" with "Inter Display" for headings
```

That's the entire UX. One input → instant typography intelligence.

## Features

| Capability | Detail |
|---|---|
| 🔗 URL Font Detection | Fetches page CSS, extracts @font-face, Google Fonts, inline font-family |
| 📸 Screenshot Analysis | AI vision identifies fonts from design mockups, websites, apps |
| ✏️ Manual Input | Type font names directly for quick pairing check |
| 📊 Score System | 0–100 for pairing harmony, readability, accessibility, overall |
| 🎨 Smart Alternatives | AI suggests replacements with reasoning |
| 🌐 Bilingual | English + Indonesian toggle |
| 🌓 Dark/Light | WCAG-AA compliant themes |
| 📱 Mobile Responsive | Works on 320px+ screens |

## How it works

```
┌──────────────┐     ┌──────────────┐     ┌──────────────┐
│  Input       │────▶│  Font        │────▶│  MiMo AI     │
│  URL/Screenshot│    │  Detection   │     │  Analysis    │
└──────────────┘     └──────────────┘     └──────┬───────┘
                                                  │
                                           ┌──────▼───────┐
                                           │  Score +     │
                                           │  Alternatives│
                                           └──────────────┘
```

## Try these examples

| Input | What you'll see |
|---|---|
| `https://stripe.com` | Clean sans-serif pairing, high scores |
| `https://nytimes.com` | Classic serif analysis, readability focus |
| `https://vercel.com` | Geist font family deep dive |
| Upload any Figma screenshot | AI identifies fonts visually |

## Stack

- **Frontend:** Single HTML, zero dependencies
- **AI Engine:** Xiaomi MiMo V2.5 via Pollinations.ai
- **Font Detection:** Client-side CSS parsing + Google Fonts API
- **Hosting:** GitHub Pages

## Why single HTML

- Zero build step, zero npm install
- Browser opens index.html directly
- Deploy in seconds — just git push
- No backend, no API key, no CORS issues

## Roadmap

- [ ] Font pairing playground (drag fonts, see live preview)
- [ ] Export analysis as PDF report
- [ ] Font licensing checker (free vs commercial)
- [ ] Historical trend tracking (monitor font changes over time)

## Run locally

```bash
git clone https://github.com/gyoomei/mimofont.git
cd mimofont
python3 -m http.server 8080
# Open http://localhost:8080
```

## License

MIT

**Built with 🧠 Xiaomi MiMo V2.5 · Submitted to MiMo 100T Creator Program**
