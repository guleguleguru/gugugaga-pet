<div align="center">

# 活泼版本咕咕嘎嘎

<img src="qa/guga-lively-cute-idle.gif" alt="Guga Lively 可爱待机预览" width="260">

**会在 Codex 里陪你工作的咕咕嘎嘎小企鹅。**<br>
软萌、犯困、会挥手，也会在你忙的时候悄悄动起来。新版用现有素材重新编排了待机、等待和审阅动作，更像一只会撒娇的小企鹅。

<p>
  <img alt="Codex Pet" src="https://img.shields.io/badge/Codex-Pet-111827?style=for-the-badge">
  <img alt="Guga Lively" src="https://img.shields.io/badge/Guga-Lively-f59e0b?style=for-the-badge">
  <img alt="Atlas" src="https://img.shields.io/badge/Atlas-8x9-22c55e?style=for-the-badge">
  <img alt="Format" src="https://img.shields.io/badge/Sprite-WEBP-38bdf8?style=for-the-badge">
</p>

[下载 ZIP](dist/guga-lively.zip) · [查看完整动作表](qa/contact-sheet.png) · [待机 MP4](qa/videos/idle.mp4) · [等待 MP4](qa/videos/waiting.mp4)

</div>

---

## 一句话介绍

`guga-lively` 是一个 Codex 自定义宠物包：黑色企鹅外套、圆滚滚身体、困困表情、快速小动作，还有挥手动作。

这版没有重新生成素材，只把现有帧重新编排成更可爱的循环：待机时会抱手、眨眼、闭眼笑；等待时会捂嘴、犯困、再恢复精神；审阅时会歪头观察。

## 立刻安装

### Windows PowerShell

```powershell
$petDir = "$HOME\.codex\pets\guga-lively"
New-Item -ItemType Directory -Force -Path $petDir | Out-Null
Invoke-WebRequest "https://github.com/guleguleguru/gugugaga-pet/raw/main/dist/guga-lively.zip" -OutFile "$env:TEMP\guga-lively.zip"
Expand-Archive "$env:TEMP\guga-lively.zip" -DestinationPath $petDir -Force
```

### macOS / Linux

```bash
mkdir -p ~/.codex/pets/guga-lively
curl -L "https://github.com/guleguleguru/gugugaga-pet/raw/main/dist/guga-lively.zip" -o /tmp/guga-lively.zip
unzip -o /tmp/guga-lively.zip -d ~/.codex/pets/guga-lively
```

安装后重新打开 Codex，选择或启用 `guga-lively`。

## 动作预览

<div align="center">
  <img src="qa/contact-sheet.png" alt="Guga Lively 全动作表" width="760">
</div>

| 状态 | 说明 |
| --- | --- |
| `idle` | 重新编排为开心、抱手、犯困、闭眼笑的可爱循环 |
| `running-right` / `running-left` | 左右移动 |
| `waving` | 招手互动 |
| `jumping` | 已恢复为之前那版经典挥手感动作 |
| `failed` | 按用户参考图替换过的委屈失败表情 |
| `waiting` | 重新编排为捂嘴、犯困、眨眼、恢复精神 |
| `running` | 通用移动循环 |
| `review` | 重新编排为歪头观察、闭眼思考、再回正 |

## 包里有什么

```text
guga-lively/
  pet.json
  spritesheet.webp

dist/
  guga-lively.zip

qa/
  guga-lively-waving.gif
  guga-lively-cute-idle.gif
  contact-sheet.png
  videos/idle.mp4
  videos/waiting.mp4
  videos/review.mp4
  videos/jumping.mp4
```

## 构建状态

- 最终安装包：`guga-lively/pet.json` + `guga-lively/spritesheet.webp`
- 精灵图规格：`1536 x 1872`，8 列 x 9 行
- 当前版本：已清理绿幕边缘，已恢复旧版挥手动作，并基于现有素材重编排了更可爱的 `idle`、`waiting`、`review`
- 校验结果：`review_ok=true`，`validation_ok=true`

## 鸣谢

这个宠物来自咕咕嘎嘎风格参考，并针对 Codex 自定义宠物格式整理成可直接安装的版本。
