# VRstarter - Visitor v01

A Virtual Reality exploration project built with Unreal Engine 5.6, featuring immersive lake and canyon environments.

## Project Overview

**Visitor_v01** is a VR application designed for exploring natural environments including lakes, rivers, and canyons. The project leverages OpenXR for cross-platform VR support and includes interactive elements and realistic water systems.

## Technical Specifications

- **Engine Version**: Unreal Engine 5.6
- **VR Platform**: OpenXR (cross-platform)
- **Target Platforms**: Windows, Linux, Android, iOS, Mac, PlayStation, Xbox, Switch, VisionOS

## Features

### VR Support
- **OpenXR Integration** - Cross-platform VR compatibility
- **Eye Tracking** - OpenXREyeTracker plugin enabled
- **Hand Tracking** - OpenXRHandTracking for natural hand interactions
- **VR Spectator Mode** - Third-person viewing capability

### Environments

#### Lake Environment
- Custom 3D lake models (LAKE_01 through LAKE_04)
- Lake-specific materials and boat assets
- Water plane system with realistic lake water shader
- Rock and basalt environment props

#### Canyon/River Environment
- Large-scale canyon models (393MB+ assets)
- River water systems
- Boat navigation elements
- Custom canyon materials and textures

### Content Assets

#### 3D Models (`Content/3DMODELS/`)
- **LAKE_MISC**: Lake environments, boats, and associated materials
- **CANYONS_MISC**: Canyon terrain, boats, and related assets
- **x_MISC**: Interactive objects like envelopes

#### Characters (`Content/Characters/`)
- **MannequinsXR**: VR-optimized character models
  - Skeletal meshes for hands (Manny and Quinn variants)
  - Hand animations (grasp, point, thumb up, index curl)
  - Custom materials with chromatic effects

#### VR Template (`Content/VRTemplate/`)
- VR pawn system with teleportation
- Interactive blueprints (grabbable objects, doors, jump pads)
- Menu system with VR cursor
- Haptic feedback support
- Input mapping contexts for VR controllers

#### Water Systems (`Content/WaterPlane/`)
- **Lake Water**: Medium and small wave simulations
- **Ocean Water**: Large wave systems with foam effects
- **Translucent Water**: See-through water for shallow areas
- Custom HDRI environment lighting

#### Weapons (`Content/Weapons/`)
- Pistol with custom materials and animations
- Grenade launcher with projectile system
- Rifle with skeletal mesh support
- Weapon audio and haptic effects

#### Level Prototyping (`Content/LevelPrototyping/`)
- Interactable objects (doors, jump pads, targets)
- Prototyping materials and meshes
- Procedural grid materials

## Maps

- `VRTemplateMap.umap` - Default VR template scene
- `VR_LAKE_00.umap` - Lake exploration environment
- `VR_RIVER_00.umap` - River/canyon exploration environment
- `LakeWater_Example.umap` - Water shader demonstration
- `OceanWater_Example.umap` - Ocean system demonstration
- `TranslucentWater_Example.umap` - Shallow water demonstration

## Asset Management

This repository uses **Git LFS** (Large File Storage) for handling large Unreal Engine assets:
- `.uasset` files (Unreal Engine assets)
- `.umap` files (Unreal Engine maps)
- `.bin` files (cached/intermediate files)

### Cloning the Repository

To clone this repository with all assets:

```bash
git lfs install
git clone https://github.com/kerinzeebart/VRstarter.git
```

## Getting Started

1. Ensure you have **Unreal Engine 5.6** installed
2. Clone the repository with Git LFS
3. Open `Visitor_v01/Visitor_v01.uproject`
4. Connect your VR headset
5. Play in VR mode to explore the environments

## Project Structure

```
VRstarter/
└── Visitor_v01/
    ├── Config/           - Project configuration files
    ├── Content/          - All game content and assets
    │   ├── 3DMODELS/    - Custom 3D environment models
    │   ├── Characters/   - Character models and animations
    │   ├── VRTemplate/   - VR gameplay systems
    │   ├── WaterPlane/   - Water rendering systems
    │   ├── Weapons/      - Weapon assets
    │   └── Meta/         - Game mode and pawn blueprints
    ├── Intermediate/     - Build cache (not in git)
    ├── Saved/           - Autosaves and editor data
    └── Visitor_v01.uproject - Main project file
```

## Development Notes

- Large 3D models (up to 393MB) are stored in Git LFS
- 4K textures used for high-quality environment rendering
- VR optimization with LOD settings for skeletal meshes
- Autosave functionality enabled for content protection

## Repository Size

- **Total Repository**: ~1.7GB
- **LFS Objects**: 2.1GB (297 objects)
- Optimized for version control using Git LFS

## License

[Add your license information here]

## Credits

Built using Unreal Engine's VR Template and custom environment assets.
