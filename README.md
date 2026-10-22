# Centre for Action Research — website package

This is the complete static website for Centre for Action Research (CAR), prepared for GitHub Pages with Cloudflare DNS. The site retains the fuller organisational profile and long-form programme, field-story, partnership, and governance content while applying the current feedback.

## Included pages

- `index.html` — Home
- `about.html` — Who we are
- `programmes.html` — Our work (six programme areas, consistent image panels)
- `impact.html` — Impact & stories (river action, adult literacy, PVTG support, seed-ball activity, Forest Rights Act convention, reporting timeline and field photos)
- `governance.html` — Governance, policy headings, statutory information and downloadable Section 12AB and 80G orders
- `partnerships.html` — Partnership pathways, collaborator years and bank transfer information
- `contact.html` — Contact details and a mailto-based enquiry form, separate from partnership and bank-transfer information

## Publish to GitHub Pages

1. Extract the ZIP. Open the `car-website` folder.
2. Upload the **contents** of `car-website` (not the enclosing folder itself) to the root of your GitHub repository. The repository root should contain `index.html`, `about.html`, `documents/`, `assets/`, `CNAME`, `robots.txt`, and `sitemap.xml`.
3. In GitHub, open **Settings → Pages** and choose the `main` branch and `/(root)` folder (or preserve the repository’s existing Pages source if it is already correctly configured).
4. Confirm the custom domain is `careco.in`. Enable HTTPS once GitHub confirms that the domain and DNS are verified.

## Cloudflare DNS

For GitHub Pages, the apex domain typically uses the four A records below. Add them only after checking for duplicate/conflicting records:

- `@` → `185.199.108.153`
- `@` → `185.199.109.153`
- `@` → `185.199.110.153`
- `@` → `185.199.111.153`

Keep these records DNS-only (grey cloud) during initial GitHub Pages domain verification and HTTPS setup. Do not remove MX, SPF, DKIM, DMARC, or other unrelated email records.

## Important content checks

- The bank details are on the **Partnerships** page. The official Punjab & Sind Bank branch list shows IFSC `PSIB0000789` for Bhubaneswar Biju Patnaik College branch. Verify the beneficiary account number against CAR’s bank-issued record before public launch or accepting transfers.
- The website displays **20 villages** for adult-literacy coverage, as instructed in the earlier revision transcript. The uploaded annual-report document describes 12 villages; CAR should reconcile this difference with the latest programme records before publishing.
- The Governance page provides downloadable copies of the two Form 10AD orders supplied with this brief. The 80G order states that continued validity depends on valid Section 12A/12AB registration for the relevant period.
- Confirm that CAR has permission to publish identifiable field photographs, particularly photos containing children or vulnerable community members.

## Notes

This is a static website. The Contact enquiry form prepares an email in the visitor’s default mail application; it does not store submissions on a server.
