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

## Samples · From X

> [Xiaoxiaodong (@xiaoxiaodong01)](https://x.com/xiaoxiaodong01/status/2090834371423183135) · 21 August 2026<br>
> GPT2 × playful tiny figures × simplification × aesthetic prompt × VOL.040<br>
> The figures are not there merely to be cute. They act as another viewpoint inside the photograph—responding, commenting, or voicing what the scene leaves unsaid.

<table>
  <tr>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090834371423183135"><img src="./assets/examples/sample-01.jpg" alt="XXD Panel 040 sample 1"></a></td>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090834371423183135"><img src="./assets/examples/sample-02.jpg" alt="XXD Panel 040 sample 2"></a></td>
  </tr>
  <tr>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090834371423183135"><img src="./assets/examples/sample-03.jpg" alt="XXD Panel 040 sample 3"></a></td>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090834371423183135"><img src="./assets/examples/sample-04.jpg" alt="XXD Panel 040 sample 4"></a></td>
  </tr>
</table>

<p align="center"><a href="https://x.com/xiaoxiaodong01/status/2090834371423183135">View the original post and full prompt →</a></p>

These samples demonstrate the 040 aesthetic motive. Their subjects, figure actions, palette, copy, and earlier canvas ratio never become generation references or current defaults.

## Four combinable output modes

Choose one or several modes with `1`, `1+3`, `1,2,4`, or `all`; `all` produces seven separate PNGs per source. After mode selection and before generation, the Skill explicitly asks for the whole finished canvas: the original-prompt `3:4`, an explicit source-aspect choice, a common ratio, or custom ratio/exact pixels. Source dimensions are never applied silently.

| Mode | Canvas rule | Result |
| --- | --- | --- |
| `top-bottom` | user-confirmed whole canvas | one complete generation: high-fidelity source above, 040 design below, approximately 50/50 |
| `left-right` | user-confirmed whole canvas | one complete generation: high-fidelity source left, 040 design right, approximately 50/50 |
| `design-only` | user-confirmed whole canvas | 040 design fills the canvas; source remains invisible |
| `wallpaper-pack` | confirmed per device | separate phone, iPad, desktop, and children's-watch PNGs |

Paired modes use the source as a high-fidelity edit/reference input and one complete style prompt to generate the finished composition directly, so photography, design, colour, light, typography, and meaning can cohere. Deterministic composition is fallback-only: after one targeted complete-canvas retry fails, when pixel-identical source preservation is explicitly required, when the active route cannot realise the canvas, or for lossless final pixel calibration.

Wallpapers may be linked or independent. A linked pack approves one iPad anchor, then recomposes every other device from the original plus that same anchor. An independent pack gives each device only the original. Neither crops another device output nor chains derivatives.

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

## Complete-canvas first, raster-only delivery

The image model owns the aesthetics of the entire finished composition; paired layouts also default to one complete-canvas generation. `scripts/compose_panel.py` remains only for condition-based recovery, lossless pixel calibration, and read-only audit. It is not run pre-emptively and does not judge aesthetic success.

Every deliverable is a raster PNG and every invocation creates a fresh task under `~/Desktop/xxd/`. The configured image route exposes sanitised status only—never providers, endpoints, credentials, headers, prompts, responses, or account details. SVG, HTML, Canvas, diagrams, and programmatic drawing are not substitutes for the final artwork.

## Selectable controls and inline parameters

When the host provides genuine interactive controls, the Skill prefers card-style selection: output modes and ordinary output sizes are multi-select, while copy mode and wallpaper relationship are single-select. Size choices include auto-fit, source aspect, 1:1, 3:4, 4:3, 4:5, 5:4, 2:3, 3:2, 9:16, 16:9, 21:9, 5:7, 7:5, and custom ratios or pixels. Without an interactive control, it falls back to a clear multiline numbered menu rather than showing fake checkboxes.

Every setting can also be supplied as an inline variable:

```text
/xxd-panel-040 photo.jpg --mode top-bottom,design-only --size auto,3:4,9:16 --text auto --locale ja-JP
```

Supported parameters include `--mode`, repeatable or comma-separated `--size`, `--text auto|custom|none`, `--locale`, `--copy`, `--wallpaper linked|independent`, `--wallpaper-size`, and `--out`. Complete parameters skip all preflight questions; partial parameters trigger only the missing questions. Different aspect ratios are independently recomposed, and the four-device wallpaper pack remains a separate branch rather than being multiplied by ordinary sizes.

## Image-model priority

GPT Image 2 is the default first choice. It keeps this project's established workflow: high-fidelity source reference, explicit whole-canvas selection before generation, one complete-canvas generation for paired modes, and scripted composition only as a conditional fallback.

Seedance 5.0 Pro, Nano Banana Pro (Gemini Image Pro), Nano Banana 2 (Gemini Image Flash), or another compatible bitmap model may also be used when it is actually available through the current tools or configured routes and can satisfy source fidelity, whole-canvas ratio, target-language text, and linked-wallpaper multi-reference requirements. An alternative changes only the generation route; it must not change modes, canvas, copy, locale, wallpaper relationship, or the complete-canvas-first strategy.

If no suitable route is available, the Skill asks the user to enable an image-generation tool or provide an API key. User-provided credentials may be used for the current task without being echoed, displayed, logged, or exposed. They are not persisted, and provider, account, billing, or global route configuration is not modified, unless the user explicitly requests that configuration change.

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

You may invoke the Skill with only a photograph. It first asks for one or more modes in a numbered multiline menu, then for copy settings; wallpaper mode also asks for linked/independent continuity and device sizes.

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
- Each selected ordinary mode returns one file; selected `wallpaper-pack` adds four separate wallpapers. `all` returns seven PNGs per source across four sibling mode directories, never a contact sheet or overview.

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
