# chillalabs Flatpak repository

Flatpak builds of chillalabs apps, served by GitHub Pages at
<https://chillalabs.github.io/flatpak/>.

## Install 2fip

```sh
flatpak install --user https://chillalabs.github.io/flatpak/2fip.flatpakref
```

Updates then come with `flatpak update`. The runtime is installed from Flathub
automatically.

To add the repository by itself:

```sh
flatpak remote-add --user --if-not-exists chillalabs https://chillalabs.github.io/flatpak/chillalabs.flatpakrepo
```

## Contents

- `repo/` — the OSTree repository (signed with the key in `chillalabs.gpg`,
  fingerprint `B8DB 59C9 D8DE 325B ED44  7464 D0A0 9A1D 8E8E DB64`)
- `2fip.flatpakref`, `chillalabs.flatpakrepo` — install and remote files

Built and published from [chillalabs/twofip](https://github.com/chillalabs/twofip)
with `just flatpak-publish`.
