# uBlockFilters

My personal collection of additional [uBlock Origin](https://github.com/gorhill/uBlock) filters: mostly cosmetic tweaks to remove clutter and annoyances on sites I use daily (YouTube, Reddit, Proton Mail, and a few Italian sites).

## Subscribe

In uBlock Origin: Settings, Filter lists, Import, then paste:

```
https://raw.githubusercontent.com/dnlprn/uBlockFilters/main/uBlockAdditionalFilters.txt
```

## What's in here

- **YouTube**: hides end screens, info cards, homepage shelves (posts, mixes), "People also search for", hover previews; packs thumbnails 6 per row
- **Reddit**: hides recent/sidebar sections and posts matching certain keywords
- **Misc**: eBay.it recommendations, Proton Mail info banners, clutter on a couple of Italian sites

## Notes

- Some selectors target site markup that changes often (especially YouTube and Proton Mail). If something stops being hidden, it's likely the site changed its classes, not uBO.
- Keyword rules on Reddit are intentionally aggressive; `:has-text()` matches any text inside a post card.
