---
name: xxd-panel-040
description: "Create XXD Panel 040 artwork from supplied photos in four independently selectable modes that may be combined: photo above/micro-narrative design below, photo left/design right, transformed design alone, or a four-device wallpaper pack with independent or anchor-linked continuity. Uses one truthful real-world subject anchor, sparse black-line doodle figures, source-derived colour, generous whitespace, and witty image-bound copy. Use for the exact 040 real-subject-plus-doodle editorial style; never use it for generic sticker decoration or multi-photo collage."
---

# XXD Panel 040 · 真实锚点与黑线微型叙事

Turn each supplied photograph into finished editorial artwork. Preserve the photograph only in paired modes; every transformed frame must reinterpret the same photo through one truthful real-world anchor, a few tiny black-line figures, and a concise visual joke or insight grounded in what the photo is really about.

Operational rules follow the shared XXD Panel workflow contract: four combinable modes; an explicitly confirmed whole-canvas ratio or exact resolution before generation; single complete-canvas raster generation by default; high-fidelity source reference in paired modes; linked or independent four-device wallpapers; copy and locale preflight; fresh generation jobs; privacy-preserving raster generation; deterministic composition as fallback only; and one fresh task directory per source and mode. Style-specific sections refine aesthetics and copy but never override this contract.

## Non-negotiable contract

- One source photo may be processed in one or more selected modes. Each selected ordinary mode (`top-bottom`, `left-right`, `design-only`) produces one PNG; selected `wallpaper-pack` produces exactly four separate PNGs. Selecting all four modes therefore produces seven final files per source. Keep every mode in its own task directory and never combine modes, sources, or wallpapers into a grid, contact sheet, or overview.
- Resolve a non-empty ordered set of modes before generation: `top-bottom`, `left-right`, `design-only`, and/or `wallpaper-pack`. Accept one choice, multiple choices separated by `+`, Chinese/English commas or whitespace, natural-language names, or `全部` / `all`. Deduplicate repeated choices and execute in menu order 1→4. If none is specified, ask with the multiline multi-select menu in the workflow. Do not ask again when the set is already clear.
- When the selected set contains `wallpaper-pack`, require a second choice: `linked` or `independent`. A linked pack approves one anchor wallpaper, iPad by default, and makes every other device reference both the original photo and that same anchor. An independent pack gives every device only the original photo. Neither permits resizing or cropping one wallpaper into the others. Do not ask this follow-up when wallpaper mode is not selected.
- Paired modes target a visually equal 50/50 relationship within one coherent generated canvas. Minor generative deviation is acceptable unless the user explicitly requires pixel-exact halves; exact deterministic geometry belongs to the documented fallback. `design-only` and every wallpaper contain no visible source photograph, no seam, and no reserved photographic panel.
- The whole final canvas ratio or exact pixels must be explicitly resolved before generation. Offer the archived/original-prompt 3:4, source aspect as an explicit choice, common ratios, or custom ratio/pixels; never infer explicitly selected final-canvas dimensions silently. Exact pixels take precedence over an explicitly chosen ratio.
- Visible photography remains faithful. Allow only restrained editorial grading and environmental extension needed for an explicitly overridden canvas. Never stretch, distort, repaint, replace, or structurally alter the subject.
- The transformed frame is not a photo filter or cartoon sticker sheet. It preserves one real, materially credible subject anchor and surrounds it with only a few primitive black or dark-grey line figures whose scale, poses, and interaction reinterpret the source relationship.
- Copy has no silent default. Resolve automatic copy, exact custom copy, or text-free output before image generation. Automatic and custom modes also require a target language or locale. By default, one source-specific copy package is shared verbatim across all selected modes; accept explicit per-mode copy overrides when the user supplies them.
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

1. Resolve one or more modes. If missing, ask exactly this as normal multiline chat text and wait:

   ```text
   请选择一个或多个模式（回复序号；多选可用 +、顿号或逗号）：

   1. 上下双联（原图在上＋040 设计在下）
   2. 左右双联（原图在左＋040 设计在右）
   3. 纯设计版（只显示 040 设计画面）
   4. 四端壁纸套装
      手机＋iPad＋电脑＋儿童手表

   示例：1｜1+3｜1、2、4｜全部
   ```

2. Before any ordinary-mode generation, explicitly resolve the **final finished canvas**, not the size of one panel. If the user did not already supply a ratio or exact pixels, ask and wait:

   ```text
   请选择最终成品画幅（回复序号即可；多选模式可共用，也可分别指定）：

   1. 原提示词画幅 3:4
   2. 跟随原图比例
   3. 常用比例
      1:1｜4:5｜2:3｜3:2｜16:9｜9:16
   4. 自定义比例或准确像素

   这里指整张最终成品的比例，不是单个区域。
   示例：1｜3：9:16｜4：2160×3840
   ```

   “跟随原图比例” is valid only when the user explicitly selects it. Never infer a silent canvas from the source dimensions, orientation, archived 3:4 brief, mode, or previous output. In multi-select, ask which mode an ambiguous ratio belongs to. Exact pixels take priority over a chosen ratio. For paired modes, odd split axes are allowed for direct generation; require an even split axis only if deterministic fallback composition is actually triggered.

