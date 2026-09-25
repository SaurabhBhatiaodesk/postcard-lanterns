# Postcard Lanterns wholesale page

The supplied HTML is split into nine independent sections. Every section contains its own scoped CSS, settings and Theme Editor preset. No shared CSS, JavaScript library or original `support.js` is required.

| File | Content |
| --- | --- |
| `sections/pl-header.liquid` | Sticky wholesale navigation |
| `sections/pl-hero.liquid` | Split heading, calls to action and image |
| `sections/pl-about.liquid` | About copy |
| `sections/pl-collection-heading.liquid` | Collection introduction |
| `sections/pl-products.liquid` | Reorderable lantern cards; seven supplied designs |
| `sections/pl-steps.liquid` | Three wholesale steps |
| `sections/pl-login.liquid` | Login banner |
| `sections/pl-registration.liquid` | Registration calls to action |
| `sections/pl-footer.liquid` | Wholesale footer |

## Installation

1. Upload the nine section files and `templates/page.boco.json` to the theme.
2. The homepage keeps the main store design. In Shopify admin, create a page (for example **BoCo**) and choose the **boco** template. On that page `layout/theme.liquid` hides the main header group and the page shows its own PL Wholesale header; the main footer stays. (`page.postcard-wholesale` with its own layout is still available as an alternative.)
3. Open that page in the Theme Editor. Each section appears separately with a **PL** prefix and can be edited or reordered. The alternate layout supplies only the reference page's header and footer, avoiding duplicate theme navigation.
4. Select the hero image and each lantern image. The source references seven local JPEGs which were not included with the HTML. Until images are selected, Shopify placeholders appear. Product blocks can optionally use a selected Shopify product's featured image.
5. Review login/application URLs, replace the footer contact placeholder and adjust the collection's design-count text if cards are added or removed. Defaults retain the client's `mybocohome.com` wholesale URLs.

Sections also work independently in existing JSON templates. Each section owns its typography and CSS. The font defaults to Assistant. Product grid columns are configurable from two to four on desktop, two on tablet and one on small phones.

## Functional scope

This is the supplied gated catalogue design. Frame selectors allow the same White/Black selection as the reference; they are not cart forms and do not select Shopify variant IDs. The Boulder card is White only. These sections do not authorize customers, expose prices or implement wholesale checkout. Approval, trade prices and ordering remain the responsibility of the store's wholesale integration. Application and login buttons link to that workflow.

The HTML's editor-only about-copy note is omitted. Its supplied fallback about copy is editable. No live store changes or theme publication are performed by this conversion.
