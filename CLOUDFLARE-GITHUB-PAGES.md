# CAR Website — GitHub Pages + Cloudflare setup

The package now contains a real `CNAME` file for **careco.in**, an XML sitemap, and a matching `robots.txt`. The apex domain is treated as canonical because `careco.in` is the domain shown in the supplied website screenshot.

## Publish the files

1. Upload the **contents** of this folder to the root of the GitHub repository; `index.html`, `CNAME`, `robots.txt`, `sitemap.xml`, `.nojekyll`, `assets/` and the other HTML pages must be at the repository root.
2. In GitHub, open **Settings → Pages**. Use **Deploy from a branch**, branch `main`, folder `/(root)`.
3. In **Custom domain**, enter `careco.in` and save. The included `CNAME` file already contains this domain.
4. Wait for DNS verification. Then enable **Enforce HTTPS** when the setting becomes available.

## Cloudflare DNS

For an apex domain (`careco.in`), the common GitHub Pages records are four `A` records for `@` pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, and `185.199.111.153`. To support `www.careco.in` as well, add a `CNAME` record for `www` pointing to `navneetchandra34-dotcom.github.io` and create a Cloudflare Redirect Rule that redirects `www.careco.in/*` to `https://careco.in/$1` (preserving the path and query string).

Initially set the GitHub Pages records to **DNS only** (grey cloud) while GitHub verifies the custom domain and certificate. Remove conflicting old `A`, `AAAA`, or `CNAME` records for the same host. **Do not delete mail-related `MX`, SPF, DKIM, or DMARC records.** Do not use an old or unknown AAAA record for the website host. After HTTPS is working, follow your intended Cloudflare proxy configuration.

## Files included

- `CNAME` — canonical custom domain, `careco.in`
- `robots.txt` — permits crawling and advertises the sitemap
- `sitemap.xml` — page URLs under `https://careco.in/`
- `.nojekyll` — avoids Jekyll processing

## Official documentation

- GitHub custom domains: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site
- GitHub DNS configuration: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
- Cloudflare DNS records: https://developers.cloudflare.com/dns/manage-dns-records/how-to/create-dns-records/
