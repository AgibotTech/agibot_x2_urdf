# X2 URDF 模型

[English](README.md)

灵犀 X2 系列人形机器人 URDF 模型。

## 支持机型

| 机型 | 目录 | 说明 |
|------|------|------|
| X2 旗舰版 | `X2_URDF-v1.3.0/` | 旗舰版 |
| X2 旗舰焕新版 | `X2_URDF-v1.4.0/X2-Ultra.*` | 电机升级，结构加强 |
| X2 人人造 | — | 即将上线 |

## 确认机型

查看机器人后颈的铭牌：
- 如果最上面一行结尾为 **"X2 Ultra"** → 使用 `X2_URDF-v1.3.0/x2_ultra.*`
- 如果最上面一行结尾为 **"X2 Ultra -N"** → 使用 `X2_URDF-v1.4.0/X2-Ultra.*`
- 如果最上面一行结尾为 **"X2 EDU"** → X2 人人造 URDF 模型即将上线，请关注仓库更新。

## 目录结构

```
├── X2_URDF-v1.3.0/                     # X2 旗舰版
│   ├── x2_ultra.urdf                   # 完整模型
│   ├── x2_ultra_simple_collision.urdf  # 简化碰撞体
│   ├── x2_ultra.xml                    # MuJoCo 格式
│   ├── x2_fist.urdf                    # 假拳末端执行器
│   ├── x2_fist.xml                     # 假拳末端执行器（MuJoCo）
│   ├── scene.xml                       # 场景文件
│   ├── meshes/                         # 网格模型（STL）
│   ├── visual/                         # 预览图片
│   └── README.md
│
└── X2_URDF-v1.4.0/                     # X2 旗舰焕新版
    ├── X2-Ultra.urdf                   # X2 旗舰焕新版 — 完整模型
    ├── X2-Ultra_simple_collision.urdf  # X2 旗舰焕新版 — 简化碰撞体
    ├── X2-Ultra.xml                    # X2 旗舰焕新版 — MuJoCo 格式
    ├── scene.xml                       # 场景文件
    ├── meshes/                         # 网格模型（STL）
    ├── visual/                         # 预览图片
    └── README.md
```

## 查看模型

### MuJoCo（XML）

```bash
pip3 install mujoco
python3 -m mujoco.viewer --mjcf X2_URDF-v1.3.0/scene.xml
```

或启动查看器后将 XML 文件拖拽到窗口中。

### URDF 在 VSCode 中

安装 **URDF Visualizer** 扩展。

## 关于 AgiBot

智元机器人致力于通用人形机器人研发。更多信息请访问[智元官网](https://www.agibot.com.cn)。

## 许可证

本项目采用木兰宽松许可证，第2版（Mulan PSL v2）开源。详见 [LICENSE](LICENSE) 文件。
