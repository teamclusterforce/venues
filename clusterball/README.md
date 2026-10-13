# Clusterball levels

The 21 levels of Clusterball (Daydream Software, 2000), converted to ClusterForce community maps
one to one: the original tracks, balls, goal, start and terrain, every original object with its
textures upscaled 8x (at most 2048 px), and the original ground colour map. Sky, sun, water and
weather come from ClusterForce, set to match each original level. The Tutorial level is left out;
it is a copy of Egypt.

These maps are not part of ClusterForce and are not shipped with the game. They will be offered
separately (a free Steam DLC or a download in the client).

## Contents

| Path | What it is |
|---|---|
| `maps/cb_<level>.cfmap` | One map per level (0.6 to 3.7 MB) |
| `basepack/textures/<name>.dds` | The 678 textures the maps share: BC7 with mip maps, named as the Clusterball artists named them (`bambooroof2`, `bergstoppar`); a name used for different pictures carries its level (`colormap_egypt`) |
| `basepack/pack.json` | Key, name and origin of the texture pack built from `basepack/` |

## Building the texture pack

The maps require the pack `clusterball_base` by its content hash
(`86bba4c3e17685194eddbeb3cf6e3f8eb45272f4af396a12ae7502ba2a52ad87`). It is built from
`basepack/` with the ClusterForce converter, bit for bit:

```
cbport packdir clusterball/basepack clusterball_base.cfpack
```

Put `clusterball_base.cfpack` next to the maps in the community map folder. Without it the maps
still play; the original objects are then drawn without textures.
