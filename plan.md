# Personal Website Plan for Sippanon Kitimoon

## 1. Goal

Build a professional personal website for Sippanon Kitimoon, Ph.D. that presents a clear academic and industry profile:

- Computational applied mathematician
- Data and signal processing engineer
- Machine learning, NLP, and analytics practitioner
- New faculty member / lecturer at the Data Science Research Center, Faculty of Science, Chiang Mai University, starting April 1, 2026

The site should be hosted with GitHub Pages so it is easy to maintain, versioned in Git, and publicly accessible.

## 2. Primary Audience

- Research collaborators in applied mathematics, data science, signal processing, and harmonic analysis
- CMU students and faculty
- Industry clients interested in analytics, signal processing, machine learning, and software consulting
- Conference organizers, grant reviewers, and academic visitors
- Recruiters or partners who need a concise professional profile

## 3. Source Material

Use these local files as the initial content base:

- `kitimoon_cv.pdf`: official CV source
- `mypic.jpeg`: welcome poster / portrait asset from Data Science Research Center, Faculty of Science, Chiang Mai University

Important extracted profile details:

- Name: Sippanon Kitimoon, Ph.D.
- Location: Chiang Mai, Thailand
- Email: `sippanon.kitimoon@gmail.com`
- Public profile: Google Scholar `https://scholar.google.com/citations?user=DyFbVikAAAAJ`
- Current role context: Data Science Research Center, Faculty of Science, Chiang Mai University
- Professional identity: Data and Signal Processing Engineer
- Research/expertise areas:
  - Signal Processing
  - Mathematics of Data Science
  - Applied and Computational Harmonic Analysis
  - Machine Learning
  - Natural Language Processing
  - Software Development
- Education:
  - Ph.D. Mathematics, Claremont Graduate University, 2025
  - M.S. Mathematics, Claremont Graduate University, 2019
  - B.A. Mathematics and Computer Science, Pitzer College, 2017
- Experience highlights:
  - Senior Software Engineer, ACERTAS Analytics, 2017-Present
  - Machine Learning Researcher, American Express / Harvey Mudd College Clinic, 2016-2017
  - Research Assistant, Claremont McKenna College, 2016
  - Teaching Assistant, Claremont McKenna College, 2015-2016
  - Tutor, Pitzer College, 2014

## 4. Recommended Site Strategy

Start with a simple static website instead of a framework-heavy application.

Recommended stack:

- Plain HTML, CSS, and minimal JavaScript
- GitHub Pages from the root of the `main` branch
- `.nojekyll` file to prevent GitHub Pages from applying Jekyll processing
- Optional future migration to Astro or another static site generator only if the site grows into a blog, publication database, or multilingual content system

Reason:

- GitHub Pages supports static files directly.
- The first version should be easy to edit without a build pipeline.
- A personal academic website benefits from speed, clarity, and low maintenance.

## 5. Repository Plan

Preferred GitHub repository:

- If the GitHub username is `skitimo`, create `skitimo.github.io`.
- Otherwise create `<github-username>.github.io`.

This creates the clean user-site URL:

- `https://<github-username>.github.io/`

If using a normal project repository instead, the URL will usually include the repository name:

- `https://<github-username>.github.io/<repository-name>/`

Initial repository structure:

```text
/
  index.html
  .nojekyll
  README.md
  plan.md
  assets/
    css/
      styles.css
    js/
      main.js
    images/
      mypic.jpeg
  files/
    kitimoon_cv.pdf
```

Notes:

- Keep `index.html` at the root because GitHub Pages looks for `index.html`, `index.md`, or `README.md` as the entry file.
- Move the public CV PDF into `files/` only after checking whether the phone number and any other personal details should be public.
- Keep image filenames lowercase and stable for long-term links.

## 6. Information Architecture

Use a single-page site for version 1, with section anchors. This keeps the first release focused and fast.

Recommended navigation:

- Home
- About
- Research
- Experience
- Publications
- Teaching
- Contact
- CV

Recommended sections:

### Home

Purpose: Establish identity immediately.

Content:

- Name: Sippanon Kitimoon, Ph.D.
- Tagline: Computational Applied Mathematician | Data Science | Signal Processing
- Affiliation: Data Science Research Center, Faculty of Science, Chiang Mai University
- Short positioning statement:
  - "I work at the intersection of applied mathematics, signal processing, machine learning, and software systems for scientific and engineering problems."
- Primary actions:
  - View CV
  - Google Scholar
  - Email

### About

Purpose: Human-readable professional summary.

Draft direction:

- Mention Ph.D. in Mathematics from Claremont Graduate University.
- Emphasize 8+ years of industry experience in software development, data analytics, and signal processing.
- Connect academic mathematics with real-world computational systems.
- Include the CMU appointment context from the welcome poster.

### Research

Purpose: Make research identity clear to academic visitors.

Organize as three to five research themes:

- Signal Processing
- Mathematics of Data Science
- Applied and Computational Harmonic Analysis
- Machine Learning and Natural Language Processing
- Computational Methods for Science and Engineering

Each theme should include one concise paragraph and optional project examples later.

### Experience

Purpose: Show credibility across industry, research, and teaching.

Feature:

- ACERTAS Analytics: big data solutions, R/Python/C++, high-performance analytics, signal processing, machine learning, NLP, predictive modeling, client-facing analytic solutions
- American Express / Harvey Mudd College Clinic: hotel recommendation system, feature engineering, k-NN, TensorFlow, recommendation accuracy improvement
- Claremont McKenna College: image processing research, MATLAB/Python, teaching assistant work
- Pitzer College: mathematics tutoring

