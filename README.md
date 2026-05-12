# visual-style

> Create, extract, and apply portable visual design systems via visual-style.md files. Colors, typography, layout, motion, and mood — one file any AI tool can consume.

**Free. Apache 2.0. Bring-your-own-Claude.**

## What this is

A Claude skill bundle — a sanitized, attributed, downloadable subject-matter expert that runs inside Claude Code, Claude Desktop, or any Claude-API workflow. Drop it in, invoke it, get answers grounded in real practitioner content rather than generic LLM consensus.

Use to create a visual-style.md from scratch, extract a style from a URL/PDF/video reference, or apply a style to HeyGen videos, HTML slides, Figma, or paper.design output.

## Install

```bash
# Claude Code plugin install (one-line)
claude plugin install visual-style --from https://fadaly.net/downloads/skills/visual-style.zip
```

Or clone this repo into your Claude skills directory:

```bash
git clone https://github.com/MomoFadaly/visual-style.git ~/.claude/skills/visual-style
```

Or download the zip from [fadaly.net/skills/visual-style](https://fadaly.net/skills/visual-style) (the per-skill landing page on fadaly.net) and extract into `~/.claude/skills/`.

## What's in the bundle

| File | Size |
|---|---|
| `references/connectors/figma.md` | 6KB |
| `references/connectors/heygen-video-agent.md` | 4KB |
| `references/connectors/html-slides.md` | 5KB |
| `references/connectors/paper-design.md` | 4KB |
| `references/extractors/from-pdf.md` | 8KB |
| `references/extractors/from-video.md` | 7KB |
| `references/extractors/from-website.md` | 7KB |
| `references/gallery/game-boy-color.visual-style.md` | 5KB |
| `references/gallery/heygen-ai-video.visual-style.md` | 5KB |
| `references/gallery/mueller-brockmann-swiss.visual-style.md` | 4KB |
| `references/gallery/neville-brody-industrial.visual-style.md` | 4KB |
| `references/gallery/saul-bass-cinematic.visual-style.md` | 4KB |
| `references/spec.md` | 9KB |
| `references/templates/full.visual-style.md` | 3KB |
| `references/templates/minimal.visual-style.md` | 584B |
| `SKILL.md` | 6KB |
| `thumb.png` | 1.81MB |

Total: 1.89MB

## Sources

This SME's canon was built from these practitioners. Every claim in the canon is attributed.

- Curated gallery of design movements (Swiss, Saul Bass, Game Boy, Neville Brody, etc.)
- Design system documentation patterns from Brad Frost, Audrey Hacq, Nathan Curtis

Primary sources (official documentation, peer-reviewed research) take priority over practitioner consensus, which takes priority over single-source claims. Confidence tiers are tagged inline.

## How it works

Claude reads `SKILL.md` as the system instructions for the skill. Supporting files (`canon.md`, `mental-models.md`, etc.) are loaded as reference material when the skill needs to answer off the cuff or cite a specific source.

When you ask a question this SME covers, Claude pulls the relevant canon entry, names its source, tags its confidence level, and pushes back if your question contradicts canon.

## Confidence levels

- **Verified** — primary source + practitioner corroboration. Treat as fact.
- **Confirmed** — practitioner consensus across credible voices, no primary contradiction. Defended best-practice.
- **Plausible** — single-source or thin evidence. Working hypothesis until validated.
- **Disputed** — credible voices disagree. The SME names the camps and gives you the lens to decide.
- **Stale** — once true, contradicted by current docs/data. Flagged for refresh.

## License

Apache License 2.0. See [LICENSE](LICENSE).

You are free to use, modify, redistribute, and build on this skill. Attribution to the original practitioners (named in `sources.md` or `SKILL.md`) is morally required even if not legally; their work made the canon possible.

## Built by

[Mo Fadaly](https://fadaly.net) — AI intrapreneur, runs Claude skills in production.

This is one of a series. See the [full catalog at fadaly.net/work](https://fadaly.net/work).
