# MinimalisticGamers

Public game, contact, support, and shared privacy-policy website for MinimalisticGamers.

This organization site is owned by the `minimalisticgamers` GitHub organization and published from its `minimalisticgamers.github.io` repository.

## Stable URLs

- Website: https://minimalisticgamers.github.io/
- Wigmaker Workshop marketing URL: https://minimalisticgamers.github.io/wigmaker-workshop/
- Support URL: https://minimalisticgamers.github.io/support/
- Privacy Policy URL: https://minimalisticgamers.github.io/privacy/
- Public support tracker: https://github.com/minimalisticgamers/minimalisticgamers.github.io/issues

Use the support and privacy URLs in each game's store listing and in-app links. The shared policy explicitly covers Wigmaker Workshop (`com.skylar.wigmaker`) and other MinimalisticGamers games that link to it. Before releasing another game, verify that its actual data practices match the policy; update the policy first if they differ. The policy includes separate explanations for public GitHub support posts, Apple diagnostics/TestFlight, and GitHub hosting.

GitHub Issues is enabled for this repository. Support requires a GitHub account and posts are public. Keep personal contact details out of the website and support posts. The site does not advertise an email address or imply that a support mailbox is configured.

## Hosting and editing

This is a standalone website repository, separate from game source. GitHub Pages publishes the root of `main`. `.nojekyll` enables direct static-file hosting. No build, dependencies, analytics, web fonts, server, form service, or API keys are needed.

- `index.html`: company home and contact links.
- `wigmaker-workshop/index.html`: dedicated game marketing page, with screenshots, features, release status, and original-creator attribution.
- `wigmaker-workshop/workshop.css` and `assets/`: game-page styles and optimized copies of the existing game artwork and screenshots.
- `support/index.html`: support information for all games.
- `privacy/index.html`: shared policy, effective 29 October 2026.
- `styles.css`: responsive layout and print styles.
- `404.html`: missing-page fallback for the root site.
- `favicon.svg`: geometric M mark.
- `sitemap.xml` and `robots.txt`: public page discovery.

The game page currently says “Coming to iPhone and iPad.” Once the app is publicly released, replace the coming-soon messaging with the verified App Store link. Do not advertise a public download or TestFlight invitation before one exists. Production runs during play, not while the app is closed. Keep the original Wigmaker / Andy Wilson / redgem.games attribution.

The game screenshots and artwork are resized copies from the Wigmaker project's accepted App Store submission assets. No gameplay UI was repainted. Social-sharing metadata uses an absolute, public image URL. The game page can be entered as the Marketing URL in App Store Connect; the shared support and privacy URLs stay separate.

Preview from this directory:

```sh
python3 -m http.server 8787 --bind 127.0.0.1
```

Then visit http://127.0.0.1:8787/. Review mobile and desktop layouts, relative links, and the public support link before committing and pushing changes to `main`.

The site currently uses its GitHub Pages address. A custom domain can be configured later through GitHub Pages and the domain's DNS provider. This repository does not configure the domain or email delivery. If a custom domain is added, update canonical URLs and the absolute paths in `404.html`.