### Publications

Purpose: Avoid manually duplicating a full publication list at first.

Version 1:

- Add a short publications section with a link to Google Scholar.
- Include selected publications later if there are 3-5 papers to highlight.

### Teaching

Purpose: Support the CMU lecturer profile.

Content:

- Current/future teaching context at CMU
- Previous teaching assistant experience in Data Structures and Advanced Programming
- Mathematics tutoring for Calculus I, II, and III

Future additions:

- Courses taught
- Student project topics
- Office hours
- Course materials

### Contact

Purpose: Give visitors a clear next step.

Content:

- Email link: `mailto:sippanon.kitimoon@gmail.com`
- Google Scholar link
- GitHub or LinkedIn link if confirmed
- CMU/DSRC affiliation text

Privacy recommendation:

- Do not publish the phone number from the CV unless intentionally required.
- GitHub Pages sites are public by default, so remove or redact any sensitive details before publishing.

## 7. Visual Direction

Base the visual design on the CV and the CMU/DSRC welcome image, but make the website cleaner and more readable than a poster.

Recommended style:

- Academic, precise, calm, and modern
- White or near-white page background
- Deep navy text and navigation
- CMU/DSRC-inspired gold accent
- Muted blue or teal secondary accent for data science identity
- Use the portrait/poster image as an identity asset, not as a cluttered full-page background

Hero design:

- Left side: name, tagline, affiliation, actions
- Right side: portrait or cropped image
- If `mypic.jpeg` is the full poster, create a clean cropped portrait asset before final implementation

Typography:

- Use a readable system font stack first.
- Use strong hierarchy but avoid oversized poster-style text on the website.
- Keep body text concise.

Accessibility:

- Ensure color contrast is strong.
- Add descriptive `alt` text for images.
- Make navigation keyboard accessible.
- Use semantic HTML sections and headings.

## 8. Content Tone

Use English as the primary language for version 1.

Optional bilingual enhancement:

- Add a short Thai welcome/affiliation note later for CMU visitors.
- Do not build a full language switcher in version 1 unless Thai content will be maintained consistently.

Writing style:

- Clear, professional, and specific
- Avoid inflated claims
- Emphasize concrete domains: applied mathematics, signal processing, machine learning, NLP, analytics, software systems

## 9. GitHub Pages Deployment Plan

Version 1 branch-based deployment:

1. Create or initialize a Git repository in this folder.
2. Add `index.html`, `assets/`, `files/`, `.nojekyll`, `README.md`, and `plan.md`.
3. Commit the first version.
4. Create the GitHub repository named `<github-username>.github.io`.
5. Push the local repository to GitHub.
6. In GitHub, open repository Settings -> Pages.
7. Set Source to "Deploy from a branch".
8. Select branch `main` and folder `/ (root)`.
9. Save and wait for the deployment.
10. Visit `https://<github-username>.github.io/`.

If a build tool is added later:

- Switch Pages source to GitHub Actions.
- Add a workflow that checks out the repo, builds the static site, uploads the Pages artifact, and deploys it.

GitHub documentation references:

- Creating a GitHub Pages site: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- Configuring a publishing source: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 10. SEO and Sharing

Add these in version 1:

- Page title: `Sippanon Kitimoon, Ph.D. | Data Science and Signal Processing`
- Meta description:
  - `Personal website of Sippanon Kitimoon, Ph.D., computational applied mathematician working in data science, signal processing, machine learning, and applied mathematics.`
- Open Graph title, description, and image
- Favicon
- Structured data later if needed

Suggested URL slugs if the site expands:

- `/research/`
- `/publications/`
- `/teaching/`
- `/cv/`

## 11. Version 1 Build Checklist

Content:

- Write homepage copy from CV summary.
- Add research theme summaries.
- Add experience timeline.
- Add publication link to Google Scholar.
- Add contact links.
- Decide whether to include public CV PDF.

Assets:

- Move `mypic.jpeg` to `assets/images/`.
- Create a cropped portrait if needed.
- Move `kitimoon_cv.pdf` to `files/` only after privacy review.
- Add favicon.

Implementation:

- Create `index.html`.
- Create `assets/css/styles.css`.
- Create minimal `assets/js/main.js` only if needed.
- Add responsive layout for mobile and desktop.
- Add `.nojekyll`.
- Add `README.md` with local editing/deployment notes.

Quality checks:

- Test locally in a browser.
- Check mobile layout.
- Validate links.
- Confirm email link works.
- Confirm CV link works if published.
- Run an accessibility/color contrast check.
- Confirm image alt text and heading structure.

Deployment:

- Initialize Git.
- Commit files.
- Push to GitHub.
- Enable GitHub Pages.
- Verify live URL.

## 12. Future Enhancements

Add only after the first version is live:

- Selected publications with BibTeX links
- Research project pages
- Student project topics
- Teaching pages for CMU courses
- Blog or notes on signal processing, mathematics of data science, and computational methods
- Thai-language introduction page
- Custom domain
- Analytics
- Automated publication sync from Google Scholar or a maintained BibTeX file

## 13. Open Decisions Before Implementation

- Confirm GitHub username and final repository name.
- Confirm whether the website should publish the phone number.
- Confirm whether `mypic.jpeg` should be used as-is, cropped into a portrait, or replaced with a separate headshot.
- Confirm whether the initial site should be single-page only or include separate pages.
- Confirm whether Thai content is needed in version 1.
