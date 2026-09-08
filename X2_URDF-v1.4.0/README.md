# X2 Ultra(new version) & X2 EDU Robot Model

[中文文档](README_CN.md)

## Choosing Your Model

Check the nameplate on the back of your robot's neck:

| Nameplate top line ends with | Model | Files to use |
|---|---|---|
| **"X2 Ultra -N"** | X2 Ultra(new version) | `X2-Ultra.urdf`, `X2-Ultra_simple_collision.urdf`, `X2-Ultra.xml` |
| **"X2 EDU"** | X2 EDU | `X2-EDU.urdf`, `X2-EDU_simple_collision.urdf`, `X2-EDU.xml` |

## Files

```
├── scene.xml                       # Scene file
├── X2-Ultra.urdf                   # X2 Ultra(new version) — full model
├── X2-Ultra_simple_collision.urdf  # X2 Ultra(new version) — simplified collision
├── X2-Ultra.xml                    # X2 Ultra(new version) — MuJoCo format
├── X2-EDU.urdf                     # X2 EDU — full model
├── X2-EDU_simple_collision.urdf    # X2 EDU — simplified collision
├── X2-EDU.xml                      # X2 EDU — MuJoCo format
├── meshes/                         # Mesh files (STL)
└── visual/                         # Preview images
```

## Model Preview

### X2 Ultra(new version)

![X2 Ultra(new version)](visual/x2_ultra_new_version.png)

## Changelog: Flagship → New Version

### Motors

* Peak torque upgraded from 36 N·m to 60 N·m. Affected joints:
  1. `*_ankle_pitch_joint`
  2. `*_shoulder_pitch_joint`
  3. `*_shoulder_roll_joint`

* Peak torque upgraded from 24 N·m to 36 N·m. Affected joints:
  1. `*_ankle_roll_joint`
  2. `*_shoulder_yaw_joint`
  3. `*_elbow_joint`
  4. `*_wrist_yaw_joint`

* Waist pitch/roll drive configuration updated from 48 N·m to 36 N·m. Affected joints:
  1. `*_waist_pitch_joint`
  2. `*_waist_roll_joint`

* Wrist motor replaced, peak torque 6 N·m. Affected joints:
  1. `wrist_roll_joint`
  2. `wrist_pitch_joint`

### Whole Body

* X2 Ultra(new version) mass: ~42 kg → ~45 kg
* Structural components reinforced

## License

This project is licensed under the Mulan PSL v2 (木兰宽松许可证, 第2版). See [LICENSE](../LICENSE) for details.
