# pacera-site

Public support and privacy pages for **Pacera**, an iOS run and ride tracker
with a voice coach.

Support and privacy stay third-party-free (no webfonts). The roads map loads
OpenStreetMap tiles and Leaflet so the survey can actually be a map.

| File | Serves |
|------|--------|
| `index.html` | Support page — the URL in App Store Connect's *Support URL* field |
| `privacy.html` | Privacy policy — the URL in App Store Connect's *Privacy Policy URL* field |
| `style.css` | Shared styles |
| `roads/index.html` | Public pavement survey |
| `roadsense-data.json` | Grid cells + jar pins, updated from the app |

Published with GitHub Pages from `main`:

- Support: https://jw125.github.io/pacera-site/
- Privacy: https://jw125.github.io/pacera-site/privacy.html
- Roads: https://jw125.github.io/pacera-site/roads/

## Keeping the policy honest

`privacy.html` must keep describing what the app actually does. The source of
truth is `docs/PRIVACY_POLICY.md` in the (private) app repo — change both
together. Destinations in the ledger (xAI, OSRM + Open-Meteo, Strava, and
optional GitHub Pages for the road map) are the complete list of places data
can go. Adding any network call to the app means adding a row here first.

The app source is kept in a separate private repository.
