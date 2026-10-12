# Meal Master

Home-cooked Sri Lankan tiffin delivery around Kandy — Thennekumbura,
Mahawatta, Menikhinna and Kengalla mark the outer edge of the route.

Live site: https://meal-master.github.io/

## What this is

One static HTML file. No build step, no framework, no server, no database.
Open `index.html` in a browser and it works, online or offline.

## Editing

Everything is in `index.html`:

- **WhatsApp number** — the `PHONE` and `PHONE_PRETTY` lines near the top of
  the `<script>` block at the bottom. `PHONE` is digits only with the country
  code and no `+`, e.g. `94771234567`. Until it's set, the order form writes
  the message and lets the customer copy it, but has no number to open.
- **Bank details** — the `[ bank ]`, `[ branch ]` and `[ account number ]`
  placeholders in the "Paying" section.
- **Prices and menu** — plain text in the "Plans" and "This week" sections.
- **Draft banner** — the `<div class="draft">` block at the top of `<body>`.
  Delete it once the real details are in.

## Publishing a change

    git add -A
    git commit -m "Update menu"
    git push

GitHub Pages redeploys within a minute or two.