3. Before generation, resolve copy mode and locale. If missing, ask and wait:

   ```text
   正式做图前，请确认文字设置（回复序号即可）：

   1. 自动文案
      我根据原图与 040 气质创作文案；请同时注明语言或地区
   2. 自定义文案
      请直接输入要呈现的准确文字，并注明语言或地区
   3. 无文字

   示例：1｜日语
   示例：2｜英式英语｜STILL IN BLOOM
   ```

   Automatic copy must be source-specific and native to the resolved locale. Preserve exact custom copy verbatim. Do not infer locale from appearance, clothing, scenery, filenames, metadata, or visible signs.

4. Only when `wallpaper-pack` is selected, resolve its relationship and device sizes. Ask for `1. 连贯套装` or `2. 四张独立` when missing. A linked set approves one iPad anchor by default; the other three outputs each reference the original plus that same anchor and are independently recomposed. An independent set gives every device only the original. Then ask for either the common preset—phone `1440×3200`, iPad `2048×2732`, desktop `3840×2160`, watch `1024×1024`—or labelled custom pixels. Never crop one wallpaper into another or chain derivatives.

5. Start a fresh job and reserve collision-safe output directories before generation. Use only the current invocation's explicit source or theme. Read `references/xxd-panel-040-prompt.en.md` or `references/xxd-panel-040-prompt.zh-CN.md` immediately before building the generation request.
6. Privately lock the principal subject or inseparable relationship, at least three source-specific recognition cues, the style's complete aesthetic motive, composition logic, materials, palette, typography, exact copy, and locale. The source photograph is the factual and identity anchor; do not borrow content from samples or old outputs.
7. Use **single complete-canvas generation as the default for every mode**:
   - `top-bottom`: supply the source as a high-fidelity edit/reference input and generate one finished image containing the faithful source in the upper half and the 040 transformation in the lower half.
   - `left-right`: supply the source as a high-fidelity edit/reference input and generate one finished image containing the faithful source on the left and the 040 transformation on the right.
   - `design-only`: generate the 040 transformation across the whole canvas; the source is reference-only and not visible.
   - `wallpaper-pack`: generate four separate complete canvases, one per device, following the resolved independent or linked relationship.
8. Append the complete-canvas payload below to the full local style prompt. Keep all 040-specific aesthetic and typography instructions active across the entire composition. For paired modes, ask for approximately equal regions while prioritising a coherent finished artwork: colour, light, rhythm, typography, meaning, and any cross-panel echo must feel intentionally unified.
9. Generate each distinct output as a fresh raster image job. Do not request two separate half-images, a contact sheet, a mockup, an empty reserved panel, or a code-rendered substitute.
10. Inspect the actual bitmap at full size and thumbnail size. Check, in order: whole-poster integration; 040 aesthetic fidelity; source identity and structure; visual and semantic correspondence between regions; typography and locale; mode, ratio/pixels, count, and PNG format; then approximate 50/50 geometry.
11. If a paired result fails a hard requirement, retry the **complete canvas once**, changing only the failed constraint. Use `scripts/compose_panel.py` only after that retry still fails, or when the user explicitly requires pixel-identical source preservation, the active image route cannot realise the selected canvas, the requested ratio exceeds route limits, or final lossless pixel calibration is necessary. The script is a fallback utility, never the default creative path and never an aesthetic judge.
12. Reopen every final PNG, apply the acceptance gate, and return absolute paths in source order and mode order 1→4. Wallpaper order is phone, iPad, desktop, watch.

## Complete-canvas generation payload

Append one resolved block to the style prompt for each output:

```text
OUTPUT MODE: TOP_BOTTOM | LEFT_RIGHT | DESIGN_ONLY | WALLPAPER_PACK
DEVICE PROFILE: NONE | PHONE | IPAD | DESKTOP | WATCH
FINAL CANVAS: <whole finished ratio and/or exact WIDTHxHEIGHT>
GENERATION STRATEGY: SINGLE COMPLETE CANVAS
REFERENCE ROLE: SOURCE — HIGH-FIDELITY CONTENT AND IDENTITY ANCHOR
SOURCE VISIBILITY: UPPER 50% | LEFT 50% | REFERENCE ONLY — NOT VISIBLE
LAYOUT RULE:
- Produce one finished poster in one image.
- TOP_BOTTOM keeps a faithful photographic source in the upper half and creates the transformed design in the lower half.
- LEFT_RIGHT keeps a faithful photographic source in the left half and creates the transformed design in the right half.
- DESIGN_ONLY and WALLPAPER_PACK use the whole canvas for the transformed design and show no source photograph or reserved panel.
- Keep paired regions approximately equal while unifying colour, light, rhythm, typography, and meaning.
- Do not output separate panels, a contact sheet, a mockup, or an empty placeholder.
WALLPAPER RELATIONSHIP: NONE | INDEPENDENT | LINKED
ANCHOR DEVICE: NONE | IPAD
```

