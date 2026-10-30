# HSS / HWU Save Editor

This is my High School Story (HSS) and Hollywood U (HWU) save editor. It is web-based and all files are processed entirely locally. It is still in beta, and may not always function correctly. Always keep a backup of your save file in a safe place in the case of corruption.

## Editor capabilities

- Detects HSS and HWU save profiles and applies the matching visual theme.
- Decrypts and re-encrypts saves in-browser, with protobuf parsing that retains unknown fields.
- Includes quick resource fields, editable raw save data, undo/revert, search, save summary, classmates, campus buildings and plots, and relationships.

## How to use the editor

First, you want to use the BACKUP / RESTORE menu in your HSS / HWU Restoration apk to export a copy of your save file.

Visit this link:
**https://muttupnable.github.io/hss-hwu-save-editor/**

The first page you see, there is a box to upload your save file too. Select this and it will open a file picker, or if you are on PC you can drag the file directly over the box.

You will then be taken to the save editor and analysis page where you will find menus and buttons to change your save data with. Have fun and always ensure to keep your original backup safe and untouched!

The root `index.html` is the editor. Its HSS and HWU art and interface files are served from the relative `assets/` directories.

## Privacy and security

- Save files are selected, read, parsed, edited, and re-encrypted locally in the visitor's browser. The site has no backend and does not upload save files.
- The editor uses the browser Web Crypto API. Mobile browsers generally require a secure context; the HTTPS GitHub Pages URL provides one. Mobile file selection and downloads can still vary by browser and have not been device-tested.
- This is a public static site. All HTML and JavaScript are downloadable and inspectable, including any encryption keys embedded in the editor source. Those keys are not secret.
- Keep an untouched backup and edit only copies. A successful download does not prove a game will accept the edited save.

See [index.html](index.html) for the complete client-side implementation.
