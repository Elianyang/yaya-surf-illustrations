# Yaya Surf Illustrations

> Blue/pink/orange/white ocean-surf illustration skill for Chinese article visuals.

`yaya-surf-illustrations` is a Codex skill for turning Chinese articles, notes, and methods into bright, ocean-themed body illustrations using Yaya's surfer girl brand IP.

It keeps the useful illustration logic of "one cognitive action per image": first understand the article's key judgment, state change, workflow, or metaphor, then turn that idea into a clean 16:9 visual.

## Visual Identity

- Blue-haired surfer girl IP
- Orange surfboard as the signature action object
- Deep-blue wetsuit with white panels
- Bright sky, cloud, wave, and white-space atmosphere
- Blue / pink / orange / white theme colors
- Short handwritten-style Chinese annotations

Theme color anchors:

- Sky blue: `#48B0E0` / `#60B8E8`
- Deep ocean blue: `#003080` / `#0B2F7A`
- Surf orange: `#E08850` / `#F07A2A`
- Soft pink: `#F4A7B8` / `#F8C7D2`
- Cloud white: `#FFFFFF` / `#F8F8F0`

## Install

Copy the skill folder into your Codex skills directory:

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./yaya-surf-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

Restart Codex after installation.

## Usage

Plan article illustrations:

```text
Use $yaya-surf-illustrations 先不要生图。
请为下面这篇中文文章设计 5 张正文配图 shot list。
```

Generate illustrations:

```text
Use $yaya-surf-illustrations 为这篇中文文章设计并生成 4 张海风冲浪女孩正文配图。
```

Single concept image:

```text
Use $yaya-surf-illustrations 为“我不是没时间学习，我是怕错过”生成一张正文配图。
```

## Structure

```text
yaya-surf-illustrations/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── character-reference.png
└── references/
    ├── brand-dna.md
    ├── character-ip.md
    ├── composition-patterns.md
    ├── prompt-template.md
    └── qa-checklist.md
```

## Notes

- Keep Yaya functionally necessary in the image, not just posing.
- Avoid generic beach posters and dense PPT diagrams.
- Keep Chinese labels short.
- Use the character reference for identity calibration, not exact pose copying.
- This repository contains personal brand assets. No open-source license is granted unless a license file is added later.

