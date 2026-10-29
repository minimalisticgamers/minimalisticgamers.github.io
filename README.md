# MinimalisticGamers

Public game, contact, support, and shared privacy-policy website for MinimalisticGamers.

This organization site is owned by the `minimalisticgamers` GitHub organization and published from its `minimalisticgamers.github.io` repository.

## Stable URLs

- Website: https://minimalisticgamers.github.io/
- Wigmaker Workshop marketing URL: https://minimalisticgamers.github.io/wigmaker-workshop/
- A Quiet Ember marketing URL: https://minimalisticgamers.github.io/a-quiet-ember/
- A Quiet Ember support URL: https://minimalisticgamers.github.io/a-quiet-ember/support/
- A Quiet Ember privacy URL: https://minimalisticgamers.github.io/a-quiet-ember/privacy/
- A Quiet Ember source URL: https://minimalisticgamers.github.io/a-quiet-ember/source/
- Support URL: https://minimalisticgamers.github.io/support/
- Privacy Policy URL: https://minimalisticgamers.github.io/privacy/
- Public support tracker: https://github.com/minimalisticgamers/minimalisticgamers.github.io/issues

Use the support and privacy URLs in each game's store listing and in-app links. The shared policy explicitly covers Wigmaker Workshop (`com.skylar.wigmaker`), A Quiet Ember (`com.skylar.adarkroom`), and other MinimalisticGamers games that link to it. A Quiet Ember also has a dedicated app policy. Before releasing another game, verify that its actual data practices match the policy; update the policy first if they differ. The policy includes separate explanations for public GitHub support posts, Apple diagnostics/TestFlight, and GitHub hosting.

GitHub Issues is enabled for this repository. Support requires a GitHub account and posts are public. Keep personal contact details out of the website and support posts. The site does not advertise an email address or imply that a support mailbox is configured.

## Hosting and editing

This is a standalone website repository, separate from game source. GitHub Pages publishes the root of `main`. `.nojekyll` enables direct static-file hosting. No build, dependencies, analytics, web fonts, server, form service, or API keys are needed.

- `index.html`: company home and contact links.
- `wigmaker-workshop/index.html`: dedicated game marketing page, with screenshots, features, release status, and original-creator attribution.
- `wigmaker-workshop/workshop.css` and `assets/`: game-page styles and optimized copies of the existing game artwork and screenshots.
- `a-quiet-ember/`: dedicated adventure marketing page, app support, privacy, corresponding source and license.
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

## A Quiet Ember

The dedicated A Quiet Ember page identifies this as an independent adaptation of the open-source A Dark Room browser game by Michael Townsend, doublespeak games, and contributors. It is separate from the official mobile edition. Keep that attribution, the MPL 2.0 license and dependency notices with the corresponding source. Do not imply original-creator endorsement.

The public game is still in preparation. There is no public App Store link or open TestFlight invite. The site describes offline play accurately, including local saves, user-selected backup export/import, and no added catch-up production when the app is closed. Later-game screenshots use isolated demonstration saves rather than an earned playthrough; the public gallery describes them as different stages of play.

The source page offers a selected source archive for the native app and vendored game. It excludes `.git`, internal account/review records, signing credentials, build artifacts, and private review/contact details. Original upstream author and license notices remain intact. Regenerate it after final native candidate changes with `ADarkRoom/Publication/package_public_source.py`, passing the intended version/build. The public `source-manifest.json` records included file hashes and the archive hash.

The currently prepared source ZIP is for the immutable **A Quiet Ember 1.0 (3)** candidate. It contains 251 source files, including 25 preferred editable translations, and has SHA-256 `7367021c7f02ca8623df6956ea0f3668439a6b185b7666ad5e8f366710f976f9`. Packaging checked its local adapters/notices and all Vendor bytes against the signed build 3 archive.
