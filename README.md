# Roblox Starter

Lightweight source and asset workspace for the next development session. No gameplay systems are implemented yet.

## Folders

| Path | Purpose / Roblox Studio location |
| --- | --- |
| `src/server/systems/` | Server-owned gameplay systems; ServerScriptService |
| `src/client/systems/` | Input, camera, UI, and effects; StarterPlayerScripts |
| `src/shared/` | Shared modules and configuration; ReplicatedStorage |
| `assets/models/` | Model exports (.rbxm / .rbxmx) |
| `assets/images/` | UI images and textures |
| `assets/audio/` | Sound source files |

## Next session

1. Open or create the experience in Roblox Studio.
2. Add one system at a time in the matching source folder.
3. Copy scripts into the Studio locations above and test with Play. This repository does not auto-sync with Studio; Rojo can be added later if needed.
4. Commit working changes with a short description.

Use `.server.luau` for server Scripts, `.client.luau` for LocalScripts, and `.luau` for ModuleScripts. Keep authoritative gameplay checks on the server. Shared code is visible to clients.

The `.gitkeep` files preserve empty folders and can be removed once those folders contain real files. Keep intentional place/model exports in version control; put generated builds in `build/` or `dist/`. Only commit assets you have permission to use, and never commit credentials.
