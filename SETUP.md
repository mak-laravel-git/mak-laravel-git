# Set up the maktech Laravel GitHub profile

## Recommended account details

- **GitHub username:** Keep `mak-laravel-git` (existing GitHub Apps and automation use this identity).
- **Profile display name:** `maktech | Laravel Engineering`
- **Short bio:** `Laravel engineering at maktech • PHP, React, Inertia.js, Next.js & Tailwind CSS • Building production-ready web applications.`
- **Profile image:** `assets/laravel-avatar.png` (set separately under GitHub account profile settings).

## Make the README appear on your public profile

GitHub profile README requires a **PUBLIC** repository named **exactly** the same as the username, with a `README.md` at the repository root.

1. Sign into the GitHub personal account `mak-laravel-git`.
2. Create a **public repository named `mak-laravel-git`** at `https://github.com/new` (or open the existing one if it already exists).
3. Upload the `README.md` file from this package to the repository root.
4. Upload the entire `assets/` folder preserving its filenames and relative paths.
5. Commit the files to the default branch.
6. Open `https://github.com/mak-laravel-git` to see the profile README.
7. Under account Settings → Public profile, set your profile name, bio, and upload `assets/laravel-avatar.png` as your avatar.

**Do NOT** upload this to `mak-laravel-git-manage` if you want it displayed automatically on the account profile; that is a normal project repository, not the special profile repository.

## Example folder layout

```
mak-laravel-git/
├── README.md
└── assets/
    ├── profile-banner.png
    ├── laravel-avatar.png
    └── tech-stack.png
```

## Git command option

If the special profile repository already exists, clone it to a local folder and copy README.md and assets/ into the clone:

```bash
git clone https://github.com/mak-laravel-git/mak-laravel-git.git
cd mak-laravel-git
# Copy README.md and assets/ from this package here.
git add README.md assets/
git commit -m "Add maktech Laravel engineering profile"
git push
```

## Notes

- The profile README and included assets are public. No credentials, private repositories, or sensitive endpoint details are embedded.
- The banner and tech-stack image render from local files; they do not depend on an external image host.
- The avatar has a transparent background and can be uploaded in your GitHub profile settings.
- Keep your existing GitHub **username** unchanged unless you are prepared to review integrations, app installations, automation, and configured repository owner names.
