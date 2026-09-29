# GitHub Profile README Specification & Architecture

## Overview
This repository (`dubeyshantanu2/dubeyshantanu2`) serves as the official public GitHub profile showcase for Shantanu Dubey. It incorporates automated vector animations, live GitHub statistics, and scheduled CI/CD contribution graph rendering.

## Components

1. **Header Banner & Dynamic Typing SVG**:
   - Provider: `capsule-render` for animated SVG wave banner with Tokyo Night/cyber gradient.
   - Provider: `readme-typing-svg` cycling through core professional titles:
     - Software Engineer
     - React Native Developer
     - AI Systems Builder
     - Algorithmic Trading

2. **Core Tech Stack Grid**:
   - Provider: `skillicons.dev`
   - Technologies: React, TypeScript, Python, Tailwind CSS, PostgreSQL, Supabase, Redis, Docker, GitHub Actions.

3. **Live Analytics & Streak**:
   - Provider: `github-readme-stats` and `github-readme-streak-stats`
   - Palette: `tokyonight` dark theme
   - Metrics: Total contributions, stars, PRs, commits, current & longest streak, top languages.

4. **Contribution Snake Animation**:
   - Workflow: `.github/workflows/snake.yml`
   - Engine: `Platane/snk/svg-only@v3`
   - Target Branch: `output`
   - Render: Theme-aware `<picture>` element supporting GitHub dark and light modes.
