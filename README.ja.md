<p align="center">
  <img src="./assets/banner.svg" alt="XXD Panel 040 プロジェクトバナー" width="1200">
</p>

<div align="center">

# 🦁 XXD Panel 040

### 写真が本当に語っていることを、ひとつの実在アンカーと小さな線画の物語へ

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)
[![Four Modes](https://img.shields.io/badge/Modes-4-d75d32?style=flat-square)](#4つの出力を支えるひとつの物語ロジック)
[![Raster Output](https://img.shields.io/badge/Output-PNG-3c6f67?style=flat-square)](#境界と信頼性)

<a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <strong>日本語</strong> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

> 実在する主役 · 黒い線画の小人 · ミクロな物語 · 大きな余白

XXD Panel 040 は、Codex と互換 Agent のための画像生成 Skill です。写真にかわいい落書きを足すだけではありません。まず写真の中で何が最も記憶に残るべきかを読み取り、実在感と素材感を持つ視覚アンカーをひとつ残します。そこへ少数の黒い線画の小人を置き、元の物語に応答し、強調し、ときには小さく反転させます。

言葉も同じ意味から生まれ、小人が残したメモ、心の声、画面外のひと言のように働きます。

## なぜ 040 が必要なのか

「実物＋落書きの小人」は、簡単に汎用ステッカーへ崩れます。元写真に関係なく小人が登る、座る、手を振る。最大の切り抜き物体が自動的に主役になり、言葉は物の名前や励ましの句になる。

040 は順序を逆にします。

```text
事実を読む → 関係を見つける → 含意を絞る → 実在アンカーを選ぶ → 相互作用を設計する → 画外のひと言を書く
```

無関係な写真に替えてもアンカー、小人の動作、空間関係、色、言葉がほぼ成立するなら、それは 040 ではありません。

## 040 のビジュアル契約

- **実在アンカー：** 写真的な実在感、素材の個性、決定的な輪郭、元写真の主要色を保ち、主役を漫画化しません。
- **最低3つの固有手掛かり：** 輪郭、姿勢、方向、比率、素材、色、開口、負形、関係距離で元写真との対応を守ります。
- **1〜5人の黒線の小人：** 細く少し素朴な線で、動作は明確。すべての仕草が写真の含意に役立つ必要があります。
- **貼るのではなく関わる：** 小人はアンカーの縁、穴、表面、方向、尺度を実際の舞台として使います。
- **元写真の色＋明るい空間：** 色は実在アンカーが担い、心地よい淡色の背景に黒または濃いグレーの線を対比させます。
- **能動的な余白：** 飾りを増やさず、軽く、正確で、呼吸できる画面にします。
- **場面内の言葉：** 注釈、考え、画外の声として小人の動作と同じ物語を完成させます。

## 作例 · X より

> [小小東（@xiaoxiaodong01）](https://x.com/xiaoxiaodong01/status/2090834371423183135) · 2026年8月21日<br>
> GPT2 × ユーモラスな小人 × 簡略化 × 美学プロンプト × VOL.040<br>
> 小人は、かわいさを添えるためだけにいるのではありません。写真の内側にあるもう一つの視点として、応答し、つぶやき、画面が言葉にしなかった一言を代わりに語ります。

<table>
  <tr>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090834371423183135"><img src="https://pbs.twimg.com/media/HQQh3RYa8AA26OL.jpg?format=jpg&amp;name=large" alt="XXD Panel 040 作例 1"></a></td>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090834371423183135"><img src="https://pbs.twimg.com/media/HQQhAkAaAAAx9F4.jpg?format=jpg&amp;name=large" alt="XXD Panel 040 作例 2"></a></td>
  </tr>
  <tr>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090834371423183135"><img src="https://pbs.twimg.com/media/HQQhzP5acAAMsin.jpg?format=jpg&amp;name=large" alt="XXD Panel 040 作例 3"></a></td>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090834371423183135"><img src="https://pbs.twimg.com/media/HQQiRA6aIAACbc5.jpg?format=jpg&amp;name=large" alt="XXD Panel 040 作例 4"></a></td>
  </tr>
</table>

<p align="center"><a href="https://x.com/xiaoxiaodong01/status/2090834371423183135">元の投稿と完全なプロンプトを見る →</a></p>

これらの作例は 040 の美学的動機を示すためのものです。作例の被写体、小人の動作、配色、文案、旧来の画面比率を生成参照や現在の既定値として固定することはありません。

## 4つの出力を支えるひとつの物語ロジック

4つのモードは単独でも複数でも選択できます。`1`、`1+3`、`1、2、4`、`全部` と返信すると、Skill が重複を除き 1→4 の順で実行します。各モードは別々のタスクフォルダに独立出力され、一覧画像にはまとめません。`全部` は元写真1枚につき7点（通常3モード各1点＋壁紙4点）です。サイズはモード名付きで同時指定でき、未指定の通常モードは元画像に適応します。文案は既定で選択モード間に共通し、モード別指定も可能です。

| モード | サイズ方針 | 成果物 |
| --- | --- | --- |
| `top-bottom` | 元画像適応 | 上に完全な元写真、下に 040 の物語。両パネルは元画像サイズを保ち、厳密に 50/50 |
| `left-right` | 元画像適応 | 左に完全な元写真、右に 040 の物語。両パネルは元画像サイズを保ち、厳密に 50/50 |
| `design-only` | 元画像適応 | 元写真を見せず、変化デザインだけを表示。元画像の比率と寸法を維持 |
| `wallpaper-pack` | 端末別4サイズ | スマートフォン、iPad、デスクトップ、子ども用ウォッチの PNG を個別出力 |

優先順位は、正確な指定ピクセル > 指定比率／用途 > 通常モードの元画像適応です。原稿 `040.md` の 3:4 は初期の制作画角であり、現在の暗黙の既定値ではありません。

ペアモードの写真は、抑制した調色と必要最小限の環境拡張だけで忠実さを保ちます。デザイン単独と壁紙では写真を根拠として使いますが、原片は表示しません。

### 壁紙セット：連動または独立

壁紙に暗黙のサイズ既定値はありません。一般プリセットはスマートフォン `1440×3200`、iPad `2048×2732`、デスクトップ `3840×2160`、ウォッチ `1024×1024`。端末別のカスタムサイズも指定できます。

- **連動セット（推奨）：** まず iPad の基準作品を生成・承認し、残り3枚は元写真＋同じ基準作品を参照して各画面に再構成します。
- **独立4作品：** 各端末は元写真だけを参照し、アンカー位置や小人の関わりを自由に探れます。

連動は切り抜きではありません。4枚を個別に生成、構成、検査し、iPad→スマートフォン→デスクトップ→ウォッチの順に参照を連鎖させません。

## 言葉は画面に「なるほど」を生む

生成前に、自動文案、カスタム文案、文字なしを選びます。文字を入れる場合は対象言語または地域も指定します。

自動文案は、見えている事実、関係の緊張、その組み合わせが示す根拠ある含意を読みます。その後、正確な命名、控えめな表現、二重の意味、軽いユーモア、小さな反転から、非常に短い手書きのひと言を作ります。

物の名前を言い直したり、「夢・記憶・旅」のような万能語に逃げたりしません。無関係な写真にも同じ強さで使える言葉は書き直します。

ユーザーが完成稿を渡した場合は一字一句保ちます。方向や編集可能な草稿の場合だけ、対象、目的、必須語、語調、含意を守りながら磨きます。

言語は命令文ではなく、想定する読者に従います。

```text
対象市場・読者 > 指定された成果物言語 > 方向指示の言語；不明なら生成前に確認
```

日本版は自然な現代日本語、韓国向けは自然な韓国語と正しい分かち書き、英国版は英国英語、アラビア語版は原則として自然な現代標準アラビア語と正しい右から左の組版を使います。外見、服装、風景、看板から国籍を推測せず、雰囲気づくりの偽外国語も使いません。

## 正確な幾何はコード、作品は画像生成

画像モデルが実在アンカー、小人、余白、文字を作ります。`scripts/compose_panel.py` は画布計画、厳密な 50/50 ラスター合成、最終寸法、監査だけを担当し、プログラム描画で作品を偽装しません。

```bash
python3 scripts/compose_panel.py --plan --layout top-bottom --source photo.png
python3 scripts/compose_panel.py --plan --layout left-right --size 2560x1440
python3 scripts/compose_panel.py --audit result.png --layout design-only --size 2048x2048
```

正確な上下構成は総高さ、左右構成は総幅が偶数である必要があります。指定ピクセルは勝手に変更されません。

## 使い始める

```bash
git clone https://github.com/nevertoday/xxd-panel-040.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-040" ~/.codex/skills/xxd-panel-040
```

Claude Code では同じフォルダを `~/.claude/skills/xxd-panel-040` にリンクできます。インストール後に Agent セッションを再起動してください。

```text
$xxd-panel-040
この写真を左右二連にしてください。文案は写真の意味から作り、自然な韓国語を使ってください。
```

写真だけでも呼び出せます。番号付きの複数行メニューでモードと文字設定を確認し、壁紙では連動／独立と端末サイズも確認します。

詳細仕様：

- [Skill ワークフロー](SKILL.md)
- [中国語の完全プロンプト](references/xxd-panel-040-prompt.zh-CN.md)
- [英語の完全プロンプト](references/xxd-panel-040-prompt.en.md)
- [元のスタイル指示](references/040-source.md)

## 境界と信頼性

- 各写真は独立したタスク内だけで使い、他の入力、旧成果物、作例の主題、色、文案、構図を借りません。
- 呼び出すたびに新しいタスクフォルダを作り、同じ原画像と条件でも新たに生成します。
- 成果物は PNG ビットマップであり、SVG、HTML、Canvas、プログラム描画の代替物ではありません。
- 設定済みビットマップブリッジは匿名化した状態だけを返し、プロバイダー、エンドポイント、ヘッダー、認証情報、プロンプト、応答本文を表示しません。
- 選択した通常モードごとに1点を返し、`wallpaper-pack` を選ぶと独立壁紙4点を追加します。`全部` は元写真1枚につき7点を4つの同階層モードフォルダへ出力し、一覧コラージュにはまとめません。

ローカル合成には Python 3 と Pillow が必要です。安全なビットマップブリッジは Python 3.11+ の `tomllib` を使用します。画像生成には、ホスト Agent の内蔵ラスター生成機能または設定済みの互換ルートが必要です。

## リポジトリ

```text
xxd-panel-040/
├── SKILL.md
├── README.md / README.en.md / README.ja.md / README.ko.md / README.ar.md
├── agents/openai.yaml
├── assets/banner.svg + examples/
├── scripts/compose_panel.py + configured_imagegen.py
└── references/xxd-panel-040-prompt.zh-CN.md + xxd-panel-040-prompt.en.md + 040-source.md
```

## XXD について

XXD は小小東（Xiaoxiaodong）のブランド名の略称です。このプロジェクトは [@xiaoxiaodong01](https://x.com/xiaoxiaodong01) が制作・管理しています。

## サポートと会員制度

### 個別深度相談 · 1時間 CNY 299

Skills 利用に関する一対一相談は1時間 CNY 299です。下の WeChat QR コードから予約してください。

### Xiaoxiaodong Skills ユーザー交流グループ · CNY 99

一度 CNY 99 を支払うと、ワークフロー共有、作品相談、ユーザー同士の支援を行う交流グループに参加できます。時間制の個別相談は含まれません。

### 知識星球＋会員プロンプトライブラリ · 年額 CNY 699

[知識星球](https://wx.zsxq.com/group/15554814142882)と[XXD 会員プロンプトライブラリ](https://vip.xiaoxiaodong.ai/)は同じ会員権です。**一度の年額決済で両方を利用でき、二重の購入は不要です。**

1. 知識星球で加入後、WeChat でプロンプトライブラリの交換コードを受け取る。
2. プロンプトライブラリで加入後、WeChat で知識星球への招待を受け取る。

<p align="center">
  <a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD 有料サービス WeChat QR コード" width="320"></a>
</p>

<div align="center">

**まず写真を読み、小人にその物語を語らせる。**

</div>

---

<div align="center">
  <h2>☕ オープンソースプロジェクトを支援</h2>
  <p>このプロジェクトが時間の節約になったなら、Star、共有、コーヒー一杯で継続を支援できます。</p>
  <table><tr><td align="center" width="240">
    <a href="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true"><img src="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true" alt="Buy Me a Coffee で Xiaoxiaodong を支援" width="180"></a><br>
    <strong>Buy me a coffee</strong><br><sub>QR コードを読み取るか開いて支援できます</sub>
  </td></tr></table>
  <p><sub>支援は任意であり、このオープンソースプロジェクトの利用権には影響しません。</sub></p>
</div>
