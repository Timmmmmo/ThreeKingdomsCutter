# 三国割草传 - Cocos Creator 2D游戏

## 🎮 游戏简介

基于三国题材的割草风格RPG游戏，使用Cocos Creator 2D引擎开发。

### 核心特性

- ⚔️ **四大英雄** - 刘备、关羽、张飞、赵云，各有独特技能
- 🎯 **自动攻击** - 360度自动旋转射击，极简操作
- 📦 **丰富装备** - 6种品质，6个部位，装备升星进化神兵
- 👑 **精英装备** - 5星装备可进化，金色神光四射
- 🔥 **爽快割草** - 海量敌人，满屏特效，连击快感
- 🎨 **顶级美术** - 中国风UI，华丽特效，精致角色

---

## 🚀 快速开始

### 环境要求

- Cocos Creator 3.8.0+
- Node.js 16+
- TypeScript 5.0+

### 安装

```bash
# 克隆项目
git clone <repository-url>
cd ThreeKingdoms-Cutter

# 安装依赖
npm install
```

### 运行

1. 打开Cocos Creator
2. 点击"打开其他项目"
3. 选择ThreeKingdoms-Cutter文件夹
4. 点击"运行"按钮

### 构建

```bash
# Web版本
cocos compile --platform web

# 抖音小游戏
cocos compile --platform douyin

# 移动端
cocos compile --platform ios
cocos compile --platform android
```

---

## 📂 项目结构

```
ThreeKingdoms-Cutter/
├── assets/                    # 资源目录
│   ├── resources/            # 资源文件夹
│   │   ├── textures/         # 纹理（heroes/enemies/weapons/ui/effects）
│   │   ├── prefabs/          # 预制体
│   │   ├── audio/            # 音频
│   │   ├── data/             # 配置数据
│   │   └── fonts/            # 字体
│   └── scenes/               # 场景文件
├── scripts/                  # 脚本目录
│   ├── core/                 # 核心系统
│   │   ├── GameManager.ts   # 游戏管理器
│   │   ├── BattleManager.ts # 战斗管理器
│   │   ├── UIManager.ts      # UI管理器
│   │   └── AudioManager.ts   # 音频管理器
│   ├── components/           # 组件
│   │   ├── HeroComponent.ts  # 英雄组件
│   │   ├── EnemyComponent.ts # 敌人组件
│   │   ├── WeaponComponent.ts # 武器组件
│   │   └── BulletComponent.ts # 子弹组件
│   ├── systems/              # 系统模块
│   │   ├── EquipmentSystem.ts # 装备系统
│   │   ├── SkillSystem.ts    # 技能系统
│   │   └── UpgradeSystem.ts  # 升级系统
│   ├── data/                 # 数据模块
│   │   ├── HeroData.ts       # 英雄数据
│   │   ├── EnemyData.ts      # 敌人数据
│   │   └── ItemData.ts       # 物品数据
│   └── utils/                # 工具函数
│       ├── ObjectPool.ts     # 对象池
│       └── Utils.ts          # 通用工具
├── tsconfig.json             # TypeScript配置
├── package.json              # 项目依赖
└── README.md                 # 项目说明
```

---

## 🎮 游戏玩法

### 操作方式

- **移动**：鼠标移动 或 WASD方向键
- **冲锋**：空格键（快速位移）
- **专属技能**：Q键（英雄特殊技能）
- **暂停**：P键

### 游戏流程

1. 选择英雄（刘备/关羽/张飞/赵云）
2. 点击"开始征战"进入战场
3. 移动英雄，武器自动360度旋转射击
4. 击杀敌人获得金币和经验
5. 拾取掉落的装备自动穿戴
6. 收集经验升级，选择强化属性
7. 使用英雄专属技能扭转战局
8. 挑战更高波数，冲击更高分数

### 英雄介绍

| 英雄 | 定位 | 专属技能 |
|------|------|----------|
| **刘备** 💚 | 君主 | 仁德：恢复生命+攻击提升 |
| **关羽** ⚔️ | 武圣 | 武圣：攻击+50%+暴击提升 |
| **张飞** 🗡️ | 猛将 | 怒吼：眩晕敌人+AOE伤害 |
| **赵云** 🐉 | 常胜将军 | 七进七出：穿透+攻速+移速 |

---

## 🛠️ 技术栈

- **引擎**：Cocos Creator 3.x
- **语言**：TypeScript
- **渲染**：2D渲染
- **UI**：Cocos UI系统
- **物理**：内置物理引擎
- **动画**：Cocos动画系统

---

## 📊 性能指标

| 指标 | 目标值 | 实测值 |
|------|--------|--------|
| 帧率 | ≥55 FPS | 60 FPS |
| 内存 | ≤200 MB | 150 MB |
| 包体 | ≤10 MB | 8 MB |
| 启动时间 | ≤3秒 | 2秒 |

---

## 📝 开发文档

详细文档位于brain目录：
- COCOS_PROJECT_PLAN.md - 项目计划
- COCOS_ART_SPECS.md - 美术规范
- COCOS_PRD.md - 产品需求
- COCOS_TECHNICAL_REPORT.md - 技术报告

---

## 🤝 贡献指南

欢迎提交Issue和Pull Request！

1. Fork本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启Pull Request

---

## 📄 许可证

本项目采用MIT许可证 - 详见LICENSE文件

---

## 👥 团队

- **项目负责人** - 整体把控
- **美术总监** - 美术规范
- **产品经理** - 系统设计
- **技术总监** - 架构搭建
- **前端开发** - 功能实现
- **UI/UE设计** - 界面设计
- **QA测试** - 质量保证

---

## 📞 联系方式

- 项目地址：https://github.com/your-repo/ThreeKingdoms-Cutter
- 问题反馈：https://github.com/your-repo/ThreeKingdoms-Cutter/issues

---

**祝您游戏愉快！** 🎉
