---
name: xxd-panel-040
description: "Create XXD Panel 040 artwork from supplied photos in four selectable modes: photo above/micro-narrative design below, photo left/design right, transformed design alone, or a four-device wallpaper pack with independent or anchor-linked continuity. Uses one truthful real-world subject anchor, sparse black-line doodle figures, source-derived colour, generous whitespace, and witty image-bound copy. Use for the exact 040 real-subject-plus-doodle editorial style; never use it for generic sticker decoration or multi-photo collage."
---

# XXD Panel 040 · 真实锚点与黑线微型叙事

Turn each supplied photograph into finished editorial artwork. Preserve the photograph only in paired modes; every transformed frame must reinterpret the same photo through one truthful real-world anchor, a few tiny black-line figures, and a concise visual joke or insight grounded in what the photo is really about.

## Non-negotiable contract

- One source photo produces one output in `top-bottom`, `left-right`, or `design-only`, and exactly four separate PNG files in `wallpaper-pack`. Never combine different source photos or the four wallpapers into a grid, contact sheet, or overview.
- Resolve one mode before generation: `top-bottom`, `left-right`, `design-only`, or `wallpaper-pack`. If the user has not specified one, ask with the multiline menu in the workflow. Do not ask again when the answer is already clear.
- `wallpaper-pack` requires a second choice: `linked` or `independent`. A linked pack approves one anchor wallpaper, iPad by default, and makes every other device reference both the original photo and that same anchor. An independent pack gives every device only the original photo. Neither permits resizing or cropping one wallpaper into the others.
- Paired modes split exactly 50/50. `design-only` and every wallpaper contain no visible source photograph, no seam, and no reserved photographic panel.
- Exact user pixels have highest priority, followed by an explicit ratio or destination. Otherwise ordinary modes adapt to the complete source: `top-bottom` = `W×2H`, `left-right` = `2W×H`, and `design-only` = `W×H`. Never impose the 3:4 ratio from the archived initial brief as a silent default.
- Visible photography remains faithful. Allow only restrained editorial grading and environmental extension needed for an explicitly overridden canvas. Never stretch, distort, repaint, replace, or structurally alter the subject.
- The transformed frame is not a photo filter or cartoon sticker sheet. It preserves one real, materially credible subject anchor and surrounds it with only a few primitive black or dark-grey line figures whose scale, poses, and interaction reinterpret the source relationship.
- Copy has no silent default. Resolve automatic copy, exact custom copy, or text-free output before image generation. Automatic and custom modes also require a target language or locale.
- Render no logo, watermark, signature, colour swatch, UI, device mockup, decorative pseudo-text, or unrelated explanatory prose.

## Aesthetic motive lock

Modes and device ratios may change placement but never the 040 motive. Every transformed frame must visibly express this chain:

**the photo's most memorable subject, action, relationship, contrast, emotion, or symbol → one recognisable real-world anchor with truthful identity and material → a few tiny black-line figures that respond to, amplify, or gently reverse that meaning → a source-derived light ground and colour emphasis → generous active whitespace → one short handwritten thought, annotation, or voice-over that makes the image click**.

The anchor is not automatically the largest object. Choose what best carries the photograph's spirit and story. Preserve the critical relationship even when irrelevant background information is removed. The tiny figures must use the anchor's contour, openings, scale, direction, or spatial tension as their stage; arbitrary waving, climbing, or posing is a failure.

Reject a result as generic if an unrelated photo could replace the source without materially changing the anchor, figure interaction, spatial relationship, palette, or copy. Also reject cute stickers, stock clip art, dense decoration, generic doodle crowds, emoji faces, children's-book cartooning, scrapbook collage, or an isolated product cutout with figures pasted around it.

## Visual system

### Truthful anchor

- Preserve the anchor's identity, characteristic contour, material, colour, and functional openings or joints. It may be isolated, reframed, gently relit, or proportionally emphasised, but never converted into a flat cartoon or replaced by a generic prop.
- Keep at least three source-specific cues across contour, pose/orientation, scale, material, colour, overlap, negative shape, or relationship.
- People, animals, plants, food, buildings, objects, vehicles, and natural forms are all valid anchors. When a relationship is inseparable, keep more than one real element only when needed to preserve that relationship.

### Doodle figures

