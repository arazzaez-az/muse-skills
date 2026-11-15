# muse-skills

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![GitHub stars](https://img.shields.io/github/stars/arazzaez-az/muse-skills?style=social)
![Skills](https://img.shields.io/badge/skills-16-blue)

A collection of agent skills installed in Muse, published in English.

## Table of contents

- [What's inside](#whats-inside)
  - [Custom skills (my own)](#custom-skills-my-own)
  - [Third-party skills](#third-party-skills)
- [How to use](#how-to-use)
- [License](#license)

## What's inside

### Custom skills (my own)

| Skill | What it does |
| --- | --- |
| `launchpad_token_research` | Researches a launchpad token's holder distribution from the full Transfer-event history (never from recent trades alone), checks liftoff progress, momentum and sellability, and reports only verified figures before a buy decision. |
| `cloud_browser_preflight` | Checks whether a cloud-browser task can actually run before claiming progress, and hands a blocked task back cleanly. |

### Third-party skills

#### Binance Agentic Wallet

| Skill | What it does |
| --- | --- |
| `binance-agentic-wallet` | The official skill for the Binance Agentic Wallet — sign in, check balances, and transact on supported mainnet chains. See [Binance](https://www.binance.com/) for the original. |

#### Remotion (13 skills)

The official skill set for building videos with Remotion. See [Remotion](https://www.remotion.dev/) and [remotion-dev/skills](https://github.com/remotion-dev/skills) for the originals.

| Skill | What it does |
| --- | --- |
| `remotion-best-practices` | Patterns and pitfalls for writing maintainable Remotion projects. |
| `remotion-captions` | Adds word-accurate captions and subtitles to a video. |
| `remotion-create` | Scaffolds a new Remotion project from scratch. |
| `remotion-docs` | Looks up Remotion documentation and API references. |
| `remotion-interactivity` | Builds interactive videos with clickable elements and state. |
| `remotion-license` | Explains Remotion licensing and the company-license rules. |
| `remotion-maps` | Renders animated maps inside a video. |
| `remotion-markup` | Turns Markdown and HTML markup into video scenes. |
| `remotion-multimedia` | Works with images, audio, and video assets in a composition. |
| `remotion-render` | Renders a composition to MP4/WebM with the right settings. |
| `remotion-saas` | Patterns for building a video-rendering SaaS on Remotion. |
| `remotion-studio` | Uses the Remotion Studio for previewing and editing. |
| `remotion-upgrade` | Upgrades a Remotion project between major versions safely. |

The third-party skills above are republished here as a personal collection for convenience; they remain the work of their original authors. If you need the latest version, install them from their official sources.

## How to use

These are Muse agent skills. Drop a skill folder into your skills directory (for example `~/.agents/skills/`) and Muse will pick it up. Each skill has a `SKILL.md` that describes when to use it and how it works.

```bash
# Example: install one skill
cp -r skills/launchpad_token_research ~/.agents/skills/
```

## License

The custom skills in this repository are shared freely for personal use. Third-party skills keep their original licenses — see each skill's own files for details.
