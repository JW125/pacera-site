# pacera-site

Public support and privacy pages for **Pacera**, an iOS run and ride tracker
with a voice coach.

Two static pages, no build step, no dependencies, no third-party requests —
not even a webfont. A page explaining that the app doesn't phone home
shouldn't phone home.

| File | Serves |
|------|--------|
| `index.html` | Support page — the URL in App Store Connect's *Support URL* field |
| `privacy.html` | Privacy policy — the URL in App Store Connect's *Privacy Policy URL* field |
| `style.css` | Shared styles |

Published with GitHub Pages from `main`:

- Support: https://jw125.github.io/pacera-site/
- Privacy: https://jw125.github.io/pacera-site/privacy.html

## Keeping the policy honest

`privacy.html` must keep describing what the app actually does. The source of
truth is `docs/PRIVACY_POLICY.md` in the (private) app repo — change both
together. In particular, the three destinations in the ledger (xAI, OSRM +
Open-Meteo, Strava) are the complete list of places data can go. Adding any
network call to the app means adding a row here first.

The app source is kept in a separate private repository.
