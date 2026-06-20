# `.github` — OUNLP organization profile

This special repo powers the OUNLP org homepage at **https://github.com/ounlp**.

- [`profile/README.md`](profile/README.md) — the page GitHub renders at the top of the org.
- [`profile/assets/`](profile/assets/) — images for the profile (e.g. `banner.png`).
- [`.github/workflows/update-news.yml`](.github/workflows/update-news.yml) — daily job that
  refreshes the **Latest from the lab** list from `https://ounlp.org/feed.xml`.

## How GitHub uses this
A repo literally named `.github` with a `profile/README.md` is rendered as the organization's
public profile. Only org owners can create it. Editing `profile/README.md` updates the homepage.

## To finish setup (one-time, by an org owner)
1. Create a **public** repo named `.github` under the `ounlp` org and push this content.
2. (Optional) Add `profile/assets/banner.png` and uncomment the banner block in `profile/README.md`.
3. Set the org profile fields (Settings → Profile): display name **OUNLP**, a one-line
   description, URL **https://ounlp.org**, location **Norman, OK**, email **jie.cao@ou.edu**.
4. **Pin** the lab's best repos on the org page.
5. The news workflow runs daily; trigger it once via the Actions tab to populate the list.
