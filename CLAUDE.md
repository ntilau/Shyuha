# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview
This repository is a research knowledge base focused on Rwanda's energy sector, particularly geothermal energy, solar power ROI, and water pumping energy requirements. It contains markdown documents summarizing findings from various sources (JICA reports, MININFRA data, web research, and engineering analyses).

## File Structure
- `JICA.md` – Findings from the Japan International Cooperation Agency (JICA) project on Rwanda's Electricity Development Plan.
- `MININFRA.md` – Summary of Rwanda's Ministry of Infrastructure (MININFRA) energy sector information (energy mix, access statistics).
- `SUMMARY.md` – Research findings on geothermal energy potential, prospect zones, exploration history, and development plans for Rwanda.
- `SOLAR_ROI_ANALYSIS.md` – Return on investment analysis for solar photovoltaic systems (100kW–10MW) targeting Kigali City.
- `WATER_PUMPING_ENERGY.md` – Analysis of energy required to pump water to Kigali City, including elevation head, friction losses, and cost estimates.
- `README.md` – Project overview and description of the Shyuha project.
- `.claude/settings.local.json` – Permission settings for Claude Code (allowed Bash and WebFetch commands).

## Common Development Tasks
Since this repository consists primarily of markdown documentation, typical tasks involve creating, editing, and validating documents.

### Git Commands
- Check status: `git status`
- View changes: `git diff`
- Stage changes: `git add <file>` or `git add .`
- Commit changes: `git commit -m "Descriptive message"`
- Push to remote: `git push`
- Pull updates: `git pull`
- Create branch: `git switch -c <new-branch>`
- Merge branch: `git merge <branch-name>`

### Markdown Linting and Spell Checking
Install tools via npm (if desired):
- `npm install -g markdownlint-cli2`
- `npm install -g markdown-spellcheck`

Then run:
- Lint markdown: `markdownlint-cli2 "**/*.md"`
- Spell check: `markdown-spellcheck "**/*.md"`

### Previewing Markdown
To preview changes locally, you can use:
- `pandoc <file>.md -t html -o preview.html` (requires pandoc)
- Or open the file in a markdown viewer (e.g., Typora, VS Code preview).

### Adding New Research Files
When adding a new markdown file:
1. Ensure the file follows the naming convention: descriptive name with `.md` extension.
2. Include a brief summary of the source and date of research.
3. Cite sources with hyperlinks where possible.
4. After writing, run lint and spell check to maintain quality.
5. Commit with a clear message describing the addition.

## Repository-Specific Notes
- The `.claude/settings.local.json` file grants Claude Code permission to run specific Git and GitHub CLI commands (e.g., `git branch`, `git push`, `gh auth`, `gh repo`) and to fetch from certain domains (www.reg.rw, africangeothermal.org, downloads.unido.org, rwandadispatch.com). These permissions are already configured; no further action is needed.
- There are no build scripts, test suites, or compiled code in this repository. Validation focuses on prose quality, proper citations, and consistent formatting.

## Guidelines for Contributions
- Keep content factual and well-sourced; prefer primary sources (government reports, peer-reviewed papers, official project documents).
- When summarizing web content, include the URL as a hyperlink.
- Use consistent heading styles (e.g., `##` for major sections, `###` for subsections).
- Avoid duplication; if a topic is covered across multiple files, consider cross-referencing with relative links.
- When updating existing files, preserve the original intent and clearly note any changes in the commit message.

## Example Workflow
1. Research a new topic (e.g., wind energy potential in Rwanda).
2. Draft a new markdown file (e.g., `WIND_ENERGY_POTENTIAL.md`) with sections: Overview, Data Sources, Findings, Implications, Sources.
3. Run `markdownlint-cli2` and `markdown-spellcheck` to check for issues.
4. Review the rendered output (via pandoc or editor preview).
5. Stage the file: `git add WIND_ENERGY_POTENTIAL.md`.
6. Commit: `git commit -m "Add wind energy potential analysis for Rwanda"`.
7. Push: `git push`.

## Maintenance
- Periodically check for broken links in markdown files.
- Update statistics or figures when newer data becomes available.
- Ensure that all claims are backed by credible sources; tag any unverified claims appropriately.