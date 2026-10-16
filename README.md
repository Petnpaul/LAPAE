# LAPAE Website — Version 1.0

A lightweight, responsive, multi-page static website for LAPAE Event Matching. Built with plain HTML, CSS, local SVG illustrations, and a tiny JavaScript file for the mobile navigation. No forms, account signup, analytics, advertising pixels, external fonts, or third-party embedded widgets are included.

## Files

- `index.html` — home page
- `solutions.html` — corporate event solutions
- `how-it-works.html` — event matching process
- `organizers.html` — for event organizers
- `about.html` — about LAPAE
- `contact.html` — email contact only
- `assets/` — CSS, JavaScript, logo, favicon, local SVG illustrations
- `CNAME` — custom domain `lapae.net`

## Brand decisions included

- Brand: LAPAE
- Positioning: Event Matching — “Where the right matches happen”
- Vietnamese headline: “Kết nối đúng đối tác cho mọi sự kiện.”
- Background: Warm Ivory `#F5F3ED`
- Primary text: Deep Navy `#101C2D`
- Accent: Teal `#46C6AD`
- Contact email: `lapaejsc@gmail.com`
- Logo: supplied transparent 2D PNG; the “Lapae” wordmark is stacked below the emblem. The wordmark uses the existing Inter/system sans-serif stack in deep navy (#101C2D) on light surfaces and white in the footer. Browser and Apple touch icons use the same supplied logo.

## Test locally

You can open `index.html` directly in a browser. For a local server, run from this directory:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish with GitHub Pages

This package is prepared for a public GitHub repository and GitHub Pages' branch-based publishing. Follow the current GitHub and Namecheap documentation if their screens or DNS instructions change.

1. Create a **public** GitHub repository for the website (for example, `lapae-website`).
2. Upload the **contents** of this folder to the repository root. Keep `CNAME` at the root.
3. In the repository, open **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, branch `main`, folder `/ (root)`, then save.
4. Under **Settings → Pages → Custom domain**, enter `lapae.net` and save. Configure the custom domain in GitHub **before** updating DNS.
5. In Namecheap **Domain List → Manage → Advanced DNS**, set the apex domain records for GitHub Pages. The current GitHub documentation lists these `A` records for host `@`:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
6. Recommended: add a `CNAME` record for host `www` that points to `<YOUR-GITHUB-USERNAME>.github.io` (replace the placeholder with the account's GitHub Pages domain, and do **not** include a repository name). Keep any future email-related DNS records separate; Version 1 does not require domain email or MX records.
7. Remove only conflicting default/parking records that prevent these records from working. DNS changes may take up to 24 hours to propagate. After GitHub verifies the domain and certificate is ready, enable **Enforce HTTPS** under **Settings → Pages**.
8. Test `https://lapae.net` and, if configured, `https://www.lapae.net`; verify desktop/mobile layouts and all page links.

Official guides: [GitHub Pages custom domains](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) · [GitHub Pages publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) · [Namecheap: connect a domain to GitHub Pages](https://www.namecheap.com/support/knowledgebase/article.aspx/9645/2208/how-do-i-link-my-domain-to-github-pages/).

This package is prepared for deployment, but it has **not** been published to a live GitHub repository or connected to Namecheap. That requires access to the user's GitHub and Namecheap accounts.

## Privacy-conscious Version 1

There are no on-site forms, login features, analytics scripts, ad trackers, or external font/image requests. The contact action opens the visitor's email application via `mailto:`. The hosting provider may still process technical request logs as part of serving the website; review current GitHub Pages documentation and any applicable privacy obligations before launch.

## Before going live

- Confirm the domain is purchased and DNS is configured.
- Confirm LAPAE's public email address.
- Review all service descriptions to ensure they accurately represent what LAPAE is currently prepared to offer.
- Add verified legal company details only if/when ready; no unverified company address, phone, client logos, testimonials, or statistics have been fabricated here.