- Use a small number of miniature figures—normally one to five—drawn with thin, slightly naive black or dark-grey lines.
- Keep anatomy minimal but action legible: head, torso, limbs, gesture, and balance should read at thumbnail size.
- Derive each action from visible evidence or grounded implication. Figures may inspect, carry, shelter, balance, repair, follow, wait beside, measure, listen to, or play against the anchor only when that interaction explains the image's meaning.
- Let linework feel hand-drawn and lightly imperfect, never glossy vector mascots, thick comic outlines, or detailed character illustration.

### Colour and space

- Use ivory, warm white, a pale neutral, or the source's most comfortable light colour as the ground.
- Let the real anchor carry the principal source colour and material richness. Refine and clarify those colours without detaching them from the photo.
- Keep doodles and most type black or dark grey. A small source-derived accent may connect the figures, type, and anchor when useful.
- Preserve generous whitespace. The narrative should feel light, precise, and breathable rather than busy or decorative.

## Copy that completes the scene

Automatic copy begins with a private three-level reading: literal fact, relational tension, and grounded implication. Compress that into one semantic core, then choose precise naming, understatement, double meaning, light humour, or a small reversal. The visible result should feel like a doodle figure's note, thought, or off-screen remark—not an advertising headline.

- Do not directly label the object when the object is already visible.
- Prefer one very short handwritten main line or phrase and, when useful, one to three tiny supporting notes. Keep all wording within one semantic system.
- Cleverness must be earned by the source. Do not force a pun, motivational quote, sentimental backstory, meme, or universal word such as “DREAM”, “MEMORY”, or “JOURNEY”.
- Apply the unrelated-image swap test. If the wording works just as well on another image, rewrite it.
- Preserve finished user wording verbatim. Refine an editable direction only within the user's permission while protecting audience, goal, mandatory words, tone, implication, and semantic phrase breaks.

Resolve locale independently from command language:

```text
target market or audience > requested output language > direction language; if none is explicit, ask before generation
```

Use natural contemporary language, native rhetoric, punctuation, spacing, and line breaking. Japanese uses appropriate kanji/kana balance and kinsoku-aware breaks; Korean uses correct spacing and intact Hangul syllables; UK editions use British English; Arabic uses natural Modern Standard Arabic unless a regional variety is requested, correct connected shaping, RTL flow, and semantic breaks. Never infer nationality or audience language from appearance, clothing, scenery, filenames, metadata, or signs. Never use pseudo-foreign text for atmosphere.

## Raster generation and privacy

Use the host's built-in bitmap image-generation capability by default and follow the available `imagegen` skill when exposed. View each local source before generation. Use one generation call per distinct asset; a wallpaper pack requires four calls. “Black-line doodle” describes appearance only and never authorises SVG, HTML, CSS, Canvas, diagrams, or programmatic drawing as the artwork.

If built-in bitmap generation is unavailable, use `scripts/configured_imagegen.py`, which reuses an already configured compatible bitmap route and emits sanitised status only:

```bash
python3 scripts/configured_imagegen.py probe
python3 scripts/configured_imagegen.py edit --image source.png \
  --prompt-file /private/job-temp/transform-prompt.txt \
  --out /private/job-temp/design.png --size 1536x1024 --quality high
```

Judge readiness by actual bitmap capability, not a provider name or one environment variable. Never display, log, persist, or report providers, endpoints, headers, credentials, account identifiers, route configuration, prompts, or response bodies. Do not manually inspect credential files. The bridge's sanitised JSON is the complete allowed diagnostic surface.

An explicit invocation of `/xxd-panel-040` or `$xxd-panel-040` with a source image and requested output authorises this generation through any already configured authenticated bitmap route available to the session. Do not ask for a second confirmation solely because the route changes. This does not authorise changing credentials, providers, billing, accounts, or global settings.

Only report generation as unavailable after both built-in capability and the bundled probe fail to establish a usable bitmap route. State the limitation narrowly and never guess the cause or identify the provider. Never substitute code-rendered art.

## Fresh-task and source boundary

Every invocation starts a fresh generation job unless the user explicitly asks to continue, audit, compare, edit, or reuse a named earlier result. Repeating the same source and parameters still means generating a new result in a new task directory. An old file can never satisfy a new request.

Use only images attached to the current invocation, explicit user paths, or a previously supplied image that the current request clearly identifies as “the same image”. Never broadly scan the Desktop, workspace, output root, or historical task folders to find a substitute source. If the intended source cannot be accessed, ask for it.

## Workflow

