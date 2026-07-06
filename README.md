# OwnlyMe website

Static multi-page B2C site. No build step. Deploy the files in this folder as-is.

## Push to GitHub, then Vercel
```
cd ownlyme
git init
git add .
git commit -m "OwnlyMe site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/ownlyme.git
git push -u origin main
```
On Vercel: Add New > Project > import the repo. Framework Preset: Other. No build command. Add your domain under Settings > Domains.

## Set before launch
- Canonical URLs, robots.txt, sitemap.xml, and llms.txt all use https://ownlyme.com/ as a placeholder. Replace with your live domain.
- The contact form opens a mailto to hello@valearion.com. Change it in get-started.html if OwnlyMe has its own inbox.
- robots.txt, sitemap.xml, and llms.txt belong at the domain root, next to index.html.

## Notes on this rebuild
- Rebuilt as four real pages (was a single-file app with JS-swapped views), so search engines and AI assistants can index each page. Added per-page titles and meta, Organization + SoftwareApplication + FAQPage schema, llms.txt, robots.txt, sitemap.xml.
- All B2B "liability" and per-pulse pricing language removed from the consumer pages.
- Removed hotlinked stock photos in favour of the credential visual and clean layout, on brand for a privacy product and better for speed and indexing.
