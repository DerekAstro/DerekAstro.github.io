# DerekAstro.github.io starter site

This is a lightweight static site for the `DerekAstro.github.io` GitHub Pages repository. It uses plain HTML and CSS, so it does not need Jekyll, npm, Python, or a build step.

## Files

- `index.html` — the homepage content and links
- `styles.css` — all visual styling and responsive layout rules
- `README.md` — these notes

## Edit before publishing, if desired

Open `index.html` in a text editor and search for the sections you want to revise:

- Hero/title block
- About
- Research
- Teaching & mentoring
- Publications
- Contact

The page currently uses a monogram placeholder (`DB`) instead of a photo. To add a photo later, put an image file in the repository, then replace the `portrait-placeholder` block in `index.html` with an `<img>` tag.

## ADS link

The homepage includes this ADS query:

```text
https://ui.adsabs.harvard.edu/search/q=author%3A%22Buzasi%2C%20D%22&sort=date%20desc%2C%20bibcode%20desc&p_=0
```

If ADS splits publications across name variants, you can refine the query later by ORCID or by adding additional author forms.

## Upload with GitHub's web interface

1. Download and unzip this folder.
2. Go to `https://github.com/DerekAstro/DerekAstro.github.io` while signed in.
3. Click **Add file** → **Upload files**.
4. Drag the **contents** of this folder into the upload area. Make sure `index.html` and `styles.css` appear at the top level of the repository, not inside an extra nested folder.
5. Use a commit message such as `Add personal website`.
6. Choose **Commit directly to the main branch** and click **Commit changes**.
7. Visit `https://derekastro.github.io/` after GitHub Pages finishes publishing.

## Upload with git from a terminal

```bash
git clone https://github.com/DerekAstro/DerekAstro.github.io.git
cd DerekAstro.github.io

# Copy index.html, styles.css, and README.md from this starter folder into this repo.
# For example, if the starter folder is in Downloads:
cp ~/Downloads/derekastro_github_pages_site/index.html .
cp ~/Downloads/derekastro_github_pages_site/styles.css .
cp ~/Downloads/derekastro_github_pages_site/README.md .

git status
git add index.html styles.css README.md
git commit -m "Add personal website"
git push origin main
```

Then visit `https://derekastro.github.io/`.
