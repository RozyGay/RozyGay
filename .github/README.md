# GitHub Workflows

This repository contains GitHub Actions workflows that enhance the profile README.

## Snake Animation Workflow

The `snake.yml` workflow generates an animated SVG of the contribution graph in the form of a snake eating the contributions.

### Features:
- **Automatic Generation**: Runs daily at midnight UTC
- **Manual Trigger**: Can be triggered manually from the Actions tab
- **Dark/Light Mode**: Generates both dark and light theme versions
- **Auto-deployment**: Automatically pushes generated files to the `output` branch

### Setup Notes:
1. The workflow uses `GITHUB_TOKEN` which is automatically provided by GitHub
2. Generated files are stored in the `output` branch
3. The snake animation will appear in the profile README after the first successful run

### Files Generated:
- `github-contribution-grid-snake.svg` - Light theme version
- `github-contribution-grid-snake-dark.svg` - Dark theme version

The profile README automatically switches between themes based on user preferences.