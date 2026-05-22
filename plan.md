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

## 13. Questions to Answer Before Implementation

Answer these before building the first version of the site.

1. What should be the public GitHub Pages URL?
   - Recommended default: use the existing repository `skitimo/website` first, then decide later whether to move to `skitimo.github.io`.
   - Answer: Use the existing `skitimo/website` repository for version 1. Expected GitHub Pages URL: `https://skitimo.github.io/website/`.

2. Should the first version be deployed from `skitimo/website`, even though the URL will likely be `https://skitimo.github.io/website/`?
   - Recommended default: yes, because the repository already exists.
   - Answer: Yes.

3. Should the website publish the CV PDF?
   - Recommended default: publish a web-safe CV only after removing private details such as phone number if needed.
   - Answer: Yes, publish the CV PDF.

4. Should the phone number from the CV appear on the public website?
   - Recommended default: no, use email and public profile links only.
   - Answer: Not explicitly answered. Use the default for the webpage: do not show the phone number in page content. Note that the published CV PDF may still contain it unless a redacted CV is provided.

5. Which email address should be public?
   - Current candidate from CV: `sippanon.kitimoon@gmail.com`.
   - Answer: Use `sippanon.kitimoon@gmail.com` unless replaced later.

6. Should `mypic.jpeg` be used as the main hero image?
   - Recommended default: crop it into a clean portrait/headshot for the website and keep the full poster out of the hero.
   - Answer: Yes, use a cropped version of the provided welcome image as the hero portrait.

7. Do you have a separate preferred headshot or profile photo?
   - Recommended default: use a cropped version of `mypic.jpeg` if no other photo is available.
   - Answer: No separate headshot provided. Use the cropped welcome image.

8. Should the first site be a single-page website or multiple pages?
   - Recommended default: single-page version 1 with section anchors.
   - Answer: Single-page website for version 1.

9. Should the first version include Thai content?
   - Recommended default: English-only version 1, with optional Thai introduction later.
   - Answer: English-only for version 1.

10. What title should appear in the hero?
    - Candidate: `Computational Applied Mathematician`
    - Candidate: `Data & Signal Processing Engineer`
    - Candidate: `Lecturer, Data Science Research Center, Faculty of Science, Chiang Mai University`
    - Answer: Not explicitly answered. Use `Computational Applied Mathematician` as the primary title and `Data & Signal Processing Engineer` as the secondary descriptor.

11. What affiliation wording should be used?
    - Candidate: `Data Science Research Center, Faculty of Science, Chiang Mai University`
    - Answer: Use `Data Science Research Center, Faculty of Science, Chiang Mai University`.

12. Should the start date from the welcome poster appear on the site?
    - Current source says: starting April 1, 2026.
    - Recommended default: include it only in the About section, not the hero.
    - Answer: Not explicitly answered. Use the default: include the April 1, 2026 start date only in the About section.

13. Which public profile links should be included?
    - Current candidate: Google Scholar `https://scholar.google.com/citations?user=DyFbVikAAAAJ`
    - Need confirmation: GitHub, LinkedIn, CMU profile, ORCID, ResearchGate, personal email.
    - Answer: Include Google Scholar and email for version 1. Add GitHub/LinkedIn/CMU/ORCID/ResearchGate only after URLs are confirmed.

14. Should publications be manually listed in version 1 or only linked through Google Scholar?
    - Recommended default: link to Google Scholar in version 1.
    - Answer: Not explicitly answered. Use the default: link to Google Scholar in version 1.

15. Are there selected research projects or publications that must be highlighted on the homepage?
    - Recommended default: no selected highlights until confirmed.
    - Answer: Not explicitly answered. Use the default: no selected publication/project highlights in version 1.

16. Should consulting or industry collaboration be presented explicitly?
    - Recommended default: mention industry analytics experience, but avoid making the site feel like a consulting landing page.
    - Answer: Not explicitly answered. Use the default: mention industry analytics experience without making the site feel like a consulting landing page.

17. Should the design use CMU/DSRC branding colors and logos?
    - Recommended default: use color inspiration only unless logo usage is clearly permitted.
    - Answer: Not explicitly answered. Use the default: take color inspiration from CMU/DSRC, but do not use official logos as standalone assets unless provided.

18. Should the logos visible in the welcome image be reused separately on the website?
    - Recommended default: no, unless official logo assets and usage permission are available.
    - Answer: Not explicitly answered. Use the default: do not reuse logos separately.

19. Should the site include a downloadable vCard/contact card?
    - Recommended default: no for version 1.
    - Answer: Not explicitly answered. Use the default: no vCard for version 1.

20. Should the site include analytics?
    - Recommended default: no for version 1.
    - Answer: Not explicitly answered. Use the default: no analytics for version 1.

21. Should I commit and push implementation changes automatically after review, or stop after local implementation?
    - Recommended default: commit locally and ask before pushing.
    - Answer: Yes, commit implementation changes locally and ask before pushing.