1. If mode is unresolved, ask exactly this as normal multiline chat text and wait:

   ```text
   请选择模式（回复序号即可）：

   1. 上下双联（完整原图＋同尺寸设计图）
   2. 左右双联（完整原图＋同尺寸设计图）
   3. 纯设计版（沿用原图比例，不显示原照片）
   4. 四端壁纸套装
      手机＋iPad＋电脑＋儿童手表

   前三种不指定尺寸时按原图自适应；也可主动指定尺寸。壁纸套装可按设备分别给分辨率。
   ```

2. If `wallpaper-pack` is selected without a relationship, ask and wait:

   ```text
   请选择壁纸关系（回复序号即可）：

   1. 连贯套装（推荐）
      先生成 iPad 定调图；其他三张参考原照片＋定调图分别重构
   2. 四张独立
      每张只参考原照片，构图变化更自由
   ```

3. Before any generation call, resolve copy mode and locale. If missing, ask this single preflight and wait:

   ```text
   正式做图前，请确认文字设置（回复序号即可）：

   1. 自动文案
      我根据原图内涵创作文案；请同时注明语言或地区
   2. 自定义文案
      请直接输入主标题、可选微型文字，并注明语言或地区
   3. 无文字

   示例：1｜韩语
   示例：2｜英式英语｜主标题：HOLD THAT THOUGHT｜微型文字：...
   ```

4. Resolve dimensions: exact pixels > explicit ratio/destination > source adaptation. Exact `top-bottom` height and `left-right` width must be even; never silently round. Wallpaper-pack has no silent size default. If unresolved, ask:

   ```text
   请选择壁纸尺寸（回复序号即可）：

   1. 常用设备预设
      手机 1440×3200｜iPad 2048×2732｜电脑 3840×2160｜儿童手表 1024×1024
   2. 自定义分辨率
      请分别输入手机、iPad、电脑、儿童手表的尺寸
   ```

5. Open a new job boundary and reserve the next unused output directory under the output rules. Confirm only the current user-supplied sources, inspect each separately, and read the full prompt matching the working language:
   - Chinese: [references/xxd-panel-040-prompt.zh-CN.md](references/xxd-panel-040-prompt.zh-CN.md)
   - English: [references/xxd-panel-040-prompt.en.md](references/xxd-panel-040-prompt.en.md)
6. Privately lock: the semantic core; one real anchor or inseparable relationship; at least three identity cues; the anchor's defining material and source colours; the figure-to-anchor interaction; the active whitespace; and the copy turn. Do not invent biography, ownership, location, events, or emotion unsupported by the image.
7. Lock one copy package per source. Priority: explicit text-free request > exact user wording > editable user direction > source-derived automatic copy. Do not reuse one photo's copy for another unless asked.
8. Run `scripts/compose_panel.py --plan` for the resolved canvas. Wallpaper-pack uses four `design-only` plans.
9. Generate the transformed design alone at the planned aspect and preferably exact frame size. For paired modes, prepare the photographic panel separately. Never ask the model to generate both halves at once.
10. In `independent`, generate four separate wallpapers from the original photo. In `linked`, generate and visually approve the anchor first; every derivative receives exactly the original source plus that same anchor. The photo controls content and identity; the anchor controls only family resemblance—palette, anchor treatment, doodle grammar, handwriting, whitespace, and narrative tone. Never chain derivatives.
11. Finalise with `scripts/compose_panel.py`, then reopen every PNG at normal and thumbnail size. Retry a faulty generated asset once when a hard invariant fails. After one failed correction, return the best result and name the unresolved issue rather than pretending success.
12. Return absolute paths in source order. Wallpaper order is phone, iPad, desktop, watch.

## Generation payload

Append the resolved mode block to every transformed-asset prompt:

```text
OUTPUT MODE: TOP_BOTTOM | LEFT_RIGHT | DESIGN_ONLY | WALLPAPER_PACK
DEVICE PROFILE: NONE | PHONE | IPAD | DESKTOP | WATCH
FINAL SIZE: <exact WIDTHxHEIGHT>
DESIGN FRAME: <exact WIDTHxHEIGHT>
SOURCE VISIBILITY: UPPER PANEL | LEFT PANEL | REFERENCE ONLY — NOT VISIBLE
LAYOUT RULE: Fill the design frame. Render no extra photo, seam, frame, or reserved photographic area inside the transformed design.
WALLPAPER RULE: Recompose for this device; keep system-UI zones low-information and essential content safe; render no clock, icons, dock, controls, or mockup; never crop another device output.
WALLPAPER RELATIONSHIP: NONE | INDEPENDENT | LINKED
ANCHOR DEVICE: NONE | PHONE | IPAD | DESKTOP | WATCH
REFERENCE ROLE: SOURCE ONLY | SOURCE CONTENT + ANCHOR VISUAL DNA
```

