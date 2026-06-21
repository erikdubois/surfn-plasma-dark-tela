# Changelog

## 2026.06.21 — repo standardisation

### What Changed

Added the standard project docs and corrected the README, which falsely claimed the
repo shipped four themes and used the wrong install command.

### Technical Details

- README rewritten: ships only `Surfn-Plasma-Dark-Tela`, which
  `Inherits=Surfn-Plasma-Dark,breeze-dark,breeze,hicolor`. Install command corrected from
  `surfn-plasma-dark-tela-git` to `surfn-plasma-dark-tela-icons-git`. The theme needs
  `surfn-plasma-dark-icons-git` at runtime, but the recipe has `depends=()` — known gap.
- Added CLAUDE.md.

### Files Modified

- README.md, CHANGELOG.md, CLAUDE.md
