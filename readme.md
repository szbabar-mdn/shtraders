# SH Traders — website

A plain static website built from the SH Traders printed product catalogue.
No build step, no database, no server-side code. Upload the files and it works.

## What's in here

```
index.html          Home
designs.html        Designs section
printing.html       Printing section (17 products + finishing key)
large-format.html   Large Format section (16 products)
gadgets.html        Gadgets section (8 products)
contact.html        Contact details
robots.txt
sitemap.xml         Update the domain inside before submitting to Google
assets/css/site.css Single stylesheet
assets/img/         Logo, section photos, rainbow artwork
assets/img/p/       41 product photos (WebP, transparent background)
```

## Putting it on your domain

**cPanel / Hostinger / any shared host**
1. Log in and open **File Manager**.
2. Go into `public_html`.
3. Upload the ZIP, then use **Extract**. Make sure `index.html` ends up directly
   inside `public_html`, not inside an extra folder.
4. Visit your domain. Done.

**FTP (FileZilla)**
Connect with the FTP details from your host and drag the *contents* of this folder
into `public_html` (or `www`, depending on the host).

**Netlify (free, fastest)**
Go to app.netlify.com, drag this whole folder onto the upload area, then attach your
domain under Domain settings.

**GitHub Pages (free)**
Create a repository, upload these files, then Settings → Pages → deploy from the
`main` branch, root folder.

## Editing later

Everything is ordinary HTML. To change a price, phone number or paragraph, open the
`.html` file in any text editor, edit the words, and re-upload that one file.

Colours, fonts and spacing all live in `assets/css/site.css` at the top, under `:root`.

Contact details appear in the header, footer and on `contact.html` — search for
`0333-9876051` to find every place it is used.

## Before you go live — two things to check

1. **sitemap.xml** still says `https://example.com/`. Replace it with your real domain.
2. **The product photos came from the catalogue's stock images.** Several carry text in
   Polish or German (Belleza, Ogrofol, Ventriculus, "Digitaldruck"). They look fine as
   generic samples, but replacing them with photographs of your own work would be
   stronger. Drop a replacement into `assets/img/p/` using the same filename and it will
   appear automatically — for example `assets/img/p/banners.webp`.

## Fonts

Headings use Archivo Narrow and body text uses Archivo, loaded from Google Fonts.
If your visitors have slow connections, the site falls back to Arial automatically and
still looks correct.
[![Netlify Status](https://api.netlify.com/api/v1/badges/7db37a40-32a1-4dd4-a617-adfe7dc4c9f4/deploy-status)](https://app.netlify.com/projects/shtraders/deploys)
