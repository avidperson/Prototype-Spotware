# cTrader Help Centre — Homepage Redesign Prototype

A self-contained, single-file (`index.html`) prototype redesigning the [cTrader Help Centre](https://help.ctrader.com/) homepage around user roles, single-screen discovery, AI-assisted search, and responsive navigation across all 17 live languages.

---

## Quick Start

- **Open locally:** Download [`index.html`](./index.html) and open it directly in any modern desktop or mobile browser. No build step, server, or external setup is required.
- **GitHub Pages (if enabled):** Visit the repository's GitHub Pages URL to interact with the live prototype directly in the browser.

---

## Key Improvements Over the Live Homepage

- **Single-Screen Search Stage:** Replaces the three large promotional banners that push documentation below the fold on live `help.ctrader.com` with a centered search bar and **Ask AI** assistant, **Try:** starter prompts on taller screens, a side-by-side hero header on shorter desktop and tablet screens, and a compact bottom promo strip (**Live Account | cTrader Store | Join Discord** on narrow and mobile views).
- **Organized Around Six User Audiences:** Replaces the duplicated 23-card **All sections** grid and unfiltered 10-card **Popular guides** list with one unified card pairing a **Sections / Popular Guides** switch and **View all** with six user groups:
  1. **Manual Traders** — *cTID, orders, charts & apps*
  2. **Copy Traders** — *Copy or provide strategies*
  3. **Algo Traders** — *cBots, indicators, MCP & CLI*
  4. **Developers** — *Open API, FIX API & plugins*
  5. **Store Sellers** — *Publish & sell on cTrader Store*
  6. **Partners & IBs** — *Partner tools, Invite & deeplinks*

  Selecting any tile opens **All Sections** (20 hubs) or **Popular Guides** (10 walkthroughs) pre-filtered for that role in a pop-up window or mobile sheet, while general **Resources** (*Knowledge base*, *cTrader bonuses*, *Troubleshooting*) remain in the left menu and search.
- **Main-Stage Search & Simulated Ask AI:** Elevates header keyword search into a focused spotlight experience featuring **AI Summary** cards with a verification note, one-click **Copy** code and deeplink examples, clickable **Sources** pills, **Follow up:** prompt chips, and **Matching Documentation** links. On phones, tapping search docks the bar cleanly above the on-screen keyboard and compacts **Ask AI** to a sparkle icon when typing space gets tight.
  > **Note on AI in this prototype:** Because `index.html` runs standalone without a backend server, **Ask AI** is simulated using 10 pre-written, source-checked answers (translated across all 17 languages) paired with instant search across 29 hubs and guides. On a live production site, this interface would connect to an AI service grounded in Spotware's official documentation.
- **Adaptive Left Navigation Across Four Screen Sizes:**
  - **Desktop (`> 960 px`):** Collapsible sidebar with **Home**, the six main groups (23 section links), single-open accordion behavior to prevent vertical jumping, a pinned **Need more help?** support card, and a curved side tab.
  - **Tablet (`561–960 px`):** Slide-out menu tucked off-screen until opened from the side tab, closing when tapping outside.
  - **Short Landscape (`width >= 561 px`, `height <= 460 px`):** Full-screen two-column menu opened from the header menu button, showing main groups on the left and section cards plus support on the right.
  - **Mobile (`<= 560 px`):** Clean centered **cTrader | Help Centre** header paired with three thumb-friendly bottom controls (**Toggle theme**, centered menu-to-close button, and circular flag button).
- **Light & Dark Theme Support:** Opens in light mode by default with dual-theme background chart artwork, badges, and cards (fixing the live homepage's dark-only banner graphics in light mode), plus an isolated **Toggle theme** button that switches themes without closing open menus, pop-ups, or search results.
- **17 Live Languages & Verified Links:** Localizes all interface text, pluralized item counts, and AI answers across all **17 live languages** (`en`, `es`, `pt`, `ar`, `id`, `ms`, `th`, `vi`, `ko`, `zh`, `ja`, `ru`, `tr`, `de`, `fr`, `it`, `pl`), including full right-to-left (**RTL**) layout mirroring for **Arabic**, a circular flag-only selector displaying language names in the active language, English-only link preservation for **cTrader Mobile**, and updated direct URLs for redirected or broken live links.

---

## Keyboard Shortcuts

| Shortcut | Action |
| :--- | :--- |
| `/` or `Ctrl+K` / `Cmd+K` | Focus the search bar |
| `[` | Collapse or expand the desktop left navigation sidebar |
| `Esc` | Close active search results, pop-up windows, or menus |

---

## Repository Structure

```text
.
├── index.html   # Complete single-file prototype (HTML, CSS, JS, search index & 17 locales)
└── README.md    # Project overview and usage notes
```
