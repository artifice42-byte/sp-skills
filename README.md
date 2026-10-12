# S&P Skill Editor (shared)

A browser-based editor for the Skills & Powers point-buy skill list, shared between collaborators through this repo.

- `index.html` – the editor (this is what you open)
- `skills.json` – the skill data (the one file you both edit)

Every save is a Git commit, so the **Commits** tab shows who changed what and you can roll back anything.

---

## One-time setup (the repo owner, ~15 min)

1. **Make a GitHub account** at github.com (free).
2. Click **+ → New repository**. Name it e.g. `sp-skills`, set it to **Public**, tick **Add a README**, click **Create repository**.
3. In the new repo click **Add file → Upload files**. Drag in `index.html` and `skills.json` from this package (you may also upload this README to replace the default one). Click **Commit changes**.
4. Go to **Settings → Pages**. Under *Build and deployment* choose **Deploy from a branch**, branch **main**, folder **/ (root)**, click **Save**. After ~1 minute GitHub shows your address:
   `https://YOUR-NAME.github.io/sp-skills/`
5. Go to **Settings → Collaborators → Add people** and invite your friend by their GitHub username.
6. Open your Pages address, click **☁ GitHub**, and follow the on-screen token steps (about 1 minute).
   Click **Save settings & test** – it should say "Connected as YOUR-NAME".

## One-time setup (your friend)

1. Make a free GitHub account, send the username to the owner.
2. Accept the invitation (email, or github.com/notifications).
3. Open the Pages address, click **☁ GitHub**, follow the token steps, **Save settings & test**.

## Everyday use (both of you)

1. Open the Pages address. It always loads the latest saved skills.
2. Click **🛠 Editor** to switch on editing. Change names, levels, costs, descriptions, prerequisites, add/disable/migrate skills.
3. Click **💾 Save to GitHub**. Done.

**If you both edited at once:** Save merges automatically as long as you changed different classes. If you both changed the *same* class, the editor warns you and asks whether to keep your version of it.

**To pick up your friend's latest work** without saving: refresh the page (it reloads from GitHub), or use **☁ GitHub → Reload from GitHub**. The browser warns before you close the tab with unsaved edits.

## Notes

- The token is stored only in your own browser. Revoke it any time at github.com/settings/tokens.
- GitHub Pages can take about a minute to show a new `index.html`, but skills data is read straight from the repo, so it is always current.
- `skills.json` is written with sorted keys and one skill per line so history diffs are readable.
- Editing `skills.json` by hand on github.com (pencil icon) also works; the editor will pick it up.
