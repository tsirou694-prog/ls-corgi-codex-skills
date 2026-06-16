# LS Corgi Codex Skills

LS Corgi Codex Skills is a small open-source skill pack for generating Chinese article illustrations with the original LS / LS-Q corgi IP.

It contains two Codex skills:

- `ls-corgi-illustrations-v2`: default version, LS-Q chibi 3D cartoon corgi style.
- `ls-corgi-illustrations`: legacy v1, flat color-block corgi illustration style.

## What This Skill Does

These skills help Codex turn Chinese articles, notes, scripts, and explanations into 16:9 article illustrations. They define:

- LS / LS-Q character identity and visual consistency.
- Article illustration strategy and shot-list rules.
- Prompt templates for single-image generation.
- QA checks for common failures such as over-dense diagrams, decorative-only mascots, unreadable labels, or style drift.

## Install On macOS

Install the default LS-Q v2 skill from GitHub:

```bash
python ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo YOUR_GITHUB_USERNAME/ls-corgi-codex-skills \
  --path skills/ls-corgi-illustrations-v2
```

Install both v2 and legacy v1:

```bash
python ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo YOUR_GITHUB_USERNAME/ls-corgi-codex-skills \
  --path skills/ls-corgi-illustrations-v2 \
  --path skills/ls-corgi-illustrations
```

Restart Codex after installation.

## Manual Install

Clone this repository and copy the skill folders into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R skills/ls-corgi-illustrations-v2 ~/.codex/skills/
cp -R skills/ls-corgi-illustrations ~/.codex/skills/
```

Restart Codex after copying.

## Usage

Example prompt:

```text
使用 LS skill 为这篇文章做 4 张正文配图，先给 shot list，再生成第一张。
```

For the default v2 style:

```text
使用 LS-Q 风格为这篇文章生成第一张正文配图。
```

For the legacy v1 style:

```text
使用老版 LS 扁平风为这篇文章生成第一张正文配图。
```

## Repository Structure

```text
skills/
  ls-corgi-illustrations-v2/
    SKILL.md
    references/
    assets/reference-ip/
  ls-corgi-illustrations/
    SKILL.md
    references/
    assets/reference-ip/
```

## IP And License

The LS / LS-Q corgi character, reference images, skill instructions, and prompt templates included in this repository are original assets provided by the copyright holder and released under the MIT License in this repository.

See [LICENSE](LICENSE) and [NOTICE](NOTICE).

