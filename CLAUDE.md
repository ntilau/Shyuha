# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview
This repository is a research knowledge base focused on Rwanda's energy sector with three primary pillars: geothermal energy potential and development, solar power return on investment (ROI) analysis, and water pumping energy requirements. It contains markdown documents summarizing findings from various sources (JICA reports, MININFRA data, web research, and engineering analyses).

## Project Goals
The Shyuha project aims to:
- Consolidate research on Rwanda's geothermal energy prospects, including profitability and direct use applications.
- Analyze solar power ROI for various system sizes to inform investment decisions in Kigali City.
- Evaluate energy requirements and optimization opportunities for water pumping to support municipal water supply.
- Provide a reliable knowledge base for policymakers, investors, and researchers working on Rwanda's sustainable energy transition.

## File Structure
The repository is organized as follows:

**Root Level** (primary research documents):
- `SUMMARY.md` – Research findings on geothermal energy potential, prospect zones, exploration history, and development plans for Rwanda.
- `SOLAR_ROI_ANALYSIS.md` – Return on investment analysis for solar photovoltaic systems (100kW–10MW) targeting Kigali City.
- `WATER_PUMPING_ENERGY.md` – Analysis of energy required to pump water to Kigali City, including elevation head, friction losses, and cost estimates.
- `HOT_SPRINGS_ENERGY_PROFITABILITY.md` – Profitability and ROI analysis of harnessing Rwanda's hot springs energy for electrical generation and direct thermal applications.
- `PROJECT_TIMELINE.md` – Consolidated implementation timeline and specific activities for all project phases.
- `README.md` – Project overview and description of the Shyuha project.
- `BUSINESS_PLAN.md` – Comprehensive business plan for geothermal power generation in Rwanda (see also README.md for overview).
- `RISK_REGISTER.md` – Detailed risk assessment and mitigation strategies for the geothermal project.

**Supporting Directories**:
- `sources/` – External source documents referenced in the research:
  - `JICA.md` – Findings from the Japan International Cooperation Agency (JICA) project on Rwanda's Electricity Development Plan.
  - `MININFRA.md` – Summary of Rwanda's Ministry of Infrastructure (MININFRA) energy sector information (energy mix, access statistics).
- `archive/` – Contains archived versions of key analyses (e.g., solar ROI, water pumping energy) and an archive README.
- `evidence/` – Contains supporting evidence documents for geothermal energy:
  - `DIRECT_USE_OPTIONS.md` – Options for direct use of geothermal energy.
  - `GEOTHERMAL_RESOURCE_BASE.md` – Details on the geothermal resource base.
  - `NATIONAL_ENERGY_CONTEXT.md` – National energy context and policies.

## Using Claude Code in this Repository
Since this repository consists solely of markdown documentation, typical interactions with Claude Code involve:
- Reading files using the `Read` tool to review existing research.
- Writing or editing files using the `Write` and `Edit` tools to add new research or update existing content.
- Validating markdown quality using external tools (see below).

### Common Development Tasks
- **Markdown Validation**: Install and run markdown linter and spell checker to maintain quality.
  - Install tools (if desired): 
    ```bash
    npm install -g markdownlint-cli2
    npm install -g markdown-spellcheck
    ```
  - Lint markdown: `markdownlint-cli2 "**/*.md"`
  - Spell check: `markdown-spellcheck "**/*.md"`
- **Previewing Markdown**: To preview changes locally, you can use:
  - `pandoc <file>.md -t html -o preview.html` (requires pandoc)
  - Or open the file in a markdown viewer (e.g., Typora, VS Code preview).
- **Git Operations**: Standard Git commands for version control.
  - Check status: `git status`
  - View changes: `git diff`
  - Stage changes: `git add <file>` or `git add .`
  - Commit changes: `git commit -m "Descriptive message"`
  - Push to remote: `git push`
  - Pull updates: `git pull`
  - Create branch: `git switch -c <new-branch>`
  - Merge branch: `git merge <branch-name>`

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
- Focus contributions on the three pillars: geothermal energy, solar power ROI, and water pumping energy.
- When adding new research, ensure it aligns with Rwanda's energy sector goals and includes proper citations.

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