# HypeCheck — Context for the Marketing Website

> Portable brief for building HypeCheck's landing/marketing site in a separate
> repo. Self-contained: everything a designer, copywriter, or AI agent needs to
> build the site without access to the app source. Values here are pulled from
> the live app so the site matches the product exactly.

---

## 1. What HypeCheck is (one-liner)

**HypeCheck turns social shopping hype into a clear buy, wait, or skip decision.**

You paste a product link or name (the kind of thing that blows up on TikTok,
Instagram, or Amazon), and HypeCheck returns an honest verdict on whether it's
actually worth buying — before you waste money on a viral dud.

- **Platform:** iOS app (App Store). Built with Flutter.
- **Category:** Shopping / utility / personal finance.
- **Status:** Launching with a subscription (hard paywall after onboarding).
- **App version:** 2.1.x.

## 2. Who it's for

People who buy things they see go viral online and later regret it — impulse-prone
social shoppers who want a quick gut-check before checkout. The emotional hook is
**money wasted on hype** ("the hype tax").

## 3. The story (positioning narrative)

- **Problem:** Viral products are engineered to look amazing. Paid creators, fake
  reviews, and inflated prices make it impossible to tell a genuinely good buy
  from an overhyped flop. People keep getting burned.
- **Insight:** Most shoppers buy the hype. The cost adds up to hundreds of dollars
  a year in regretted purchases and overpaying.
- **Solution:** HypeCheck reads the real signal — proof vs. hype, fair price,
  genuine complaints — and gives a fast Buy / Wait / Skip call so you keep your
  money for things actually worth it.
- **Payoff:** "Keep what you save."

Approved headlines from the app (safe to reuse on the site):
- "Stop paying for the hype."
- "Most shoppers buy the hype. You won't."
- "Here's how HypeCheck has your back."
- "Keep what you save."

## 4. Core features (what to show on the site)

| Feature | Plain-English benefit |
|---|---|
| Hype check on any product link | Paste a TikTok / Instagram / Amazon link or product name |
| Buy · Wait · Skip verdict | One clear call in seconds — no research rabbit hole |
| Proof score & hype risk | How much real evidence backs the product vs. manufactured buzz |
| Fair-price check | Whether the asking price is fair, plus cheaper alternatives |
| Fake-hype & creator-bias detection | Flags paid-creator patterns and suspect reviews |
| Scan history | Your past checks, saved on-device |

> **Honesty constraint:** don't over-claim accuracy or invent statistics. The app
> deliberately avoids fabricated numbers. Keep marketing claims directional
> ("helps you avoid overhyped buys"), not absolute ("saves you $X guaranteed").

## 5. How it works (3-step section)

1. **Paste** a product link or name.
2. **HypeCheck analyzes** the proof, the price, and the complaints.
3. **Get a verdict** — Buy, Wait, or Skip — and what to do next.

## 6. Pricing

Hard paywall — full app unlocked by an active subscription. Two plans shown
(an A/B test runs weekly-vs-monthly as the short-term option):

| Plan | Price | Notes |
|---|---|---|
| Weekly | $4.99 / week | short-term option (A/B arm) |
| Monthly | $9.99 / month | short-term option (A/B arm) |
| **Yearly** | **$39.99 / year** | **3-day free trial**, best value, default-selected |

Renewal terms line: "Auto-renews until cancelled. Cancel anytime."

## 7. Brand kit

**Logo:** a rounded-square "price tag" in green with a white checkmark. (In the
app it's drawn in code; the site will need an exported SVG/PNG — see Assets.)

**Color palette (exact hex from the app):**

| Token | Hex | Use |
|---|---|---|
| Ink | `#0E1117` | primary text, dark buttons |
| Paper | `#F7F6F1` | warm off-white background |
| Surface | `#FFFFFF` | cards |
| Mint (primary) | `#16A57A` | brand green, positive/"Buy", accents |
| Coral | `#E86F51` | warnings / "Skip" / the hype-tax red |
| Gold | `#E1A11B` | ratings / highlights |
| Blue | `#3C78D8` | secondary accent |
| Line | `#E4E2D9` | borders / dividers |

Brandmark gradients: green tag `#3BE0A4 → #0C8A62`, dark variant `#1B212B → #0A0D12`,
checkmark `#076E51`.

**Typography:** Inter (Google Fonts). Headlines are heavy (700–800 weight),
tight, sentence-case with hard line breaks for punch. Body is medium weight,
slightly muted ink.

**Verdict color language:** Buy = mint/green, Wait = gold, Skip = coral/red.

**Tone of voice:** punchy, money-smart, a little cheeky, anti-hype. Short
sentences. Talks to the reader directly ("you"). Never preachy about their
spending — the enemy is the hype, not the shopper.

## 8. Suggested site sections

1. **Hero** — headline ("Stop paying for the hype."), subhead, App Store badge, phone mockup.
2. **How it works** — the 3 steps above.
3. **Features** — the table in §4 as cards with the verdict color language.
4. **The hype tax** — the money-wasted angle; emotional payoff "Keep what you save."
5. **Pricing** — plans from §6 with the trial called out; mirror the in-app paywall.
6. **Social proof** — reviews/ratings once available (don't fabricate).
7. **FAQ** — what it analyzes, is it accurate, how to cancel, privacy.
8. **Footer** — Privacy Policy, Terms (Apple Standard EULA), support email, App Store link.

## 9. Links & legal

- **App Store URL:** _TBD — add once live._
- **Privacy Policy:** self-hosted page (source content exists at `docs/privacy-policy.html` in the app repo). _TBD final URL._
- **Terms of Use:** Apple Standard EULA — `https://www.apple.com/legal/internet-services/itunes/dev/stdeula/`
- **Support / contact email:** egamovhamid@gmail.com
- **Bundle ID (reference):** `com.summerapps.hypecheck`

## 10. Assets needed (not in this file)

- Logo exported as SVG + PNG (light + dark) — currently only drawn in app code.
- App screenshots (home, a verdict/detail screen, the savings/"hype tax" screen, the paywall).
- App Store badge + device mockups.

> If you want these generated, ask the app repo: the logo can be exported from the
> `drawBrandMark` painter, and screenshots captured from the iOS Simulator.
