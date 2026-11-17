# Fast Dynamic Trees

This Minecraft 1.21.1 fork preserves Dynamic Trees' registry IDs, world generation,
tree cutting and compatibility with existing tree packs, while reducing ongoing
forest simulation. It is meant to **replace**, not accompany, Dynamic Trees.

The `trees.staticTrees` server config is enabled by default:

- Rooty soil, dynamic leaves and saplings no longer receive random growth ticks.
- Existing canopies do not regrow leaves after they are removed.
- Voluntary seed spreading and autonomous seed planting are disabled.
- World-generated trees still produce complete canopies; structural leaf decay
  on neighbor updates and falling-tree behavior remain enabled.
- Players can still obtain seeds and grow saplings using bonemeal.

Turn `trees.staticTrees` off to restore upstream growth behavior. Existing
`dynamictrees` world and addon IDs are intentionally unchanged.

---

## Upstream Dynamic Trees

Minecraft Forge mod providing dynamic trees that progressively grow from seed to maturity.

![Logo](./header.png)

This branch is for the 1.21.1 version of Minecraft.

### Links
- [CurseForge](https://www.curseforge.com/minecraft/mc-mods/dynamictrees)
- [Modrinth](https://modrinth.com/mod/dynamictrees)
- [Discord](https://discord.gg/A4FCBS3)

### Compiling
* Clone the repository.
* Open a command prompt/terminal to the repository directory.
* Run `gradlew build` on Windows, or `./gradlew build` for MacOS or Linux.
* The built jar file will be in `build/libs/`.
