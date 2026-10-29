# MinimalisticGamers

Public contact, support, and shared privacy-policy website for MinimalisticGamers.

This organization site is owned by the `minimalisticgamers` GitHub organization and published from its `minimalisticgamers.github.io` repository.

## Stable URLs

- Website: https://minimalisticgamers.github.io/
- Support URL: https://minimalisticgamers.github.io/support/
- Privacy Policy URL: https://minimalisticgamers.github.io/privacy/
- Support email: contact@minimalisticgamers.io

Use the support and privacy URLs in each game's store listing and in-app links. The shared policy covers MinimalisticGamers games that link to it. Before releasing another game, verify that its actual data practices match the policy; update the policy first if they differ. The policy includes separate explanations for support emails, Apple diagnostics/TestFlight, and GitHub hosting.

## Hosting and editing

This is a standalone website repository, separate from game source. GitHub Pages publishes the root of `main`. `.nojekyll` enables direct static-file hosting. No build, dependencies, analytics, web fonts, server, form service, or API keys are needed.

- `index.html`: company home and contact links.
- `support/index.html`: support information for all games.
- `privacy/index.html`: shared policy, effective 29 October 2026.
- `styles.css`: responsive layout and print styles.
- `404.html`: missing-page fallback for the root site.
- `favicon.svg`: geometric M mark.

Preview from this directory:

```sh
python3 -m http.server 8787 --bind 127.0.0.1
```

Then visit http://127.0.0.1:8787/. Review mobile and desktop layouts, relative links, and email links before committing and pushing changes to `main`.

The site currently uses its GitHub Pages address. A custom domain can be configured later through GitHub Pages and the domain's DNS provider. This repository does not configure the domain or email delivery. If a custom domain is added, update canonical URLs and the absolute paths in `404.html`.
