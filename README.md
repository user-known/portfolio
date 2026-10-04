# Portfolio

Personal portfolio for Vignesh Balakumar. Plain HTML, CSS and JS. No build step.

## Pages
- `index.html` home
- `about.html` about
- `projects.html` all projects (filterable)
- `case-study.html` the case study template. It renders any project from `projects-data.js`
- `admin.html` add and edit projects (not linked from the site)
- `projects-data.js` the project list. The home page, projects page and hero card all read this one file.

## Adding a project
1. Open `admin.html` (on the live site, or from the folder in a browser).
2. Click **New**, fill in the fields, tick the categories, and tick "Show on the home page" if it belongs in Selected work.
3. Either **Download file** and replace `projects-data.js` in the repo, or open "Publish straight to GitHub", enter owner, repository and a fine-grained token (Contents: Read and write, one repository only), and click **Publish**.
4. GitHub Pages updates in a minute or two.

Your edits are saved as a draft in your browser until you publish or discard them.

## Case study pages
There is one template, `case-study.html`. It builds each project's page from `projects-data.js`, so you never copy it.
- In the admin, open a project, switch to the **Case study page** tab and tick "Show a case study page".
- Fill in only the sections you need (header, overview quote and image tabs, brief, process diagram, challenge, research numbers and questions, insights, identity, website slides, campaign images, outcomes). A section with nothing in it is left out of the page and the side menu.
- The project's card then links to `case-study.html?p=<page name>` automatically. Use **Preview page** to see your unpublished draft in a new tab.
- A project with no case study page shows a card with no link. The "Custom link" field on the Project card tab overrides the built-in page (for example to point at an external site).

## Images
Put images in an `images/` folder and enter the path (for example `images/acme.jpg`) as the cover image, or use **Upload image** in the admin with GitHub connected. Without an image the card uses its gradient cover.

## Before publishing
- Replace `hello@yourdomain.com` (the `EMAIL` line in each page's script, plus the visible text and `mailto:` links).
- Replace the `#` links for LinkedIn and Behance.
- Replace the "Add..." placeholder text in `projects-data.js` and the pages.
- If you don't want the admin page public, leave `admin.html` out of the repo and open it locally from the folder instead.
- General Sans is loaded from Fontshare. Check its license for your use.

## Hosting on GitHub Pages
Settings > Pages > Deploy from a branch > `main` / root. The site appears at
`https://<username>.github.io/<repo>/`.
