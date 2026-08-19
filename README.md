# double_battles (Official mirror)

Installable releases of the **Double Battles** mod for [gen1recomp](https://github.com/bryanthaboi/gen1recomp).

Wild and trainer double battles: 1v2, 2v2 and trainer pairs, in classic, wide and 3D.

Grab the newest `.zip` from [Releases](https://github.com/shanehudson-gen1recomp-mods/double_battles/releases) and install it in-game: **MODS > Import mod .zip**. Installed copies get update checks through the launcher automatically.

Source code and issues live in the [mods monorepo](https://github.com/shanehudson-gen1recomp-mods/monorepo); this repo only hosts releases.

## Tested alongside

Third-party mods this release was run alongside, with the exact
versions used. Later versions of these mods may change behavior; if a
combo misbehaves, check the version you have against this list first.

| Mod | Version tested | Notes |
|---|---|---|
| [Dramatic Shape Voxel Mod](https://github.com/DramaticShape/DramaticShapeVoxelMod) | 1.6.2 | built-in scene detection plus the adapter composing both battlers into its billboard textures |
| Battle Art voxel fork | 1.7.6 | same scene detection path as Dramatic Shape |
| Gen1 Modern UI (`gen1_modern_ui`) | 0.8.3 | its battle cards name the right Pokémon through the slot borrow |
| [Crystal 251](https://github.com/Deftones565/gen1recomp-mod-crystal-251) (`CRYSTAL_251`) | 0.10.1 | compatibility developed against its source and covered by the headless suite, not yet play-tested. Its class-level battle patches (executeAction, TrainerAI, Status.residual, the battle.damage hook) all sit on paths our turn loop calls, partner battlers are announced for its per-battler stat attach, and its solitary legends stay 1v1. Known limit: its per-turn wild flee rolls do not run inside a double |

## All mods in this family

- **Double Battles** (`double_battles`, this repo): Wild and trainer double battles: 1v2, 2v2 and trainer pairs, in classic, wide and 3D.
- [Free Fly](https://github.com/shanehudson-gen1recomp-mods/free_fly) (`free_fly`): A party member that knows FLY can take off and free-roam over the overworld, then land anywhere walkable.
- [PMD Sky Sprites](https://github.com/shanehudson-gen1recomp-mods/pmd_sky_sprites) (`pmd_sky_sprites`): Wild flyers and your FLY mount wear species-true, 8-direction PMD animation sheets in the air. Ships community art only (PMDCollab SpriteCollab, CC BY-NC 4.0, credits included), which covers a small roster. For full coverage of all 251 species, supply your own game: drop a cartridge dump of Pokemon Mystery Dungeon: Explorers of Sky (US) - a .nds file - into this mod's folder and the official in-air animations are read straight off your cart while you play. In memory only: nothing official ships with the mod and nothing is extracted to disk. The IMPORT PMD setting turns cartridge reading off.
- [Wild Skies](https://github.com/shanehudson-gen1recomp-mods/wild_skies) (`wild_skies`): Ambient flying Pokémon from the local encounter table roam the sky in loose flocks, resting on streets and rooftops.
- [Dev Hook Inspector](https://github.com/shanehudson-gen1recomp-mods/dev-hook-inspector) (`dev-hook-inspector`): Developer tool: a HOOKS entry on the START menu lists every installed mod's public exports, engine-hook wraps and events.