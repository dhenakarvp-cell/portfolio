# Dhenakar VP portfolio

A static site with no build step. Vercel serves the files as they are.

## Files

- `index.html`: the whole site (styles and script are inside it)
- `404.html`: page shown for broken links
- `favicon.svg`: browser tab icon
- `assets/og-image.png`: preview image for LinkedIn, WhatsApp and Slack shares
- `robots.txt`, `sitemap.xml`: for search engines
- `vercel.json`: clean URLs, caching and security headers

## Deploy on Vercel (free)

1. Create a free account at github.com.
2. Click **New repository**, name it `portfolio`, set it to Public, and create it.
3. On the repository page, click **uploading an existing file**. Drag in everything from this folder, including the `assets` folder, then click **Commit changes**.
4. Go to vercel.com and sign up with your GitHub account.
5. Click **Add New → Project**, pick the `portfolio` repository and click **Import**.
6. Leave every setting as it is (Framework Preset: Other) and click **Deploy**.
7. Your site goes live at an address like `portfolio-xxxx.vercel.app`.

To get `dhenakar.vercel.app`: in Vercel, open the project, go to **Settings → Domains**, and add `dhenakar.vercel.app`. If that name is taken, pick another and update the URLs below.

## After the first deploy

1. If your final address isn't `dhenakar.vercel.app`, replace it everywhere in `index.html`, `robots.txt` and `sitemap.xml` (search and replace), then upload the changed files.
2. Add the site to Google Search Console as a URL-prefix property, verify it with the HTML tag method (paste the meta tag into the `<head>` of `index.html`), and submit `sitemap.xml`.
3. Test the structured data at search.google.com/test/rich-results.

## Editing later

Edit a file on GitHub (pencil icon) and commit. Vercel redeploys automatically in under a minute.

- **Add your photo:** upload a square image as `assets/dhenakar.jpg` (about 400 × 400 px). It replaces the DV circle automatically.
- **Add a resume download:** upload `assets/Dhenakar-VP-Resume.pdf`, then remove the `<!--` and `-->` around the "Download resume" button in the Contact section of `index.html`.
- **Update the date:** change `dateModified` in the JSON-LD and `lastmod` in `sitemap.xml` when you make real content changes.
