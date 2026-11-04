# Changelog

All notable changes to this project are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/).

## [1.0.0] - 2026-11-04

First personalized release of the al-folio v1.x starter — Nick Chin's personal academic site.

### Added

- Personal site identity and feature configuration in `_config.yml`
- Personal profile data: `_data/coauthors.yml`, `_data/socials.yml`, `_data/venues.yml`
- Personal bibliography in `_bibliography/papers.bib` (verified author orders)
- Personalized `_pages/about.md` and `_pages/cv.md`
- Project skills index (`.agents/skills/README.md`)

### Changed

- GitHub Actions workflows (`deploy`, `axe`, `broken-links-site`, `lighthouse-badger`, `copilot-setup-steps`, `upgrade-check`) adapted for this site
- `update-citations.yml`: cron schedule disabled until a repo `PAT` secret and Google Scholar ID are configured (re-enable notes inline)
- `requirements.txt`: pin `rendercv[full]==2.6.*` (2.7+ removed `cv.yml` fields the CV pipeline uses; migration note inline)
- `.gitignore`: exclude personal working files (`nick-profile.md`) and personal-assistant managed dirs (`.ai/`, `.memory/`, `.prds/`, `.tmp/`, `.reports/`, `.openchamber/`, `.opencode/`, `.zcode/`)

### Removed

- All al-folio demo content: blog posts, news, projects, teachings, books, and the dropdown/profiles/repositories/plugins pages
- `_data/repositories.yml` and demo assets, including large media (profile photos, tutorial video, sample audio, PDFs, notebooks)
