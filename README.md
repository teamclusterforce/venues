# ClusterForce community maps

Community maps for [ClusterForce](https://clusterforce.net): venues that are not part of the game
itself and are added by the player.

| Folder | Content |
|---|---|
| `clusterball/` | The 21 levels of the original Clusterball as ClusterForce maps |

A map is one `.cfmap` file. A map whose objects use shared textures names a texture pack
(`.cfpack`) in its manifest; the client loads both from its community map folder:

- `%APPDATA%\ClusterForce\Client\community_maps\` (the player's folder), or
- `community-maps\` next to `ClusterForce.exe`.

Texture packs are build outputs and are not stored here; this repository holds their sources.
