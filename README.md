# The New Business Project

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/RoyWraps69/thenewbusinessproject)

**👆 Click this button to deploy this site to Netlify in 60 seconds.**

---

A civic program providing **new Chicagoland businesses** with their first essential services — free of charge.

Co-founded by:
- **[Chicago Fleet Wraps](https://chicagofleetwraps.com)** — vehicle graphics
- **[Regions PM](https://regionspm.com)** — property management

## Live site

**[thenewbusinessproject.com](https://thenewbusinessproject.com)**

## What the program offers

Any Chicagoland business with a license, LLC formation, or DBA registration dated within the last **90 days** qualifies for:

- **Free vehicle graphics** — up to 8 sq ft of cast vinyl, designed and installed at no cost (provided by Chicago Fleet Wraps)
- **Free property search consultation** — help finding office, retail, or warehouse space in Chicagoland (provided by Regions PM)
- **More services as new partners join** — actively recruiting attorneys, accountants, banks, payroll providers, web designers, printers, marketing agencies, insurance brokers

### Eligibility

| | |
|---|---|
| Geographic | Cook, DuPage, Lake, Kane, Will, or McHenry County, IL |
| Business age | License / formation date within the last 90 days |
| Income test | None |
| Industry filter | None |

## Repository structure

```
.
├── public/
│   ├── index.html          ← Main landing page (everything inline)
│   ├── thank-you/
│   │   └── index.html      ← Post-application page
│   ├── _redirects          ← Netlify redirects
│   ├── robots.txt
│   ├── sitemap.xml
│   └── favicon.svg
├── netlify.toml            ← Netlify build config
└── README.md
```

## Deployment

### Quick deploy (Netlify recommended)

1. Sign in to [Netlify](https://app.netlify.com)
2. **Add new site → Import existing project**
3. Connect this GitHub repo
4. Build settings: leave blank — publish directory is `public`
5. **Deploy site**
6. Domain settings → Add custom domain → `thenewbusinessproject.com`
7. Update DNS at your registrar to point to Netlify

### One-click button

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/RoyWraps69/thenewbusinessproject)

## How to add a partner

When a new service business signs on as a partner:

1. Add an entry to the `Partners` section in `public/index.html`
2. Add their organization to the `sponsor` array in the JSON-LD schema (also in `index.html`)
3. Optionally add their logo SVG to `public/partners/[name].svg` and reference it
4. Commit and push — Netlify auto-deploys

## How to add a recipient (public roster)

When a business goes through the program:

1. Add an entry to the `Recipients` section in `public/index.html` (currently shows a placeholder until first recipient)
2. Include business name, photo (with permission), industry, and date helped
3. Commit and push

## Contact

- **Program inquiries**: hello@thenewbusinessproject.com
- **Partner applications**: partners@thenewbusinessproject.com
- **Press**: press@thenewbusinessproject.com

## License

This site's source code is open. The "The New Business Project" name and program are trademarked by its founders.
