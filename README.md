# Summer 2026 Manufacturing Roadshow Site

This is the site for ReImagine Appalachia and AMCC's Summer 2026 Manufacturing Roadshow. It's a static site — there's no backend, no CMS, and no database. The only outside service it talks to is Formspree, which handles the email signup form.

The site is live at https://reimagine-appalachia.github.io/amap-roadshow/

## What's in this repo

`index.html` is the homepage. It has an overview of all five stops and the email signup form.

`agenda.html` has the full schedule for each stop.

`speakers.html` lists all the speakers and lets you filter by which stop they're presenting at.

`resources.html` has descriptions of and links to all the partner organizations.

`about.html` covers the A-MAP background, the 10 pillars, and why people should attend.

`styles.css` holds all the styling for every page.

The `assets` folder has the logos, the hero background photo, and the downloadable one-pager PDF.

A few files in `assets` — `logo.png`, `img_0.jpeg`, `img_1.png`, `logo_preview_TEMP.png`, and `amcc_preview_TEMP.png` — are leftovers from earlier attempts at getting the logos right. They aren't referenced anywhere on the site, so they're safe to delete whenever someone gets around to it.

## How to make edits

The site is hosted on GitHub Pages and deploys automatically from the `main` branch. To change anything, open the file you want to edit in the repo, click the pencil icon in the top right to switch into edit mode, make your changes, and commit them. GitHub Pages will rebuild and publish the update within about a minute. If you don't see your change after refreshing, try opening the site in a private or incognito tab — browsers tend to cache CSS files aggressively, so what you're seeing might just be an old cached version rather than a failed update.

There's no build step and nothing else to configure. The URL never changes, since it's tied to the repository name rather than anything in the code.

## What still needs attention

A few resource links on `resources.html` are placeholders because the source materials didn't include real URLs for them when the site was built — specifically the AMCC slides and the AMCC newsletter signup. You can find these by searching `resources.html` for `class="link-btn pending"`.

The footer doesn't have a phone number. The original one-pager had a placeholder number (123-456-7890) that was obviously fake, so it was left off entirely. Add a real one if there's a number you want listed.

The virtual stop on September 8 and the closing summit don't have agendas or registration links yet. Both currently show "Registration Coming Soon" on the agenda page, and can be updated once those details are finalized.

## Data collected

The only data collected is an email address through the signup form, and it's opt-in. There are no accounts, no participant profiles, and nothing else tracked.
