# X2 Ultra (new version) Robot Model

[中文文档](README_CN.md)

## Files

```
├── scene.xml                       # Scene file
├── X2-Ultra.urdf                   # X2 Ultra (new version) — full model
├── X2-Ultra_simple_collision.urdf  # X2 Ultra (new version) — simplified collision
├── X2-Ultra.xml                    # X2 Ultra (new version) — MuJoCo format
├── meshes/                         # Mesh files (STL)
└── visual/                         # Preview images
```

## Model Preview

### X2-Ultra (new version)

![X2-Ultra (new version)](visual/x2_ultra_new_version.png)

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
  5. `*_waist_pitch_joint`
  6. `*_waist_roll_joint`

* Wrist motor replaced, peak torque 6 N·m. Affected joints:
  1. `wrist_roll_joint`
  2. `wrist_pitch_joint`

### Whole Body

* X2-Ultra mass: ~41 kg → ~45 kg
* Structural components reinforced

## URDF Processing

URDF processing utilities are available in the `X2_URDF-v1.3.0/scripts/` directory.

## License

This project is licensed under the Mulan PSL v2 (木兰宽松许可证, 第2版). See [LICENSE](../LICENSE) for details.