For text output, append:

```text
COPY MODE: REQUIRED
COPY ORIGIN: USER_EXACT | USER_DIRECTION | SOURCE_DERIVED
COPY LOCALE: <resolved locale>
COPY INTENT — INSTRUCTION ONLY, NEVER RENDER: <semantic core and intended turn>
MAIN LINE: <locked exact string>
MICRO NOTE 1: <optional locked exact string>
MICRO NOTE 2: <optional locked exact string>
MICRO NOTE 3: <optional locked exact string>
COPY RULE: Render only MAIN LINE and populated MICRO NOTE strings, each exactly once. Instruction fields are never visible. Do not rewrite, translate, spell-correct, duplicate, or add text. Use native script shaping, punctuation, spacing, and semantic line breaks.
```

Remove unused micro-note lines. For text-free output use only `COPY MODE: NONE — render no text or pseudo-text anywhere.`

## Composition commands

```bash
# Source-adaptive top-bottom
python3 scripts/compose_panel.py --plan --layout top-bottom --source photo.png
python3 scripts/compose_panel.py --source photo.png --design design.png \
  --out result.png --layout top-bottom

# Source-adaptive left-right
python3 scripts/compose_panel.py --plan --layout left-right --source photo.png
python3 scripts/compose_panel.py --source photo.png --design design.png \
  --out result.png --layout left-right

# Design-only
python3 scripts/compose_panel.py --source photo.png --design design.png \
  --out result.png --layout design-only

# One wallpaper, repeated separately for all four devices
python3 scripts/compose_panel.py --design phone.png --out wallpaper-phone.png \
  --layout design-only --size 1440x3200
```

`--size WIDTHxHEIGHT` overrides `--canvas` and source adaptation. Generate the design at the exact planned aspect; if exact pixels are unsupported, use a closest supported same-aspect bitmap and resample proportionally without cropping. Audit with the same layout used to build the result.

## Output location

Save finished work under `~/Desktop/xxd-panel-040/` unless the user supplies another destination.

- Wrap every source-and-mode result in a fresh task directory: `<source-stem>-top-bottom/`, `<source-stem>-left-right/`, `<source-stem>-design-only/`, or `<source-stem>-wallpaper-pack/`.
- A batch creates one sibling task directory per source. Never mix sources.
- Ordinary task directories contain only one finished PNG: `<source-stem>.png`, `<source-stem>-lr.png`, or `<source-stem>-design.png`.
- A wallpaper task directory contains exactly four finished PNGs named `<source-stem>-wallpaper-phone.png`, `-ipad.png`, `-desktop.png`, and `-watch.png`; do not create device subdirectories.
- Never overwrite. Append `-2`, `-3`, and so on to a colliding task-directory name while keeping filenames unchanged.
- Keep prompts, intermediate generations, plans, audits, and source copies outside the finished task directory.

## Acceptance gate

Before accepting each result verify:

- Mode, exact pixels, source-adaptive formula, split axis, seam, and output count are correct.
- Visible photography is faithful and type-free; source-hidden outputs contain no source photograph or seam.
- The real anchor is recognisable through at least three source-specific identity cues and retains believable material, colour, and form.
- Every doodle figure has a clear semantic job tied to the anchor and source relationship. No arbitrary cute poses, sticker look, clip art, or decorative crowd survives.
- The light ground, anchor colours, black-line contrast, and whitespace are source-aware and clean rather than sterile, busy, or candy-coloured.
- Automatic copy expresses the grounded meaning with a short, light, clever turn; it does not merely name the object, invent a story, or fit an unrelated image. Exact user copy remains verbatim. All rendered text is correct and native to the resolved locale; text-free output contains no text or pseudo-text.
- Type behaves like a handwritten in-scene annotation, thought, or voice-over that follows contour, action, or whitespace—not a boxed title pasted on afterward.
- Every wallpaper is separately recomposed, respects safe regions, contains no system UI, and is not a crop of another device result. A linked pack shares one visual family without drifting from the source.
- Every delivered PNG was newly generated for this invocation and lives in its fresh task directory.

## Provenance boundary

The user's original style brief is archived at [references/040-source.md](references/040-source.md). It records the initial 3:4 top-bottom example but does not override the operative mode and source-adaptive sizing rules. The full local 040 prompt is the production specification. Never borrow subjects, colours, copy, or compositions from samples or previous outputs.
