# blendOS Tracks

* GNOME: `gnome`
* Plasma: `plasma`
* Cinnamon: `cinnamon`
* LXQT: `lxqt`
* MATE: `mate`
* XFCE: `xfce`
* Cosmic: `cosmic`

## Example GNOME `/system.yaml` (vanilla)

```
repo: 'https://pkg-repo.blendos.co/'

impl: 'https://github.com/blend-os/tracks/raw/main'

track: 'gnome'
```

## Example GNOME `/system.yaml` with Caddy

```
repo: 'https://pkg-repo.blendos.co/'

impl: 'https://github.com/blend-os/tracks/raw/main'

track: 'gnome'

packages:
    - 'micro'
    - 'caddy'

services:
    - 'caddy'

package-repos:
    - name: 'chaotic-aur'
      repo-url: 'https://cdn-mirror.chaotic.cx/$repo/$arch'
```
