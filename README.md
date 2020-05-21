# ytmdesktop-adblock

## No longer updated.
I've moved on to a native app that Chrome provides. Feel free to fork and keep up with upstream if needed.

---

A fork of [ytmdesktop](https://github.com/ytmdesktop/ytmdesktop) with added adblocker from [cliqz-oss/adblocker](https://github.com/cliqz-oss/adblocker).
No promises on keeping up with upstream.

### Installation instructions

If you have access to AUR, you can install `ytmdesktop-git` package after editing PKGBUILD file.
Steps for `yay` (my choice of AUR package manager) look like this:

- `yay --editmenu -S ytmdesktop-git`
- When you're asked "PGKBUILDS to edit?", type `A` to select All. This will open PKGBUILD in your default editor.
- In PKGBUILD file find line starting with `source=` (around 16th line) and change it from <br> `'git+https://github.com/`**`ytmdesktop`**`/ytmdesktop.git'` <br> to <br> `'git+https://github.com/`**`margiris`**`/ytmdesktop.git'` <br> (this simply changes sources from original to this repository).
- Save and close PKGBUILD.
- Proceed with installation.

On Windows, MacOS and Linux distros without AUR it's currently only possible to run this program with `nmp`, since I don't have time to build binaries.

```language:bash
# Clone and go to this repository
git clone https://github.com/margiris/ytmdesktop && cd ytmdesktop
# Install dependencies
npm install

# Run the app
npm start
```
