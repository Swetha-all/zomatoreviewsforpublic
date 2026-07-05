# Zomato Feedback Analyzer

AI-assisted product research project — analyzing user reviews to identify pain points and prioritize fixes, the way a PM would before writing a roadmap.

## Problem

Zomato has millions of users leaving reviews on the Play Store, but raw reviews aren't actionable on their own. This project turns unstructured user feedback into a structured, prioritized list of product issues.

## Methodology

1. Collected 25 user reviews (mix of 1★–5★) covering delivery, support, payments, and UX
2. Used Claude to categorize each review into themes and count mentions
3. Prioritized themes by frequency and severity
4. Wrote an executive summary with a recommended Q1 fix order

## Files

| File | Contents |
|---|---|
| `reviews.txt` | Raw sample reviews used for analysis |
| `theme_analysis.txt` | Reviews grouped into themes, with pain points, fixes, and priority |
| `summary.txt` | Executive summary with recommended Q1 priority order |

## Key Findings

| Theme | Mentions | Priority |
|---|---|---|
| Customer Support | 9 | High |
| Delivery & Logistics | 6 | High |
| Payments & Refunds | 5 | High |
| Order Accuracy | 4 | High |
| UI/UX | 3 | Medium |
| Pricing | 1 | Low |

**Top insight:** Customer support isn't just the most-mentioned issue — it's the root cause that turns every other problem (bad delivery, wrong order, refund delay) into a bad *experience*, because tickets get closed without actual resolution.

## Recommended Priority Order

1. Support resolution SLA + human escalation trigger
2. Photo/OTP proof-of-drop for delivery
3. Auto-refund SLA for cancelled/unconfirmed orders
4. Packer-side photo verification for order accuracy

---

*Built using Claude for review categorization and prioritization.*
