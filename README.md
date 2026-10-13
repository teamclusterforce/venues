# ClusterForce community maps

Community maps for [ClusterForce](https://clusterforce.net): venues that are not part of the game
itself and are added by the player.

| Folder | Content |
|---|---|
| `clusterball/` | The 21 levels of the original Clusterball as ClusterForce maps |

## Planned

- **Build your own venues.** A track and venue editor is planned, so players can design their
  own maps for ClusterForce.
- **Steam Workshop.** Community maps are meant to be shared and subscribed to through the Steam
  Workshop, so they arrive in the game without any manual copying.

## Using a map today

A map is one `.cfmap` file; maps that share textures also need the texture pack they name. The
client loads both from its community map folder:

- `%APPDATA%\ClusterForce\Client\community_maps\` (the player's folder), or
- `community-maps\` next to `ClusterForce.exe`.
