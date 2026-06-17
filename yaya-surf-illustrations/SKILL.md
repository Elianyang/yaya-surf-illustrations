---
name: yaya-surf-illustrations
description: Generate and plan Chinese article illustrations in Yaya's ocean-surf brand style. Use when the user asks for personal brand assets, blue-haired surfer girl IP, blue/pink/orange/white theme colors, Chinese body illustrations, article illustrations, shot lists, concept metaphors, workflow diagrams, or adapting Ian Xiaohei-style illustration logic into Yaya's own brand character.
---

# Yaya Surf Illustrations

## Core Positioning

Create 16:9 Chinese body illustrations that preserve the useful logic of Ian-style cognitive metaphor images while replacing the visual IP with Yaya's bright ocean-surf character system.

The goal is not an oil painting, glossy 3D render, beach poster, cute mascot sticker, PPT infographic, or generic avatar. The goal is to turn a key judgment, process, state, or metaphor from Chinese content into a clean, hand-drawn, brand-consistent illustration where the blue-haired surfer girl is doing the core cognitive action.

## Read As Needed

- `references/brand-dna.md`: visual DNA, theme colors, line, background, text, and style boundaries.
- `references/character-ip.md`: Yaya surfer girl portrait, personality, action library, and character constraints.
- `references/composition-patterns.md`: content-to-image structures and ocean/surf metaphor rules.
- `references/prompt-template.md`: single-image generation prompt template.
- `references/qa-checklist.md`: post-generation checks and iteration rules.
- `assets/character-reference.png`: visual reference for the character. Use for identity calibration, not for exact pose copying.

## Workflow

### 1. Digest The Content

Read the user-provided article, Markdown file, screenshot, notes, or concept. Identify:

- the core claim
- the cognitive turn
- the workflow or state change
- which sections need an illustration
- which sections should stay text-only

Do not illustrate every paragraph. Prefer cognitive anchors such as before/after change, branching choices, a stuck point, a handoff, an input-output loop, a missing bridge, a repeated wave, or evidence accumulating into trust.

### 2. Produce A Shot List First

If the user asks to analyze, plan, or think through illustrations, output a short shot list before generating images. For each image include:

- where it goes
- topic
- core meaning
- structure type
- what Yaya is doing
- suggested visual elements
- short Chinese annotation words

Default to 4-8 images for a long article, 1-3 for short content. Keep it useful rather than turning the article into a picture book.

### 3. Generate One Image At A Time

If the user asks to generate or make images, call `image_gen` for each image separately. Do not combine multiple concepts into one collage unless explicitly requested.

Each image should include:

- 16:9 horizontal Chinese body illustration
- clean white or white-with-airy-sky hand-drawn background
- Yaya surfer girl as the action subject
- vivid blue hair gathered into one ponytail/braid, with orange braided accents; never two ponytails
- blue/pink/orange/white palette with deep navy for structure
- loose pencil/ink linework with simple flat color fills
- short handwritten-style Chinese annotations
- a small bottom-corner handwritten credit: `Co-Created with 丫丫老师AI研习社`
- one clear metaphor or state change
- generous whitespace

Avoid directly copying Ian Xiaohei compositions. Keep the method of "one cognitive action per image", but invent new metaphors from the user's content and Yaya's ocean-surf world.

### 4. Check And Iterate

After generation, use `references/qa-checklist.md`. Regenerate or edit if:

- Yaya is only posing or decorating
- the image becomes a generic beach portrait
- the image becomes oil-painted, glossy, or 3D-rendered
- the cognitive structure is unclear
- it looks like a PPT diagram
- there are too many labels or long Chinese text
- the palette drifts away from blue/pink/orange/white
- the character loses blue hair, single ponytail/braid, orange surfboard, or friendly surfer identity
- the image omits the bottom-corner credit

### 5. Save Deliverables

When working inside a workspace, save final images to:

```text
assets/<article-slug>-yaya-surf-illustrations/
```

Name files in order:

```text
01-topic-name.png
02-topic-name.png
```

Keep original generated files unless the user explicitly asks to replace them.

## Output

For plans, be concise and practical. For generated images, report:

- how many images were generated
- what each image is for
- save paths
- which images are strongest and which are optional
