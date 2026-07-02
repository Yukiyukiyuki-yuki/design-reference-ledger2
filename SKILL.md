---
name: design-reference-ledger
description: Archive and reuse the user's creative design references with image-backed Chinese ledgers. Use when the user sends posters, campaign visuals, outdoor ads, brand key visuals, social graphics, packaging, editorial layouts, exhibition/event graphics, or screenshots and asks to记录/整理/点评/归档/存进灵感库, or later asks for design ideas, poster directions, moodboards, campaign visual concepts, or creative strategies based on saved references.
---

# Design Reference Ledger

## Purpose

Build a persistent, image-backed design inspiration ledger. Each new reference must preserve the original image, add one Chinese table row, write sharp design commentary, and extract reusable visual methods for future design briefs.

## Core Files

Use this default structure inside the active project or user-chosen archive folder:

```text
outputs/
  design-inspiration-ledger.md
  images/
    DIA-YYYYMMDD-###.png
```

Use `references/ledger-template.md` when creating a new ledger.

## Adding New References

1. Inspect every image or screenshot the user provides.
2. Read the existing `design-inspiration-ledger.md` if it exists.
3. Assign the next ID as `DIA-YYYYMMDD-###`.
4. Copy each source image out of any temporary clipboard path into `outputs/images/`.
   - Single image: `DIA-YYYYMMDD-###.png`
   - Multiple images for one case: `DIA-YYYYMMDD-###-1.png`, `DIA-YYYYMMDD-###-2.png`
5. Add one row to the Markdown table using the Chinese schema below.
6. In the `海报原图` cell, use Markdown image syntax with an absolute path:

```markdown
![DIA-YYYYMMDD-###](/absolute/path/to/outputs/images/DIA-YYYYMMDD-###.png)
```

For multiple images in one cell, stack them with `<br>` between Markdown image tags.

Do not use HTML `<img>` tags for local images; they may not render in Codex Desktop.

## Chinese Ledger Schema

Keep the main table columns exactly:

| 案例ID | 海报原图 | 记录日期 | 来源/文件 | 类型 | 场景/目标 | 第一眼钩子 | 版式结构 | 字体处理 | 色彩/光影 | 图像/材质 | 文案/信息 | 有效原因 | 可复用方法 | 标签 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

Field guidance:

- `案例ID`: `DIA-YYYYMMDD-###`.
- `海报原图`: Markdown image link with absolute local path.
- `记录日期`: Current date.
- `来源/文件`: Stable copied filename, not a temporary clipboard path.
- `类型`: Poster, outdoor ad, campaign KV, art festival visual, city/culture poster, product launch, etc.
- `场景/目标`: What the design is trying to achieve.
- `第一眼钩子`: The first visual reason someone stops.
- `版式结构`: Composition, hierarchy, negative space, grid, information placement.
- `字体处理`: Font mood, hand lettering, type hierarchy, type-image relationship.
- `色彩/光影`: Palette, contrast, light, texture, saturation.
- `图像/材质`: Photo, illustration, 3D, collage, object, place, surface, material.
- `文案/信息`: Main claim, slogan, narrative, event details.
- `有效原因`: Creative judgment; explain the mechanism, not only the look.
- `可复用方法`: A transferable design method for later briefs.
- `标签`: 5-10 searchable tags.

## Commentary After Each Row

After the table, append:

```markdown
## DIA-YYYYMMDD-### 点评

1. ...
2. ...
3. ...
4. ...
5. ...

## 以后可借用

- ...
- ...
- ...
```

Commentary must identify:

- Attention device: why the design stops people.
- Memory device: what remains after 3 seconds.
- Transferable method: what can be borrowed later.
- Risk: what may fail if copied without context.

Avoid empty adjectives like "高级", "有冲击力", or "很有创意" unless explaining the mechanism.

## Visual Pattern Vocabulary

Use concrete pattern names when useful:

- `真实照片 + 巨型口语判断句 + 手绘标注`
- `技术反命题 + 具体感官证据`
- `地方符号清单 + 复古印刷质感`
- `普通公共物件 + 戏剧化环境 + 精致字体`
- `黑白真实场景 + 荧光地图/地形图形 + 硬朗信息块`

## Generating Design Directions From The Ledger

When the user asks for new design ideas:

1. Read the ledger first.
2. Select 3-6 relevant cases by category, goal, audience, tone, tags, or visual mechanism.
3. Name the cases being reused.
4. Produce design directions with:
   - 核心想法
   - 视觉隐喻
   - 画面结构
   - 字体/颜色
   - 图像/材质
   - 文案语气
   - 可借鉴档案
   - 风险提醒

If multiple options are requested, make the options strategically different, not minor style variations.

## Output Defaults

Use Chinese by default.

After adding a case, summarize with:

```markdown
已追加为 `DIA-YYYYMMDD-###`。

| 项目 | 内容 |
|---|---|
| 类型 | ... |
| 第一眼钩子 | ... |
| 设计机制 | ... |
| 可复用方法 | ... |
```

