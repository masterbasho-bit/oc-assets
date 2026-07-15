# oc-assets

Image mirror / backup host for the **outsidecontext.com** dispatch pages
(WordPress "Code Block" pages for Basho's Art, Book, and Film products).

These are the same images served from the project Vercel deploys. They are
mirrored here so the live pages have a durable second source: each `<img>` on
the pages carries an `onerror` fallback that swaps to the matching raw URL here
if the Vercel deploy ever changes, is renamed, or goes offline.

```
artsales/…   <- artsales-masterbasho-9526s-projects.vercel.app/…
booksales/…  <- booksales.vercel.app/…
filmsales/…  <- filmsales.vercel.app/…
```

Raw URL pattern:
`https://raw.githubusercontent.com/masterbasho-bit/oc-assets/main/<deploy>/<path>`

Long-term, these can be replaced by uploads to the WordPress media library.
