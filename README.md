# Joonyoung Kim — Academic Website

A minimal academic website for `joonyoungk.github.io`.

The site uses **GitHub Pages + Jekyll only**. There is no external theme,
JavaScript framework, or UI library, so most updates require editing only
Markdown/YAML files.

## 1. Files you will edit most often

| What to change | File |
|---|---|
| Name, status, affiliation, links | `_data/profile.yml` |
| About text | `index.md` |
| Publications | `_data/publications.yml` |
| Code repositories | `_data/code.yml` |
| Education / research experience / skills / scholarships | `_data/cv.yml` |
| CV PDF | `files/Joonyoung_Kim_CV.pdf` |
| Profile photo | `assets/images/profile.jpg` |
| Main colors / spacing / typography | `assets/css/main.css` |
| Top navigation | `_data/navigation.yml` |

## 2. Add your profile photo

1. Upload a square or portrait photo as:

   `assets/images/profile.jpg`

2. Open `_data/profile.yml` and change:

```yaml
image: ""
```

to:

```yaml
image: "/assets/images/profile.jpg"
```

If `image` is blank, the site shows the `JK` placeholder automatically.

## 3. Add Google Scholar / ORCID

Open `_data/profile.yml`.

```yaml
google_scholar_url: "YOUR_URL"
orcid_url: "YOUR_URL"
```

Blank URLs are automatically hidden.

## 4. Add a publication

Open `_data/publications.yml` and copy an existing publication block.

You can add links later:

```yaml
pdf: "https://..."
doi: "https://..."
code: "https://github.com/..."
project: "https://..."
```

A button is displayed only when its URL is not blank.

## 5. Add a code repository

Open `_data/code.yml` and replace `[]` with:

```yaml
- title: "Repository title"
  description: "One-sentence description."
  github: "https://github.com/joonyoungk/repository-name"
  publication: "Related publication title"
  language: "Python"
  tags:
    - "Transportation"
    - "Bayesian Modeling"
```

Add another block for each repository.

## 6. Update the CV PDF

Replace:

`files/Joonyoung_Kim_CV.pdf`

with a new PDF using the **same filename**.

The CV download button will continue working without any code change.

## 7. Change the design

The easiest global settings are at the top of:

`assets/css/main.css`

For example:

```css
--accent: #315f85;
--page-width: 1180px;
--content-width: 790px;
--sidebar-width: 270px;
```

The default design intentionally uses a white background, restrained color,
a sticky desktop sidebar, and a simple academic bibliography layout.

## 8. Publish on GitHub Pages

Repository name:

`joonyoungk.github.io`

After uploading these files, open the repository's **Settings → Pages** and
publish from the `main` branch and repository root if branch publishing is
being used.

Your site URL is:

`https://joonyoungk.github.io`

## 9. Current TBD items

The following are intentionally not shown until you add them:

- Research Interests
- Google Scholar
- ORCID
- Public code repositories
- Publication PDF / DOI / Code links
- Profile photo

This avoids displaying "TBD" publicly.
