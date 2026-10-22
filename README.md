# Wolfgangs Claude Skills

Ein Plugin-Marktplatz für Claude mit allen Skills aus Raphis Liste (126 Stück). Die meisten Skills liegen als Kopie direkt in diesem Repo (unter `plugins/`, mit der Lizenz des Originals), weil die Claude App keine Verweise auf Unterordner oder feste Versionen anderer Repos lädt. instagram-agent, humanizer, taste-skill und animated-website werden direkt aus den Original-Repos geladen und aktualisieren sich automatisch. HyperFrames ist bewusst auf v0.8.184 eingefroren, weil spätere Versionen hyperframes-core, talking-head-recut und embedded-captions entfernt haben.

## Inhalt

| Plugin | Skills | Quelle |
|---|---|---|
| `eigene-skills` | autopilot, reel-viral-playbook, loopsystem, podcast-schnitt-premiere | dieses Repo |
| `hyperframes` | hyperframes, hyperframes-core, hyperframes-cli, media-use, talking-head-recut, embedded-captions und weitere | [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) |
| `instagram-agent` | 13 Skills: ig-reel, ig-carousel, ig-caption, ig-story, ig-plan, ig-viral, ig-audit, ig-profile, ig-comment, ig-reply, ig-dm, ig-human, ig-repurpose | [Jakeschincariol/instagram-agent-skill](https://github.com/Jakeschincariol/instagram-agent-skill) |
| `agency-agents` | 16 Marketing-Skills (LinkedIn, Social, TikTok, Content, YouTube, Short-Video, Podcast, E-Mail, SEO, AEO, KI-Zitierungen, Agentic Search, PR, Buch, Growth) | [bestagentkits/agency-skills](https://github.com/bestagentkits/agency-skills), basierend auf [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) |
| `taste-skill` | taste-skill (früher design-taste-frontend) | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) |
| `taste-skill-classics` | design-taste-frontend-v1, industrial-brutalist-ui | [Leonxlnx/taste-skill-classics](https://github.com/Leonxlnx/taste-skill-classics) |
| `brandkit` | brandkit | [Leonxlnx/imagegen-skills](https://github.com/Leonxlnx/imagegen-skills) |
| `emil-design-eng` | emil-design-eng | [emilkowalski/skill](https://github.com/emilkowalski/skill) |
| `animated-website` | animated-website | [sva-admin/animated-website](https://github.com/sva-admin/animated-website) |
| `humanizer` | humanizer | [blader/humanizer](https://github.com/blader/humanizer) |
| `agency-sales` | 8 Sales-Skills | [bestagentkits/agency-skills](https://github.com/bestagentkits/agency-skills) |
| `agency-paid-media` | 6 Paid-Media-Skills | [bestagentkits/agency-skills](https://github.com/bestagentkits/agency-skills) |
| `agency-projektmanagement` | 6 Projektmanagement-Skills | [bestagentkits/agency-skills](https://github.com/bestagentkits/agency-skills) |
| `ecc-dev-skills` | 11 Entwicklungs-Skills (Everything Claude Code v1.10.0) | [affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code) |
| `ecc-dev-commands` | 15 Slash Commands (/plan, /tdd, /verify und weitere) | [affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code) |
| `dokument-skills` | docx, pdf, pptx, xlsx, frontend-design (nur für Claude Code nötig, in der App eingebaut) | [anthropics/skills](https://github.com/anthropics/skills) |

## Installation

### 1. In der Claude App (einmal, gilt dann überall)

1. Claude im Browser oder in der Desktop-App öffnen.
2. Links **Anpassen** → **Plugins** → **Hinzufügen** → **Marktplatz hinzufügen** → **Aus einem Repository hinzufügen**.
3. `doubleukay10/claude-skills` eingeben.
4. Die gewünschten Plugins installieren (`dokument-skills` in der App weglassen).

Plugins aus der App werden im Konto gespeichert und erscheinen automatisch in Claude Code auf jedem Gerät, auf dem du mit demselben Konto angemeldet bist (Claude Code ab Version 2.1.273).

### 2. Claude Code auf Mac oder Windows (falls die Synchronisation nicht greift)

```bash
claude plugin marketplace add doubleukay10/claude-skills
claude plugin install eigene-skills@wolfgang-skills
claude plugin install hyperframes@wolfgang-skills
claude plugin install instagram-agent@wolfgang-skills
claude plugin install agency-agents@wolfgang-skills
claude plugin install taste-skill@wolfgang-skills
claude plugin install taste-skill-classics@wolfgang-skills
claude plugin install brandkit@wolfgang-skills
claude plugin install emil-design-eng@wolfgang-skills
claude plugin install humanizer@wolfgang-skills
claude plugin install animated-website@wolfgang-skills
claude plugin install agency-sales@wolfgang-skills
claude plugin install agency-paid-media@wolfgang-skills
claude plugin install agency-projektmanagement@wolfgang-skills
claude plugin install ecc-dev-skills@wolfgang-skills
claude plugin install ecc-dev-commands@wolfgang-skills
claude plugin install dokument-skills@wolfgang-skills
```

Aktualisieren: `claude plugin marketplace update wolfgang-skills`

## Nicht enthalten

- **Adobe-Skills** (6) und **Plugin Management** (cowork-plugin-customizer, create-cowork-plugin): direkt im Anthropic-Verzeichnis unter Anpassen → Plugins installieren.
- **Claude Standard-Skills** (docs, deep-research, skill-creator, Browser, Computer use usw.): sind in der Claude App bereits eingebaut.

## Eigene Skills ändern

Dateien unter `plugins/eigene-skills/skills/<name>/SKILL.md` bearbeiten, Version in `plugins/eigene-skills/.claude-plugin/plugin.json` erhöhen, committen und pushen.
