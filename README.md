# HSS / HWU Save Editor

This repository hosts the browser-based High School Story (HSS) and Hollywood U (HWU) save editor as a static GitHub Pages site.

## Open the editor

After the first successful Pages deployment, visit:

**https://muttupnable.github.io/hss-hwu-save-editor/**

The root `index.html` is the editor. Its HSS and HWU art and interface files are served from the relative `assets/` directories.

## GitHub Pages deployment

The workflow in `.github/workflows/pages.yml` deploys the repository root to GitHub Pages after every push to `main`. It can also be started manually from the repository's **Actions** tab using **Deploy static site to GitHub Pages**.

For a new fork, enable **Settings → Pages → Build and deployment → Source: GitHub Actions**. The first deployment must complete successfully before the Pages URL is available. The workflow uses the official GitHub Pages actions and needs no application secrets, backend, package installation, or third-party runtime dependencies.

## Privacy and security

- Save files are selected, read, parsed, edited, and re-encrypted locally in the visitor's browser. The site has no backend and does not upload save files.
- The editor uses the browser Web Crypto API. Mobile browsers generally require a secure context; the HTTPS GitHub Pages URL provides one. Mobile file selection and downloads can still vary by browser and have not been device-tested.
- This is a public static site. All HTML and JavaScript are downloadable and inspectable, including any encryption keys embedded in the editor source. Those keys are not secret.
- Keep an untouched backup and edit only copies. A successful download does not prove a game will accept the edited save.

## Editor capabilities

- Detects HSS and HWU save profiles and applies the matching visual theme.
- Decrypts and re-encrypts saves in-browser, with protobuf parsing that retains unknown fields.
- Includes quick resource fields, editable raw save data, undo/revert, search, save summary, classmates, campus buildings and plots, and relationships.

See [ASSET_SOURCES.md](ASSET_SOURCES.md) for asset provenance and [index.html](index.html) for the complete client-side implementation.
