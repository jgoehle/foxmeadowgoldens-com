# Fox Meadow Goldens — How to update the website

This site is plain HTML — no complicated software. Here are the only three things
you'll ever really need to do.

## 1. Announce a new litter (or go back to "no litters")

Open **`puppies.html`** and find the block near the top marked:

```
<!-- LITTER STATUS — THIS IS THE ONE BLOCK TO EDIT WHEN THINGS CHANGE. -->
```

Change the heading and paragraph inside that box. For example:

- **New litter:** `<h2>Puppies have arrived! 🎉</h2>` and a paragraph with the
  born date, how many males/females, and when they'll be ready.
- **Back to none:** change it back to `<h2>No litters at this time</h2>`.

The homepage (`index.html`) has a matching status box — update it the same way so
the two agree.

## 2. Add photos to the gallery

1. Put your image files into the **`images`** folder.
2. Open **`gallery.html`**, find the `<div class="gallery" id="gallery">` line, and
   add one line per photo:

   ```html
   <a href="/images/NEW-PHOTO.jpg"><img loading="lazy" src="/images/NEW-PHOTO.jpg" alt="Fox Meadow Golden"></a>
   ```

   Tip: keep file names lowercase with no spaces (e.g. `spring-litter-01.jpg`).

## 3. Change contact info

Phone, email, and the Facebook link appear in the footer of every page and on
`contact.html`. Search for `585-729-8781`, `foxmeadowgoldens@gmail.com`, or the
Facebook URL and update as needed.

---

## Where the contact form goes

The "Send us a message" form uses **Netlify Forms**. After the site is live on
Netlify, go to **Netlify → your site → Forms → Settings → Form notifications** and
add an email notification to **foxmeadowgoldens@gmail.com** so you're emailed each
time someone writes in. Submissions are also saved in that Forms dashboard.

## Publishing changes

If the site is connected to GitHub (recommended), just commit your changes and
Netlify republishes automatically. Otherwise, drag this whole folder onto the
Netlify "Deploys" page to update it.
