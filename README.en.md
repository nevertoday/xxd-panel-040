<p align="center">
  <img src="./assets/banner.svg" alt="XXD Panel 040 project banner" width="1200">
</p>

<div align="center">

# 🦁 XXD Panel 040

### Turn what a photograph is truly saying into one real anchor and a tiny black-line story

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)
[![Four Modes](https://img.shields.io/badge/Modes-4-d75d32?style=flat-square)](#four-outputs-one-narrative-logic)
[![Raster Output](https://img.shields.io/badge/Output-PNG-3c6f67?style=flat-square)](#boundaries-and-trust)

<a href="README.md">简体中文</a> · <strong>English</strong> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

> TRUTHFUL ANCHOR · BLACK-LINE FIGURES · MICRO-NARRATIVE · ACTIVE WHITESPACE

XXD Panel 040 is an image-generation skill for Codex and compatible agents. It does not simply add cute doodles to a photograph. It first decides what is most worth remembering, preserves one truthful and materially credible visual anchor, then lets a few black-line figures respond to, amplify, or gently reverse the source story.

Copy grows from the same implication, like a figure's annotation, thought, or off-screen remark.

## Why it exists

“Real object plus doodle people” easily becomes a sticker template: figures climb, sit, and wave no matter what the source contains; the largest cutout object becomes the subject; copy merely names it or adds a motivational line.

040 reverses that order:

```text
read the facts → find the relationship → distil the implication → select the real anchor → design the interaction → write the voice-over
```

If an unrelated photograph could replace the source without materially changing the anchor, figure action, spatial relation, colour, or copy, the result is not 040.

## The 040 visual contract

- **Truthful anchor:** retain photographic credibility, material identity, defining contour, and principal source colour rather than cartooning the subject.
- **At least three identity cues:** contour, pose, direction, proportion, material, colour, opening, negative shape, or relational distance keep the source recognisable.
- **One to five black-line figures:** thin, slightly naive, and action-readable; every gesture must serve the source implication.
- **Interaction, not stickers:** figures genuinely use the anchor's edge, opening, surface, direction, or scale instead of floating beside it.
- **Source colour and a light field:** the real anchor carries colour; a comfortable pale ground gives black or dark-grey lines clear contrast.
- **Active whitespace:** the composition stays light, exact, and breathable rather than manufacturing design through decoration.
- **In-scene copy:** wording behaves like an annotation, thought, or voice-over that completes the figure action.

## Samples

<div align="center">

### Samples in progress

This section is reserved for approved 040 artwork and its original posts. Samples demonstrate adaptability only; they never become generation references, fixed palettes, fixed copy, or default canvas sizes.

</div>

## Four outputs, one narrative logic

If no mode is specified, the skill asks first. Dimensions may be supplied in the same reply; exact pixels take priority.

| Mode | Sizing logic | Deliverable |
| --- | --- | --- |
| `top-bottom` | source-adaptive | complete source above, 040 micro-narrative below; both panels retain the source size and split exactly 50/50 |
| `left-right` | source-adaptive | complete source left, 040 micro-narrative right; both panels retain the source size and split exactly 50/50 |
| `design-only` | source-adaptive | transformed design only, with no visible source photo; retains source ratio and dimensions |
| `wallpaper-pack` | four device sizes | separate phone, iPad, desktop, and children's-watch PNGs |

Exact user pixels > explicit ratio or destination > source adaptation for ordinary modes. The original `040.md` used a 3:4 creative canvas, but that historical example is not a silent default in the current Skill.

Photography in paired modes stays truthful, with only restrained grading and necessary environmental extension. Design-only and wallpapers still use the photograph as evidence but do not show it.

### Wallpaper packs: linked or independent

Wallpaper mode has no silent size default. Choose the common preset—phone `1440×3200`, iPad `2048×2732`, desktop `3840×2160`, watch `1024×1024`—or give labelled custom sizes.

- **Linked pack (recommended):** generate and approve the iPad anchor first; every other device references the original photo plus that same anchor and is recomposed for its canvas.
- **Independent set:** every device references only the source photograph and may explore freer anchor placement and figure interaction.

Linked never means cropped. All four files are separately generated, composed, and reviewed, with no iPad→phone→desktop→watch reference chain.

## Copy must produce a moment of recognition

Before generation, choose automatic copy, custom copy, or text-free output. Name the target language or locale whenever copy is present.

Automatic copy reads three levels: visible fact, relational tension, and the grounded implication they jointly suggest. It then uses precise naming, understatement, double meaning, light humour, or a small reversal to produce one extremely short handwritten remark.

It does not repeat the object name or reach for universal words such as “Dream”, “Memory”, or “Journey”. Copy must pass the unrelated-image swap test: if it works equally well on another photograph, it must be rewritten.

Finished user wording stays verbatim. A direction or editable draft is refined only while preserving audience, purpose, mandatory words, tone, and implication.

Language follows the intended audience rather than the command language:

```text
target market or audience > requested output language > direction language; if none is explicit, ask before generation
```

A Japanese edition uses natural Japanese, a Korean-audience edition uses natural Korean and correct spacing, a UK edition uses British English, and Arabic defaults to natural Modern Standard Arabic with genuine right-to-left composition. The Skill never guesses nationality from appearance, clothing, scenery, or signs and never uses pseudo-foreign text.

## Code guarantees geometry; image generation creates the artwork

The image model creates the truthful anchor, figures, whitespace, and copy. `scripts/compose_panel.py` only plans canvases, performs exact 50/50 raster composition, finalises dimensions, and audits results. It never fakes artwork with programmatic drawing.

```bash
python3 scripts/compose_panel.py --plan --layout top-bottom --source photo.png
python3 scripts/compose_panel.py --plan --layout left-right --size 2560x1440
python3 scripts/compose_panel.py --audit result.png --layout design-only --size 2048x2048
```

Exact top-bottom canvases need an even total height; left-right canvases need an even total width. Requested pixels are never silently changed.

## Get started

```bash
git clone https://github.com/nevertoday/xxd-panel-040.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-040" ~/.codex/skills/xxd-panel-040
```

Claude Code users may link the same directory to `~/.claude/skills/xxd-panel-040`. Restart the agent session after installation.

```text
$xxd-panel-040
Turn this photograph into a left-right composition. Derive the copy from the image and write it in natural Korean.
```

You may invoke the Skill with only a photograph. It first asks for the mode in a numbered multiline menu, then for copy settings; wallpaper mode also asks for linked/independent continuity and device sizes.

Full specifications:

- [Skill workflow](SKILL.md)
- [Chinese full prompt](references/xxd-panel-040-prompt.zh-CN.md)
- [English full prompt](references/xxd-panel-040-prompt.en.md)
- [Original style brief](references/040-source.md)

## Boundaries and trust

- Each photograph stays within its own task and never borrows subjects, colours, copy, or composition from other inputs, old results, or samples.
- Every invocation creates a fresh task directory; even identical sources and parameters must generate anew.
- Deliverables are PNG bitmaps, never SVG, HTML, Canvas, or programmatic-drawing substitutes.
- The configured bitmap bridge emits sanitised status only and does not expose providers, endpoints, headers, credentials, prompts, or response bodies.
- Ordinary modes return one image per source; wallpaper mode returns exactly four separate files, never a contact sheet.

Local composition needs Python 3 and Pillow. The safe bitmap bridge uses Python 3.11+ `tomllib`. Image generation still requires a host agent with built-in raster generation or an already configured compatible raster route.

## Repository

```text
xxd-panel-040/
├── SKILL.md
├── README.md / README.en.md / README.ja.md / README.ko.md / README.ar.md
├── agents/openai.yaml
├── assets/
│   ├── banner.svg
│   └── examples/
├── scripts/
│   ├── compose_panel.py
│   └── configured_imagegen.py
└── references/
    ├── xxd-panel-040-prompt.zh-CN.md
    ├── xxd-panel-040-prompt.en.md
    └── 040-source.md
```

## About XXD

XXD is the abbreviated brand name of Xiaoxiaodong. This project is created and maintained by [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## Support and Membership

### In-depth Consultation · CNY 299/hour

One-to-one consultation for using the Skills is billed at CNY 299 per hour. Contact Xiaoxiaodong through the WeChat QR code below to book.

### Xiaoxiaodong Skills User Community · CNY 99 to join

A one-time CNY 99 fee joins the community for workflow sharing, work discussion, and peer support. It does not include hourly one-to-one consultation. Include “Skills User Community” in your WeChat message.

### Knowledge Planet + Member Prompt Library · CNY 699/year

[Knowledge Planet](https://wx.zsxq.com/group/15554814142882) and the [XXD Member Prompt Library](https://vip.xiaoxiaodong.ai/) are one membership: **one annual payment unlocks both, with no second purchase required.**

1. Subscribe through [Knowledge Planet](https://wx.zsxq.com/group/15554814142882), then contact Xiaoxiaodong on WeChat for a Prompt Library redemption code.
2. Subscribe through the [Member Prompt Library](https://vip.xiaoxiaodong.ai/), then contact Xiaoxiaodong on WeChat for a Knowledge Planet invitation.

<p align="center">
  <a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD paid community WeChat QR code" width="320"></a>
</p>

<div align="center">

**Read the photograph first; then let the tiny figures tell its story.**

</div>

---

<div align="center">
  <h2>☕ Support this open-source project</h2>
  <p>If this project saved you time, a Star, a share, or a coffee helps keep it moving.</p>
  <table>
    <tr>
      <td align="center" width="240">
        <a href="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true"><img src="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true" alt="Support Xiaoxiaodong through Buy Me a Coffee" width="180"></a><br>
        <strong>Buy me a coffee</strong><br>
        <sub>Scan or open the QR code to support Xiaoxiaodong</sub>
      </td>
    </tr>
  </table>
  <p><sub>Support is entirely optional and never changes access to this open-source project.</sub></p>
</div>
