# BuyWorldZa — website photo library

Public mirror of the product/print photos used by buyworldza.co.za
(source of truth: `store/assets/` in the DEAS-Dropship-Test repo).

Why this repo exists
- The deployed site no longer has to carry ~37 MB of images through every build.
- GitHub raw + jsDelivr give free, cached, HTTPS hosting in front of them.
- The photos are versioned and diffable instead of living only on JP's D: drive.

URL patterns (repo root mirrors `store/assets/`)

    https://raw.githubusercontent.com/jpgreyling44/buyworldza-assets/main/<path>
    https://cdn.jsdelivr.net/gh/jpgreyling44/buyworldza-assets@main/<path>

Example: `art/aurora-arcs.webp` ->
`https://cdn.jsdelivr.net/gh/jpgreyling44/buyworldza-assets@main/art/aurora-arcs.webp`

Refreshing after a photo changes: commit + push here. Raw updates instantly;
jsDelivr caches for up to 12 h (purge with
`https://purge.jsdelivr.net/gh/jpgreyling44/buyworldza-assets@main/<path>`).
