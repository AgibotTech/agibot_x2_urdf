# X2 URDF Models

[中文文档](README_CN.md) | [GitHub](https://github.com/AgibotTech/agibot_x2_urdf)

URDF models for the AgiBot X2 series humanoid robots.

## Supported Models

| Model | Directory | Description |
|-------|-----------|-------------|
| X2 Ultra | `X2_URDF-v1.3.0/` | Flagship model |
| X2 Ultra(new version) | `X2_URDF-v1.4.0/` | Upgraded motors, reinforced structure |
| X2 EDU | `X2_URDF-v1.4.0/` | Educational variant |

## Identifying Your Robot

Check the nameplate on the back of your robot's neck:
- If the top line ends with **"X2 Ultra"** → use `X2_URDF-v1.3.0/` (`x2_*` files)
- If the top line ends with **"X2 Ultra -N"** → use `X2_URDF-v1.4.0/` (`X2-Ultra.*` files)
- If the top line ends with **"X2 EDU"** → use `X2_URDF-v1.4.0/` (`X2-EDU.*` files)

## Directory Structure

```
├── X2_URDF-v1.3.0/                     # X2 Ultra (flagship)
│   ├── x2_ultra.urdf                   # Full model
│   ├── x2_ultra_simple_collision.urdf  # Simplified collision
│   ├── x2_ultra.xml                    # MuJoCo format
│   ├── x2_fist.urdf                    # Dummy fist end-effector
│   ├── x2_fist.xml                     # Dummy fist end-effector (MuJoCo)
│   ├── scene.xml                       # Scene file
│   ├── meshes/                         # Mesh files (STL)
│   ├── visual/                         # Preview images
│   ├── README_CN.md
│   └── README.md
│
└── X2_URDF-v1.4.0/                     # X2 Ultra(new version) & X2 EDU
    ├── X2-Ultra.urdf                   # X2 Ultra(new version) — full model
    ├── X2-Ultra_simple_collision.urdf  # X2 Ultra(new version) — simplified collision
    ├── X2-Ultra.xml                    # X2 Ultra(new version) — MuJoCo format
    ├── X2-Ultra_omnihand.urdf          # X2 Ultra(new version) — dexterous hand variant
    ├── X2-Ultra_omnipicker.urdf        # X2 Ultra(new version) — gripper variant
    ├── X2-EDU.urdf                     # X2 EDU — full model
    ├── X2-EDU_simple_collision.urdf    # X2 EDU — simplified collision
    ├── X2-EDU.xml                      # X2 EDU — MuJoCo format
    ├── scene.xml                       # Scene file
    ├── meshes/                         # Mesh files (STL)
    ├── visual/                         # Preview images
    ├── README_CN.md
    └── README.md
```

## Viewing the Models

### MuJoCo (XML)

```bash
pip3 install mujoco
python3 -m mujoco.viewer --mjcf X2_URDF-v1.3.0/scene.xml
```

Or launch the viewer and drag-and-drop the XML file into the window.

### URDF in VSCode

Install the **URDF Visualizer** extension.

## About AgiBot

AgiBot is a robotics company building general-purpose humanoid robots. Learn more at [official website](https://www.agibot.com).

## License

This project is licensed under the Mulan PSL v2 (木兰宽松许可证, 第2版). See [LICENSE](LICENSE) for details.
