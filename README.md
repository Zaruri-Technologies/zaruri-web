# Zaruri Coming Soon

A private, minimal coming-soon page with an animated circular glow. It intentionally contains no logo, company name, product description, contact form, analytics, or external dependencies.

## Files

- `index.html` — the complete website (HTML and CSS in one file)
- `README.md` — setup and deployment instructions

## Preview on your computer

You can double-click `index.html` to open it in a browser.

For a local web-server preview, open a terminal in this folder and run:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Upload to GitHub

1. Create or open the GitHub repository you want to use for the public Zaruri website.
2. Choose **Add file → Upload files**.
3. Upload `index.html` and `README.md` from this folder. Upload the files themselves, not the ZIP file.
4. Commit the files to the `main` branch.

## Deploy with Vercel

1. In Vercel, select **Add New → Project**.
2. Import the GitHub repository containing these files.
3. Leave **Framework Preset** as `Other`.
4. Leave **Build Command** empty.
5. Leave **Output Directory** empty (or use `.` if Vercel requires a value).
6. Select **Deploy**.
7. In the Vercel project, open **Settings → Domains** and add `zaruri.ai`.
8. Follow the DNS instructions shown by Vercel.

Every later commit to the repository will automatically trigger a new Vercel deployment.

## Privacy note

The page uses `noindex, nofollow` to ask search engines not to index it. This is not a secrecy guarantee: anyone who knows the domain can still visit the page. The source contains no product details.

## Customization

All styling is inside `index.html`. The main colors are defined at the top of the `<style>` block. The ring speed is controlled by this line:

```css
animation: orbit 9s linear infinite;
```

Change `9s` to a higher value for slower rotation or a lower value for faster rotation.
