# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A static GitHub Pages website presenting "The Advanced Persistent Threat: A Terminal Testimony" - a deeply personal narrative using cybersecurity metaphors to tell a story of struggle, faith, and recovery.

## Development

- **Local Preview**: Open `index.html` directly in browser (no build process)
- **Deploy**: Push to `main` branch - GitHub Pages deploys automatically

## Architecture

### Core Files
- `index.html` - Single-page narrative with 11 chapters + epilogue, includes JavaScript boot sequence
- `assets/styles/terminal.css` - Terminal aesthetics with CRT effects (scanlines, flicker, VT323 font)

### Visual Effects System
The CSS implements authentic CRT terminal effects:
- Scanline overlay animation
- Screen flicker effect
- Vignette darkening at edges
- Power-on animation
- Text glow effects
- Typed boot sequence with JavaScript

### Content Metaphor Mapping
- "theAdversary" = negative thoughts/addiction
- SSH sessions = internal dialogue
- File systems = identity/memory aspects
- Root access = spiritual authority
- Firewall = protective relationships

### CSS Classes
- `.command` / `.output` / `.comment` - Terminal styling
- `.keyword` / `.string` / `.function` - Syntax highlighting
- `.boot-sequence` / `.boot-line` - Boot animation
- `.chapter` - Content sections

## Important Considerations

1. **Static Site**: Pure HTML/CSS with minimal JavaScript for boot animation only
2. **Sensitive Content**: Personal stories about addiction, trauma, and recovery - handle with care
3. **Terminal Aesthetic**: Maintain VT323 font, green-on-black (#33ff33), and CRT effects
4. **Accessibility**: Includes `prefers-reduced-motion` and `prefers-contrast: high` support
