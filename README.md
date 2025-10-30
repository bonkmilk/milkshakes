# Milshake Flavors (BlendOS Tracks)

* GNOME: `gnome`
* Plasma: `plasma`
* Cinnamon: `cinnamon`
* LXQT: `lxqt`
* MATE: `mate`
* XFCE: `xfce`
* Niri: `niri`

## Example Niri `/system.yaml` (vanilla)

```
repo: 'https://pkg-repo.blendos.co/'

impl: 'https://github.com/bonkmilk/milkshakes/raw/main'

track: 'niri'
```

## Example Niri `/system.yaml` with Caddy

```
repo: 'https://pkg-repo.blendos.co/'

impl: 'https://github.com/bonkmilk/milkshakes/raw/main'

track: 'milkshakes-base'

packages:
    - 'micro'
    - 'caddy'

services:
    - 'caddy'

package-repos:
    - name: 'chaotic-aur'
      repo-url: 'https://cdn-mirror.chaotic.cx/$repo/$arch'
```