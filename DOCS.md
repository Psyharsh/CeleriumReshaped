# Content Table
- [Overview](#overview)
- [Installation](#installation)
- [How to add your own files](#how-to-add-your-own-files)
- [Troubleshooting](#troubleshooting)
- [Included Mods - What They Do](#how-mods-work)

## Overview
This is Documentation for Celerium: Reshaped. \
In this document, you can find:
- Info about the modpack itself
- Support for some problems;
- Things that are useful to know;
- Optional mods

---

## Installation

### Manual Installation (Advanced)

This modpack is designed to be installed using a **modpack-aware launcher** such as the **Modrinth App**, **SKLauncher** or **Prism Launcher**.

Manual installation using the **official Minecraft Launcher** is possible, but **not officially supported**, as it does not handle mod dependencies or updates automatically.

If you choose to install manually:
- You are responsible for keeping mods and configs up to date
- Updates must be applied manually
- Support may be limited if issues arise from manual setup

For the best experience and easiest updates, using a supported launcher is strongly recommended.

### Modrinth App (Recommended)

The **Modrinth App** provides the easiest and most reliable way to install this modpack.

1. Install the Modrinth App
2. Search for the `Celerium: Reshaped` modpack on Modrinth
3. Click **Install**
4. Launch the instance once installation is complete

This method automatically handles:
- Mod downloads and dependencies
- Configuration files
- Updates

### Prism Launcher

**Prism Launcher** is a powerful multi-instance launcher suitable for advanced users.

1. Install Prism Launcher
2. Add a new instance \
  2A. Search for the `Celerium: Reshaped` in the Modrinth tab, and choose the version you want
  2B. Import the modpack using the provided `.mrpack` file of your choice
3. Launch the instance after installation finishes

Prism Launcher allows full control over:
- Java versions
- Memory allocation
- Per-instance settings

### SKLauncher

**SKLauncher** supports importing modpacks using both `.zip` and `.mrpack` formats.

1. Open SKLauncher
2. Go to **Modpacks**
3. Click **Import modpack**
4. Select the modpack `.zip` or `.mrpack` file
5. Wait for the import process to complete
6. Launch the modpack from the installation list

While SKLauncher supports modpack importing:
- Dependency handling may vary depending on the pack
- The pack does **not** update automatically
- Some issues may be harder to reproduce compared to modpack-focused launchers

For the most reliable experience and update support, a modpack-aware launcher such as the **Modrinth App** or **Prism Launcher** is recommended. \

---

## How to add your own files
To add your own files is simple, actually.
1. Go to .minecraft at `C:\Users\[YOUR USER]\AppData\Roaming\.minecraft`
2. If you installed the modpack through a launcher go to A, but if installation was mannual, go to B. \
   2A. In the folder, you will find another folder called ´modpacks´, open that and try to find the folder for Celerium, after you find it, you will have several folders like "mods", "resourcepacks", "shaderpacks", etc. \
   2B. In the folder you will find folders like "mods", "resourcepacks", "shaderpacks", etc.
3. For shaders you put them in the "shaderpacks" folder, resource packs in the "resourcepacks" folder, all of them have their respective folders.
4. Normally, you need a .zip file to put a respective thing in their folder. (Ex.: ComplementaryShaders, SimpleCraft, Fresh Animations, NoisiumForked, etc).
5. Put the .zip file in its respective folder and open the game to test it
  5A. For shader packs, you need to put Iris yourself.

---

## Troubleshooting

If you experience issues while using Reshaped, follow the steps below. Most problems can be resolved with simple adjustments.

### GPU Crashes on Older Intel Integrated Graphics

Some older Intel iGPUs (e.g. Bay Trail, HD 3000/4000) may experience crashes or driver resets when using advanced rendering features.

**Solutions**
- In Sodium:
  - Set **Chunk Updates** to **Deferred**
  - Disable **Persistent Mapping**
- Use **Fast** graphics settings
- Consider switching to Linux (Mesa drivers tend to be more stable for older Intel GPUs
but do **NOT** if you don't understand how to change Operating Systems, research first.)

### High ms/t or Delayed Actions

**Symptoms**:

- Block breaking delay
- Mobs reacting slowly
- High ms/t in debug screen

**Solutions**:

- Get AFK for a while to let chunk generation catch up
- Lower Simulation Distance
- Reduce Render Distance
- Close background applications

### Stuttering When Exploring

**Symptoms**:

- Lag spikes while moving into new terrain
- Microstutters during chunk loading

**Solutions**:

- Set Chunk Builder Threads to 1 (low-end CPUs)
- Lower render distance
- Disable optional performance mods if instability appears
- Ensure sufficient RAM allocation (2–4 GB recommended, but do not allocate almost all of your RAM, that is not recommended ever.)

### Low FPS

**Solutions**:
If you are using Core, consider switching to Lite, it has the same mod list but has more optimized settings! \
But if you're already using Lite, Minimal might be your go-to. \
If Minimal also doesn't help that much, you will have to start digging into the settings. Be careful though! \

### Visual Popping / Missing Entities

**Cause**:

- Culling optimizations

**Solutions**:

- Adjust settings in culling mods
- Reduce aggressiveness of culling through the options of Entity Culling and MoreCulling

### Game Crashes on Launch

**Solutions**:

- Ensure all mods installed correctly (reinstall pack if needed)
- Update graphics drivers
- Remove recently added optional mods
- Check logs for mod conflicts
### Optional Mods Causing Issues

**Symptoms**:

- Instability after enabling optional mods

**Solutions**:

- Disable recently added optional mods
- Add optional mods one at a time
- Prefer the default configuration for maximum stability

---

## Included Mods – What They Do <a name="how-mods-work"></a>

Reshaped is built on a carefully selected set of mods, each chosen for a specific purpose.
Every mod contributes to performance, stability, or usability—nothing is included without reason.

### Performance Engine

These mods form the core of Reshaped’s optimization system:

- **Sodium** – Replaces the rendering engine for massive performance improvements
- **Sodium Extra** – Adds additional settings and fine-tuning options for Sodium.
- **Lithium** – Optimizes game logic and server-side performance
- **FerriteCore** – Reduces memory usage
- **ModernFix (mVUS)** – Applies a wide range of performance and bug fixes
- **ImmediatelyFast** – Speeds up UI and rendering paths
- **EntityCulling** – Skips rendering hidden entities
- **MoreCulling** – Reduces unnecessary block rendering
- **Krypton** – Improves networking performance (works best when installed in a server)
- **Dynamic FPS** – Reduces resource usage when the game is unfocused
- **Exordium** – Optimizes UI rendering
- **Let Me Despawn** – Improves entity despawn behavior
- **Clumps** – Groups XP orbs to reduce lag
- **Alternate Current** – Optimizes redstone updates
- **LazyDFU Reloaded** – Speeds up game startup by deferring DataFixerUpper initialization.
- **ThreadTweak** – Adjusts thread priorities to improve performance and responsiveness on some systems.

### Stability & Fixes

These mods improve reliability and correct vanilla issues:

- **Debugify** – Fixes vanilla bugs
- **FastQuit** – Speeds up world exit and reduces hang time
- **YOSBR** – Ensures consistent configuration behavior
- **No Telemetry** – Disables Microsoft telemetry and data collection.

### Essential Quality of Life

Lightweight improvements that do not impact performance:

- **Shulker Box Tooltip** – View contents without opening
- **Better F3** – Enhanced debug screen
- **Block Entity Render Distance** – Controls rendering range for block entities
- **AppleSkin** – Displays hunger and saturation information directly in the HUD.
- **Longer Chat History** – Increases the amount of messages stored in chat history.

### Core Libraries

Required dependencies for the mod ecosystem:

- **Fabric API**
- **Fabric Language Kotlin**
- **Cloth Config**
- **YACL (Yet Another Config Lib)**
- **Mod Menu**
- **LibIPN**
- **Almanac**

Optional Mods

Reshaped includes a selection of optional mods that can be enabled during installation.
These are not required for the core experience, but allow you to customize the pack to your preferences.

> The core pack remains stable and optimized without them. Which explains why they are not present in Minimal.

### Visual Enhancements

Mods that improve visuals and immersion:

- **Hold My Items** – Improves item handling visuals
- **LambDynamicLights** – Adds dynamic lighting from held light sources
- **Chat Heads** – Displays player heads in chat

These mods may reduce performance on lower-end systems.

### Quality of Life

Optional usability improvements:

- **Inventory Profiles Next** – Advanced inventory sorting and management
- **Better Mount HUD** – Improves mount-related UI
- **Bridging Mod** – Enhances block placement for bridging

> Some QoL mods may not be allowed on certain servers.

### Shader Support

Optional support for advanced graphics:

- **Sodium Core Shader Support** – Enables resourcepacks to be able to replace sodium's shaders, similar to resourcepacks being able to replace vanilla's core shaders.
- **Iris** – Iris – Provides shader support while preserving the performance benefits of Sodium. (You have to manually add this, though.)

Required only if you plan to use shaders.
