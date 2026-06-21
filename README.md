# Supernova SMP website

A responsive, static website ready for GitHub Pages.

The site uses the transparent `supernova-logo.png` stored beside `index.html`. Keep every file in the ZIP together at the repository root; no nested asset folder is required for the live site.

The owner profile uses `kyluua-profile-v2.png`, also stored at the repository root. The versioned filename prevents an older profile image from being reused by browser or GitHub Pages caches. The copy button includes a compatibility fallback for browsers that cannot use the modern clipboard API.

## Domain security

The included `CNAME` file connects the Pages site to `supernovasmp.xyz`. In the domain's DNS settings, remove the incorrect A record `157.85.90.148`. Keep only GitHub Pages' four A records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, and `185.199.111.153`. After DNS updates, confirm the custom domain in GitHub **Settings → Pages** and enable **Enforce HTTPS** when it becomes available.

## Customize before publishing

Open `script.js` and update the Discord URL at the top:

- `discordUrl`

The Minecraft server address is already set to `supernovasmp.xyz`.

## Languages

The site includes English, German, Spanish, French, and Portuguese. It automatically uses a supported browser language and remembers each visitor's choice. All translations are stored in the `TRANSLATIONS` section of `script.js`, where more languages can be added later.

The separate `credits.html` page credits **kyluua** as the server owner and creator.

The `rules.html` page contains the server rules and community guidelines in all five supported languages.

## Publish with GitHub Pages

1. Copy all files in this folder into the root of your GitHub repository.
2. Commit and push the files.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, then choose your main branch and `/ (root)`.
5. Add `supernovasmp.xyz` under **Custom domain**.

For the custom domain, your DNS provider also needs the GitHub Pages records described in GitHub's documentation.
