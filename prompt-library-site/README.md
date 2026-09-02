# Ashmont Prompt Library

Companion web page for **Medical AI in Practice: Prompting, Protocols, and Clinical
Implementation Standards** (Ashmont Research Publications, Second Edition).

Every chapter of the book carries a PROMPT LAB block with a QR code. Those QR codes
point at this page, one anchor per chapter (`#ch-1` ... `#ch-36`). The page serves each
prompt in three platform-tailored variants (ChatGPT, Gemini, Claude) with copy buttons.

## Important

The QR codes are printed permanently in the book. This site must stay reachable at
**https://ashmont-prompt-library.vercel.app** and the anchors `#ch-1` through `#ch-36`
must not be renamed, or the printed codes stop working.

## Deploying

Static site, no build step.

1. Push these files to a GitHub repository named `ashmont-prompt-library`.
2. In Vercel: **Add New -> Project -> Import** that repository.
3. Framework preset: **Other**. Build command: none. Output directory: leave empty (root).
4. Deploy. The production URL becomes `https://ashmont-prompt-library.vercel.app`.
5. Check that Settings -> Deployment Protection -> Vercel Authentication is **off**, so
   readers can open the page without a Vercel account.

## Files

- `index.html` - the page (styles and logic inline, no build step, no dependencies)
- `d1.js` - prompt data, chapters 1-18
- `d2.js` - prompt data, chapters 19-36

To correct a prompt later, edit the relevant entry in `d1.js` or `d2.js` and push. The URL
and anchors stay the same, so already-printed QR codes keep working.