For text output append:

```text
COPY MODE: REQUIRED
COPY ORIGIN: USER_EXACT | USER_DIRECTION | SOURCE_DERIVED
COPY LOCALE: <resolved locale>
COPY PAYLOAD: <the exact 040-specific title and supporting-text package resolved under the local production prompt>
COPY RULE: Render only the populated strings in COPY PAYLOAD, each exactly once. Do not rewrite, translate, spell-correct, duplicate, or add text. Use native shaping, direction, punctuation, spacing, and semantic line breaks. Preserve the 040-specific hierarchy, amount of supporting text, placement, material, and typographic role instead of applying a generic overlay.
```

For text-free output append only `COPY MODE: NONE — render no text or pseudo-text anywhere.`

## Composition fallback only

`scripts/compose_panel.py` remains available for deterministic recovery and audit. Trigger it only under step 11. When used, generate a same-aspect design asset from the full 040 prompt, preserve the source without destructive crop or stretch, and document which fallback condition applied. A direct complete-canvas success must not be split and recomposed again.

```bash
# Read-only audit after direct generation
python3 scripts/compose_panel.py --audit final.png --layout top-bottom --size WIDTHxHEIGHT

# Deterministic fallback after the complete-canvas retry has failed
python3 scripts/compose_panel.py --source photo.png --design design.png \
  --out final.png --layout top-bottom --size WIDTHxHEIGHT
```

## Output location

Save finished work under `~/Desktop/xxd/xxd-panel-040/` unless the user supplies another destination. Create the shared `~/Desktop/xxd/` wrapper, the skill root, and each task directory when needed.

- Wrap every source-and-mode result in a fresh task directory: `<source-stem>-top-bottom/`, `<source-stem>-left-right/`, `<source-stem>-design-only/`, or `<source-stem>-wallpaper-pack/`.
- A batch or multi-select creates one sibling task directory per source and selected mode. Never mix sources or modes.
- Ordinary task directories contain only one finished PNG: `<source-stem>.png`, `<source-stem>-lr.png`, or `<source-stem>-design.png`.
- The final count per source equals one file for each selected ordinary mode plus four files when `wallpaper-pack` is selected. `all` / `全部` therefore means seven final PNGs across four sibling task directories.
- A wallpaper task directory contains exactly four finished PNGs named `<source-stem>-wallpaper-phone.png`, `-ipad.png`, `-desktop.png`, and `-watch.png`; do not create device subdirectories.
- Never overwrite. Append `-2`, `-3`, and so on to a colliding task-directory name while keeping filenames unchanged.
- Keep prompts, intermediate generations, plans, audits, and source copies outside the finished task directory.

## Acceptance gate

Before accepting each result verify:

- Mode, exact pixels, explicit final-canvas ratio or pixels, split axis, seam, and output count are correct.
- Visible photography is faithful and type-free; source-hidden outputs contain no source photograph or seam.
- The real anchor is recognisable through at least three source-specific identity cues and retains believable material, colour, and form.
- Every doodle figure has a clear semantic job tied to the anchor and source relationship. No arbitrary cute poses, sticker look, clip art, or decorative crowd survives.
- The light ground, anchor colours, black-line contrast, and whitespace are source-aware and clean rather than sterile, busy, or candy-coloured.
- Automatic copy expresses the grounded meaning with a short, light, clever turn; it does not merely name the object, invent a story, or fit an unrelated image. Exact user copy remains verbatim. All rendered text is correct and native to the resolved locale; text-free output contains no text or pseudo-text.
- Type behaves like a handwritten in-scene annotation, thought, or voice-over that follows contour, action, or whitespace—not a boxed title pasted on afterward.
- Every wallpaper is separately recomposed, respects safe regions, contains no system UI, and is not a crop of another device result. A linked pack shares one visual family without drifting from the source.
- Every delivered PNG was newly generated for this invocation and lives in its fresh task directory.

## Override policy

Preserve user-specified source, mode set, output count, dimensions, target locale, copy mode, and exact finished wording. Priority is explicit text-free request > exact user wording > editable user direction > source-derived automatic copy. Exact pixels take precedence over an explicitly chosen ratio; neither may be inferred silently. A labelled wallpaper size overrides only that device.

User instructions may change subject emphasis, tone, interaction, or copy within 040, but do not silently relax one-photo isolation, exact paired geometry, four separate wallpaper outputs, fresh-task generation, source-hidden output rules, or native-language typography. Leave the truthful-anchor-plus-black-line-figure aesthetic only when the user explicitly asks to leave the 040 style.

## Provenance boundary

The user's original style brief is archived at [references/040-source.md](references/040-source.md). It records the initial 3:4 top-bottom example but does not override the operative mode and explicit final-canvas selection and complete-canvas generation rules. The full local 040 prompt is the production specification. Never borrow subjects, colours, copy, or compositions from samples or previous outputs.
