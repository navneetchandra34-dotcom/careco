# Centre for Action Research (CAR) — Website

A multi-page, responsive, static website for Centre for Action Research (CAR), built for GitHub Pages. The site uses plain HTML, CSS, and JavaScript; it has no build dependencies, package manager, server-side code, or paid components.

## Website contents

- `index.html` — homepage and programme overview
- `about.html` — identity, vision, mission, values, and approach
- `programmes.html` — thematic programme areas
- `impact.html` — reported activity highlights, campaigns, and forward plan
- `partnerships.html` — collaboration and CSR / institutional partnership information
- `governance.html` — leadership, policies, and statutory details provided in the source materials
- `contact.html` — office contact information and an email-compose helper
- `404.html` — branded not-found page
- `assets/` — local logo, photographs, styles, JavaScript, and favicon
- `.nojekyll` — prevents GitHub Pages from applying Jekyll processing

## Publish on GitHub Pages

1. Sign in to GitHub and create a **public repository** for the website (for example, `centre-for-action-research`). A public repository is the simplest free option for a public-facing organization site.
2. Extract this package. Upload **the contents of this folder** to the repository's top level, so `index.html` is at the repository root. Do not upload the ZIP as a ZIP file.
3. Commit the files to the `main` branch.
4. Open the repository's **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Select branch **`main`** and folder **`/(root)`**, then save.
7. Wait for the Pages deployment to finish. GitHub will show the published URL in Settings → Pages; it will usually be `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.
8. Open the published URL on a phone and a desktop browser. Test all menu items, contact links, and the email-compose helper.

Official GitHub instructions: <https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site>

### If you use a custom domain later

Configure the domain in **Settings → Pages** and add the DNS records GitHub specifies for that domain. Add the final HTTPS website address to the canonical URLs, Open Graph URL, sitemap, and `robots.txt` after the domain is confirmed. Those files are intentionally not pre-filled with an invented domain.

## Important notes about the contact and donation experience

- GitHub Pages serves static files; it does not run a private database, email handler, payment gateway, or server-side form processor.
- The contact-page form validates the fields in the browser and opens an email draft addressed to `centreforactionresearch@gmail.com`. It does **not** silently submit or store a visitor's information. Visitors can also use the directly displayed email address and phone numbers.
- No donation checkout, payment link, UPI QR, bank details, or donation promise has been invented. Add a donation/payment process only after CAR confirms its official account, receipt process, current tax eligibility, and any relevant compliance requirements. CSR support is presented as a partnership conversation rather than a checkout.

## Pre-launch fact-check and safeguarding checklist

The site is based on the two supplied Word documents and the photographs shared with the brief. Before publishing, CAR should approve the content and check these items:

- **Legal and tax status:** The supplied profile states registration under the Indian Trust Act, 1882; Section 12AA and Section 80G; NITI Aayog NGO Darpan; and CSR-related registration. Tax registrations and compliance requirements can change. Confirm each claim against current certificates and approved wording. The source's phrase “registered under Ministry of Commerce ... for CSR funding” should be checked against the actual CSR-1 / MCA record and must not be reproduced as a current legal assurance without verification.
- **Reporting-period figures:** The supplied activity summary reports 14 major programmes/visits/conventions/advocacy events; 6+ districts; 3 CSR/academic partnership meetings; 2 small-river restoration conventions; adult-literacy activity in 12 Rayagada villages; and support to 800+ PVTG families. Confirm the reporting period, source records, and any desired methodology before public use. They are presented as reported reach/activity highlights, not independently audited outcomes.
- **Sustainable Development Goals:** The supplied profile lists SDGs `1, 2, 3, 4, 8, 7, 8, 13, 15 and 16`, repeating Goal 8 and presenting Goals 7/8 out of numerical order. Confirm the organization’s intended SDG list before displaying individual goal badges or claims.
- **Vision wording:** The supplied profile offers two alternative vision statements. This site combines the underlying themes of ecological protection and dignified, equitable livelihoods; leadership should approve the final wording.
- **Leadership and partnerships:** Confirm current titles, spellings, role tenure, and permission to publish partner names/logos. The partner names on the site reflect the supplied documents and do not imply endorsement beyond the relationship stated there.
- **Photographs and informed consent:** Confirm consent, release, and organizational permission for each image, especially identifiable members of vulnerable/tribal communities and any children. Consider whether names, precise locations, or other identifying information should be omitted for safeguarding reasons. Replace any photo for which publication permission cannot be confirmed.
- **Policies and downloadable records:** The profile lists HR, financial management/accounts, POSH, procurement, and gender policies. Publish policy files, certificates, audited financial statements, annual reports, and board details only after checking they are current, approved for public distribution, and safe to disclose.
- **Donation transparency:** Before asking for donations, publish a verified process for fund use, receipts, tax eligibility where applicable, donor restrictions, contact for due diligence, and reporting of how funds are used. Do not claim foreign-contribution eligibility or FCRA status unless current records confirm it.
- **Content review:** Check dates, place spellings, partner descriptions, telephone numbers, email, and office address. Correct the source typo “Jual Oran” to the appropriate public spelling only after the organization confirms it; this website avoids relying on that spelling in prominent copy.

## Technical and accessibility notes

- The website is mobile responsive, has keyboard-focus styling, semantic landmarks, descriptive page titles, meta descriptions, reduced-motion support, and an accessible mobile navigation toggle.
- Images are stored locally in `assets/`; Google Fonts are loaded remotely when available, with system-font fallbacks.
- The email-compose helper requires an email app configured on the visitor's device. If CAR needs a true online form, connect a reputable form backend/service and update the privacy notice before launch.
- No analytics, trackers, cookies, external donation widgets, or user database are included.

## Updating the website

Edit the relevant `.html` file directly. Shared appearance is in `assets/styles.css`, and small interactions are in `assets/site.js`. Keep filenames and relative paths intact. After major edits, test every page and image locally, then commit changes to the `main` branch. GitHub Pages will republish automatically.
