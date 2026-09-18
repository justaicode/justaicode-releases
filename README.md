# justaicode releases

Public download channel for the apps at [justaicode.app](https://justaicode.app) that have no other release channel. Application source stays in its own private repository.

Each app publishes a GitHub Release tagged `<app>-v<version>` with its installer, and keeps a small `<app>/latest.json` on `main` that the download page reads. Nothing here is edited by hand: `publish.sh` in the site repository builds both.

| App id | What | Reads |
|---|---|---|
| `ekybe-mac` | Ekybe for macOS (Developer ID signed, notarized ZIP) | `ekybe-mac/latest.json` |
| `chevio-mac` | Chevio for macOS (Developer ID signed, notarized ZIP) | `chevio-mac/latest.json` |

Install: unzip, move the app into Applications, open it. macOS checks the notarization ticket on first launch.
