# CLAUDE.md — surfn-plasma-dark-tela

## Project overview

Standalone repo for the **Surfn Plasma Dark Tela** icon theme, split out of the
`erikdubois/surfn` monolith. See [README.md](./README.md).

## Current state

Ships one theme: `usr/share/icons/Surfn-Plasma-Dark-Tela/`. Packaged as
`surfn-plasma-dark-tela-icons-git` (recipe in `~/KIRO-PKG-BUILD-ICONS/surfn-plasma-dark-tela/`).

## Patterns & decisions

- Theme dir PascalCase; repo/package lowercase. `icon-theme.cache` rebuilt by the pacman
  hook on install. Theme `Inherits=Surfn-Plasma-Dark,breeze-dark,breeze,hicolor`, so it
  needs `surfn-plasma-dark-icons-git` at runtime — but the recipe has `depends=()` (known
  gap). Bash scripts follow the canonical Kiro template.
