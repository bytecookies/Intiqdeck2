# INTIQ Brand Deck

A 15-slide animated presentation that invites intimate apparel brands to join INTIQ, the rewards programme by Peppermint Communications. It is a plain static website: HTML, CSS and JavaScript, with no build step.

## Run it on your computer

Open `index.html` in Chrome, or serve the folder:

```bash
npx serve .
```

## Deploy on Vercel

1. Push this folder to a new GitHub repository.
2. In Vercel, choose **Add New → Project** and import the repository.
3. Set **Framework Preset** to **Other**. Leave Build Command and Output Directory empty.
4. Click **Deploy**.

Or from a terminal: `npx vercel` (preview) and `npx vercel --prod` (live).

## Presenting

| Key | Action |
| --- | --- |
| → / Space / Page Down / clicker | Next build, then next slide |
| ← / Page Up | Previous build or slide |
| F | Full screen |
| N | Speaker notes |
| Home / End | First / last slide |

You can also click (right side for next, left third for back) or swipe on a phone. Link straight to a slide with `#s5`, `#s10` and so on.

## Making changes

| What | Where |
| --- | --- |
| Slide text and speaker notes | `index.html` (each slide is a `<section>`; notes are in `data-notes`) |
| Photos | `assets/js/photos.js` |
| Colours, fonts, layout | `assets/css/deck.css` |
| Navigation and animation logic | `assets/js/deck.js` |

### Replacing a photo

1. Put your image in `assets/photos/`, for example `buy-and-fly-2006.jpg` (landscape, at least 1600px wide).
2. In `assets/js/photos.js`, change that photo's `src` to `"assets/photos/buy-and-fly-2006.jpg"`.

If a photo can't load, its frame shows the satin fabric, so a slide never looks broken.

## Slides

Slides marked (builds) reveal one part per click.

1. Cover
2. Keeping retailers active is hard
3. Every scheme is a heavy operations load (builds)
4. What we have built: INTIMASIA, SOURCE NXT, INTICEDE BSD (builds)
5. Buy & Fly: we have done this before
6. Introducing INTIQ
7. We take this load off you (builds)
8. Your scheme vs INTIQ (builds)
9. Our team does the work on ground
10. Rewards: one wallet, five steps (builds)
11. 15+ cities in Maharashtra and Gujarat
12. The numbers (builds)
13. The programme (builds)
14. From 2 states to all of India: MP, Delhi NCR, UP, Karnataka, then all India (builds)
15. Let's grow together

## Adding the logo

Put `intiq-logo.svg` or `intiq-logo.png` in `assets/brand/`. See `assets/brand/README.md`.

## Confirm before presenting

- Five reward steps and destinations (marked "Indicative" on slide 10)
- Commercial figures on slide 12 (marked "Proposed")
- Programme dates and targets on slides 13 and 14
- Venture names on slide 4

See `CREDITS.md` for data sources and photo licences.
