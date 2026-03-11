# MG Spatial Selection – Demo Project (UE5.7)

![GitHub Release](https://img.shields.io/github/v/release/cem-akkaya/MGSpatialSelection)
[![Unreal Engine Supported Versions](https://img.shields.io/badge/Unreal_Engine-5.7-9455CE?logo=unrealengine)](https://github.com/cem-akkaya/MGSpatialSelection/releases)
![GitHub License](https://img.shields.io/github/license/cem-akkaya/MGSpatialSelection?label=License)
[![Actively Maintained](https://img.shields.io/badge/Maintenance%20Level-Actively%20Maintained-green.svg)](https://gist.github.com/cheerfulstoic/d107229326a01ff0f333a1d3476e068d)

<img src="https://raw.githubusercontent.com/cem-akkaya/MGSpatialSelection/refs/heads/master/Resources/Splash.jpg" alt="mgss-demo" width="100%"/>

## About This Demo

This project demonstrates how to use the **MG Spatial Selection** plugin inside a real Unreal Engine level.  
It shows how to achieve high-performance, real-time spatial selection of actors using a hybrid CPU/GPU architecture.

Original Plugin: **https://github.com/cem-akkaya/MGSpatialSelection**

The demo includes:

- **Material-Based Selection**: Custom post-process effects using the `MG Selection Mask` node.
- **Interface-Driven Interaction**: Example units implementing `IMGSpatialSelectionInterface`.
- **Enhanced Input Integration**: Ready-to-use input mapping for box selection.
- **Configurable Settings**: Examples of MPC integration and decay effects.

If you encounter any issues, please open an issue on the plugin repository.  
Feel free to contribute!

---

## How to Use the Demo

1. **Download or clone** this repository.
2. Ensure the **MG Spatial Selection** plugin is in the `Plugins/` directory.
3. Right-click the `.uproject` → **Generate Project Files**.
4. Build the project using Visual Studio or Rider.
5. Open in Unreal Engine.
6. Open the `Lvl_TopDown` map and **Play In Editor**.

---

## Inside the Demo Project

### Demo Map
- `Lvl_TopDown`: Simple top-down selection example.

### Key Blueprints
- `BP_TopDownCharacter`: Manages the `MGSpatialSelectionComponent` for selection.
- `SelectionTestActor_BP`: Example of a selectable actor implementing the interface.

### Features in Action
- **High-Performance Selection**: Uses native `UBoxComponent` for efficient overlap detection.
- **Dynamic Terrain-Aware Mask**: Pixel-perfect visuals that follow terrain geometry without CPU raycasts.
- **MPC Integration**: Real-time shader updates via Material Parameter Collections.
- **Post-Selection Decay**: Smooth "fade-out" effects when releasing the selection.

---

## Demo Images

<table>
<tr>
<td align="center">
<img src="Plugins/MGSpatialSelection/Resources/Demo1.gif" width="100%"/><br/>
<b>RTS Box Selection in Action</b>
</td>
<td align="center">
<img src="Plugins/MGSpatialSelection/Resources/Demo2.gif" width="100%"/><br/>
<b>Terrain-Aware Selection Mask</b>
</td>
</tr>
</table>

---

## Plugin Link

This demo is only the showcase.  
Download the full plugin here:

**https://github.com/cem-akkaya/MGSpatialSelection**

---

## License

This demo project is released under the **MIT License**.  
Commercial use is allowed as long as the copyright notice remains.

---

## Support Me

If this project helped you, consider supporting development:

<a href="https://www.buymeacoffee.com/akkayaceq" target="_blank">
<img src="https://cdn.buymeacoffee.com/buttons/default-yellow.png" height="41" width="174"/>
</a>
