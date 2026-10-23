Visit **[biomedical-ai-lab.github.io](https://biomedical-ai-lab.github.io)** 🚀

# Biomedical AI Lab website

Source for the Biomedical AI Lab website, built with the [Lab Website Template](https://greene-lab.gitbook.io/lab-website-template-docs) (Jekyll + GitHub Actions).
The site is published at **https://biomedical-ai-lab.github.io/** (this needs the repo to be named `biomedical-ai-lab.github.io`). At launch it moves to **biomed-ai.com**.

## How the site is organized

| Page | File | Data it reads |
| --- | --- | --- |
| Home | `index.md` | `_includes/themes.html`, featured papers, latest news |
| Research | `research/index.md` | papers tagged `gait`, `wearables`, `language`, `imaging`, `neuroscience` |
| Publications | `publications/index.md` | `_data/citations.yaml` (generated) |
| People | `people/index.md` | `_members/*.md`, `_data/alumni.yaml` |
| Prof. Albert's profile | `_members/mark-v-albert.md` | `_data/courses.yaml` (Teaching section) |
| Software & Data | `software/index.md` | `_data/projects.yaml` |
| News | `news/index.md` | `_posts/*.md` |
| Join Us | `join/index.md` | |
| Contact | `contact/index.md` | `_data/affiliation.yaml` |

## Branding: one file

Everything that names a university lives in **`_data/affiliation.yaml`**: institution, department, logo files, address, colors and fonts.
If the lab moves, edit that file and replace the logos in `images/affiliation/`. No page needs to change.

- The lab's own logo is `images/logo.png` (the turtle, shown in the header). Keep it separate from any university mark.
- University marks must be the official files from the university's identity guide, unedited.
- Pages should never write the university's name or a hex color directly; use `{{ site.data.affiliation.institution }}` and the CSS variables instead.

## "Under construction" switch

`under-construction` in `_config.yaml` controls what the public sees:

- `true`: every page at the public address shows a placeholder (lab name, contact email, social links).
- `false`: the full site is public.

Local previews (`bundle exec jekyll serve`) and pull-request preview links always show the full site, so you can keep working while the placeholder is up.
To see the placeholder locally, run `$env:JEKYLL_ENV="production"; bundle exec jekyll serve` in PowerShell (close and reopen the terminal afterwards to clear it).

## Common tasks

Every change goes through a pull request: edit on a branch, open a PR, check the preview link the bot posts, then merge.

### Add a paper

Add its DOI (or `arxiv:` / `pubmed:` id) to `_data/sources.yaml` with theme tags. The cite workflow turns it into a full citation in `_data/citations.yaml`; never edit that file by hand.

### Pull all of Prof. Albert's papers automatically

Create `_data/orcid.yaml` with his ORCID iD:

```yaml
- orcid: 0000-0000-0000-0000
```

Every work on his ORCID record with a DOI is then cited automatically. Keep `sources.yaml` for tags, buttons and papers ORCID is missing.

### Add or update a person

Create `_members/first-last.md` (copy an existing one). Set `role` to `principal-investigator`, `phd`, `ms`, `undergrad` or `affiliated`.
Put a square headshot at `images/team/first-last.jpg`; until then a placeholder shows.
When someone leaves, delete their member file and add them to `_data/alumni.yaml` with their next position.

### Add a course

Add an entry to `_data/courses.yaml`. Mark the one or two newest courses `recent: true` to show them as cards. Courses at the institution named in `affiliation.yaml` show open; earlier institutions fold away automatically.

### Post news

Add `_posts/YYYY-MM-DD-short-title.md` with a `title` and a few sentences. The home page shows the latest five.

## First-time setup on GitHub (once)

1. **Settings → Actions → General → Workflow permissions:** choose "Read and write permissions" and allow Actions to create pull requests.
2. Push to `main`. The `on-push` workflow builds the site into the `gh-pages` branch.
3. **Settings → Pages:** deploy from branch `gh-pages`, folder `/ (root)`.
4. At launch: add `biomed-ai.com` under **Settings → Pages → Custom domain**, update the domain's DNS at its registrar as GitHub's Pages docs describe, and retire the Google Site.

Until the custom domain is set, the site is at `https://biomedical-ai-lab.github.io/`.

## Still to do

- [ ] Prof. Albert reviews his draft bio in `_members/mark-v-albert.md`
- [ ] Add his ORCID iD (see above)
- [ ] Headshots in `images/team/` for the members who don't have one yet (13 done)
- [x] Lab logo (`images/logo.png`), browser icon (`images/icon.png`) and share image (`images/share.jpg`)
- [ ] Official university logo files in `images/affiliation/`, then set `logo` and `logo_dark` in `affiliation.yaml`
- [ ] Confirm the Google Docs syllabus links are shared publicly
- [ ] Links for the 5 tools listed under "In the works" on Software & Data

## Credits

Built on the [Lab Website Template](https://github.com/greenelab/lab-website-template) by the Greene Lab (BSD-3-Clause, see `LICENSE.md`).
