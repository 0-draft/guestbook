# Guestbook

Leave a trace. If you visited, say hi. It takes 10 seconds.

[Sign the guest book](https://github.com/0-draft/guestbook/issues/new?template=guestbook.yml&title=%F0%9F%93%AE+%5BGuest+Book%5D). It opens a GitHub issue form with one field, and the message is added below automatically.

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
    <tr><td><code>2026-03-23</code></td><td><a href="https://github.com/kanywst">@kanywst</a></td><td><a href="https://github.com/kanywst/kanywst/issues/2">‼️</a></td></tr>
  </tbody>
</table>
<!-- GUESTBOOK:END -->

## How it works

`.github/workflows/guestbook.yml` runs whenever an issue is opened whose title starts with `📮 [Guest Book]`. It hands the issue to `scripts/update_guestbook.py`, which escapes the message, adds it to the table between the two markers above, and keeps the newest 20. The workflow commits the README and closes the issue.

Moved out of the [kanywst/kanywst](https://github.com/kanywst/kanywst) profile README on 2026-10-02, with the entries signed there.
