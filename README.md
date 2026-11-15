# muse-skills

A collection of agent skills installed in Muse, published in English.

## What's inside

### Custom skills (my own)

| Skill | What it does |
| --- | --- |
| `launchpad_token_research` | Researches a launchpad token's holder distribution from the full Transfer-event history (never from recent trades alone), checks liftoff progress, momentum and sellability, and reports only verified figures before a buy decision. |
| `cloud_browser_preflight` | Checks whether a cloud-browser task can actually run before claiming progress, and hands a blocked task back cleanly. |

### Third-party skills (included for convenience, with attribution)

| Skill | Source |
| --- | --- |
| `binance-agentic-wallet` | Binance Agentic Wallet — the official skill for the Binance Agentic Wallet. See [Binance](https://www.binance.com/) for the original. |
| `remotion-*` (13 skills) | Remotion — the official skill set for building videos with Remotion (best-practices, captions, create, docs, interactivity, license, maps, markup, multimedia, render, saas, studio, upgrade). See [Remotion](https://www.remotion.dev/) and [remotion-dev/skills](https://github.com/remotion-dev/skills) for the originals. |

The third-party skills above are republished here as a personal collection for convenience; they remain the work of their original authors. If you need the latest version, install them from their official sources.

## How to use

These are Muse agent skills. Drop a skill folder into your skills directory (for example `~/.agents/skills/`) and Muse will pick it up.

## License

The custom skills in this repository are shared freely for personal use. Third-party skills keep their original licenses — see each skill's own files for details.
