# Contributing to tourism-okf

## Concept format

Every concept is a UTF-8 markdown file with YAML frontmatter. Required field: **`type`**.

```markdown
---
type: Attraction
title: 秦始皇兵马俑博物馆
description: 世界文化遗产，秦始皇帝陵陪葬坑，需提前预约。
tags: [xian, lintong, world-heritage]
timestamp: 2026-06-30T00:00:00Z
---

# Body …

# Citations

[1] [Official source](https://…)
```

## Directory layout (C1)

```text
tour-guide/destinations/<city>/
├── index.md
├── attractions/
├── routes/
├── tips/
├── food/
└── culture/
```

## Citation priority

1. 景区 / 博物馆 **官方网站**（开放时间、票价、预约）
2. **陕西省文化和旅游厅**、**西安市文化和旅游局** 公告
3. **全国旅游监管服务平台**（12301）
4. 高德 POI（地址、坐标）— 补充定位，不作唯一事实来源
5. 攻略类网站 — **仅作叙述参考，不得作为 `# Citations` 主源**

Claims about hours, tickets, or policies **must** cite an official source or say「以当季公告为准」.

## Type vocabulary

| type | Use for |
| --- | --- |
| `Attraction` | 景点、博物馆、街区 |
| `Route` | 可执行路线 |
| `Tip` | 交通、季节、预约、避坑 |
| `Food` | 餐饮、小吃 |
| `Culture` | 历史背景、非遗、典故 |
| `Persona` | 导游人设（可选） |

## Index files

- Bundle root `tour-guide/index.md` may declare only `okf_version: "0.1"`.
- Subdirectory `index.md` files have **no frontmatter**.

## Phase 1 (西安 D2)

- **Done**: 10 core attractions (E2 review)
- **Next**: 20 more attractions, routes, tips, food, culture (~70 concepts)
