# Miles Lab website

Source for the Miles Lab website, built with [Quarto](https://quarto.org) and published to GitHub Pages.

## Put it online (one time)

1. Create a new **public** repository on GitHub (for example `miles-lab`).
2. Upload everything in this folder, including the hidden `.github` folder. Either:
   - drag the files into the repo's "Add file → Upload files" page, or
   - from a terminal in this folder:
     ```
     git init -b main
     git add .
     git commit -m "Initial lab site"
     git remote add origin https://github.com/YOUR-USERNAME/miles-lab.git
     git push -u origin main
     ```
3. In the repo, go to **Settings → Pages** and set **Source** to **GitHub Actions**.
4. Open the **Actions** tab. The "Publish site" workflow builds the site in about two minutes.
   Your site will be at `https://YOUR-USERNAME.github.io/miles-lab/`.
5. Put that URL in `_quarto.yml` (`site-url`) and link it from your Purdue profile.

After that, every change you push to `main` republishes the site automatically.
You can even edit files directly on github.com.

## Preview on your own computer (optional)

Install Quarto, then run `quarto preview` in this folder. It opens the site and refreshes as you edit.

## Where things live

| To change...            | Edit                                         |
|-------------------------|----------------------------------------------|
| Menu, links, footer     | `_quarto.yml`                                |
| Colors and fonts        | `styles.scss`                                |
| Home page               | `index.qmd`                                  |
| Research themes         | `research.qmd`                               |
| Your bio                | `people/miles.qmd`                           |
| Add a lab member        | copy `people/_template.qmd`, add photo to `images/people/` |
| Publications            | paste BibTeX into `publications.bib`         |
| Add a news post         | copy a folder in `news/posts/`               |
| Join, Resources, Contact| `join.qmd`, `resources.qmd`, `contact.qmd`   |

## Placeholders to fill in

Search the project for `TODO` and `[` brackets. The main ones:

- Your GitHub username (`_quarto.yml`)
- Purdue profile, ORCID, Google Scholar links
- Department, office, lab room, and email (`contact.qmd`, `join.qmd`)
- Graduate programs you advise through (`join.qmd`)
- Your headshot (`images/people/`) and CV
- Real publications (`publications.bib`)
- Photos for the research themes
