# GitHub Pages + Cloudflare deployment for careco.in

## 1. Upload the website
Upload the **contents** of the `car-website` folder to your repository root. Verify that `index.html` is at the root level and the `assets/` and `documents/` folders remain intact.

## 2. GitHub Pages
In repository **Settings → Pages**, publish from `main` and `/(root)`. In the Custom domain field, enter `careco.in`. Wait until GitHub reports the domain as verified before enabling Enforce HTTPS. The file `CNAME` contains `careco.in`.

## 3. Cloudflare DNS
For the apex domain, configure A records to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, and `185.199.111.153`, with name `@`. Use DNS-only during initial verification. Remove conflicting A/AAAA records for the same hostname only after checking that they are not required for other services. Preserve MX and email authentication records.

If you also want `www.careco.in`, add a CNAME for `www` pointing to your GitHub Pages hostname (`YOUR-GITHUB-USERNAME.github.io`) and configure the preferred redirect/canonical domain consistently.

## 4. Files to keep
`CNAME`, `.nojekyll`, `robots.txt`, `sitemap.xml`, all HTML files, `assets/`, and `documents/`. Do not upload a placeholder CNAME; this package already includes the domain from the supplied screenshot.

## 5. Before launch
Verify the bank account/IFSC against the bank-issued record, confirm the current adult-literacy village count against programme records, and ensure photo permissions are in place.
