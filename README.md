# Ghost Bear — Arma 3 Squad XML

## Files
- `squad.xml` — squad details and member roster
- `squad.dtd` — XML document type definition
- `logo.png` — supplied Ghost Bear emblem, 512×512 with transparency; **conversion required**

## Before uploading
1. Open `squad.xml` in a text editor and replace `REPLACE_WITH_STEAM64_ID` with your 17-digit Steam64 ID and `REPLACE_WITH_ARMA_PROFILE_NAME` with your exact Arma 3 profile nickname. Repeat the `<member>...</member>` block for additional players, using each player's own ID and nickname.
2. Use Bohemia Interactive's Arma 3 Tools / TexView2 to open `logo.png` and save it as **`logo.paa`**. Keep transparency. `logo.png` is **not** a replacement for `logo.paa`.
3. Upload `squad.xml`, `squad.dtd`, and the resulting `logo.paa` into the root of a public GitHub repository. The PNG and README are optional.
4. In repository Settings > Pages, deploy from `main` and `/(root)`.
5. After Pages publishes, verify `https://YOURUSERNAME.github.io/ghost-bear/squad.xml` loads, then enter that URL in the Arma 3 profile Squad URL field.

The `squad.xml` file points to `<picture>logo.paa</picture>`; the PAA must be in the same folder as the XML. Do not use the GitHub repository browser URL as your squad URL.
