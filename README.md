# Guestbook

> [!WARNING]
> **Retired on 2026-11-08, to be archived on or after 2026-12-08.** Nobody but the author has ever signed it, here or in the profile README it started in. Its workflow is disabled, so a new entry is no longer added to the book.

A guest book that visitors signed by opening a GitHub issue form with one field; the message was added below automatically. The entries are kept as they stood when it was retired.

<!-- GUESTBOOK:START -->
<table align="center">
  <thead>
    <tr>
      <th>🕐</th>
      <th>👤</th>
      <th>💬</th>
    </tr>
  </thead>
  <tbody>
    <tr><td><code>2026-10-14</code></td><td><a href="https://github.com/kanywst">@kanywst</a></td><td><a href="https://github.com/0-draft/guestbook/issues/5">workflow no longer hardcodes the repo or branch</a></td></tr>
    <tr><td><code>2026-10-14</code></td><td><a href="https://github.com/kanywst">@kanywst</a></td><td><a href="https://github.com/0-draft/guestbook/issues/3">smoke test after the move to 0-draft 👋</a></td></tr>
    <tr><td><code>2026-03-23</code></td><td><a href="https://github.com/kanywst">@kanywst</a></td><td><a href="https://github.com/kanywst/kanywst/issues/2">‼️</a></td></tr>
  </tbody>
</table>
<!-- GUESTBOOK:END -->

## How it works

`.github/workflows/guestbook.yml` runs whenever an issue is opened whose title starts with `📮 [Guest Book]`. It hands the issue to `scripts/update_guestbook.py`, which escapes the message, adds it to the table between the two markers above, and keeps the newest 20. The workflow commits the README and closes the issue.

## Your own

Copy these three files into your repository, your profile repository included:

- `.github/workflows/guestbook.yml`
- `.github/ISSUE_TEMPLATE/guestbook.yml`
- `scripts/update_guestbook.py`

Then put the two markers where the table should go in your README, with a sign link above them that points at your repository:

```markdown
[Sign the guest book](https://github.com/OWNER/REPO/issues/new?template=guestbook.yml&title=%F0%9F%93%AE+%5BGuest+Book%5D)

<!-- GUESTBOOK:START -->
<!-- GUESTBOOK:END -->
```

The first entry fills in the table.

Moved out of the [kanywst/kanywst](https://github.com/kanywst/kanywst) profile README on 2026-10-02, with the entries signed there.
