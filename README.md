# What's Your Group Chat Role?

A 60-second quiz that tells you your role in the group chat. Plain HTML: no build step, no dependencies.

## Files

- `index.html`: the whole quiz
- `og.png`: the image that shows up when someone pastes the link in a chat or post (1200×630)
- `favicon.svg`: the browser tab icon
- `fonts/`: Bagel Fat One and Figtree, self-hosted (SIL Open Font License, see the license files)

## Put it online with GitHub Pages

1. Push this folder to a public repo named `group-chat-role`.
2. In the repo, go to **Settings → Pages**, set the source to **Deploy from a branch**, and pick `main` and `/ (root)`.
3. In about a minute it's live at `https://nothingbutnette.github.io/group-chat-role/`.

## If you use a different repo name or your own domain

The link preview needs the full address. In `index.html`, find and replace `https://nothingbutnette.github.io/group-chat-role/` with the new address (it appears in `og:url`, `og:image`, `twitter:image` and `canonical`).

For a custom domain, add it under **Settings → Pages → Custom domain**, then set the DNS records your domain registrar asks for.

## Checking the link preview

After it's live, paste the link into opengraph.xyz to see how it'll look in iMessage, Instagram and X. Apps cache previews, so if you change `og.png`, rename it (for example `og-2.png`) and update the tags.

## Editing roles and questions

Everything is in the `<script>` near the bottom of `index.html`:

- `T` holds the ten roles (name, tagline, description, best duo, rival).
- `Q` holds the ten questions. Each answer points to one role.
- `PALS` holds the color options.
