# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [PR-1](https://github.com/jgf-dev/agent-data/pull/1) - 2026-09-21

### Summary
This initial release establishes the `agent-data` project foundation, setting up a modern Python 3.13 environment with `uv` package management and integrating the **SKYLENAGE-GameCodeGym (V-GameGym)** benchmark dataset for code LLMs.

### Added
- **SKYLENAGE-GameCodeGym Dataset Support**: Integrated the game prompts benchmark dataset from ModelScope under `modelscope/game-prompts/`. Included tracking for the 27MB `pygame_seeds_2500_filtered.json` dataset file using Git LFS (Large File Storage).
- **ModelScope Download Utility**: Added a lightweight utility script `modelscope/game-prompts/get.py` to automate downloading the benchmark dataset locally via the ModelScope CLI.
- **Modern Python Environment**: Initialized the project with Python 3.13, configured `uv` as the package manager (`pyproject.toml`, `uv.lock`), and added a baseline `main.py` entrypoint.
- **Core Dependencies**: Configured dependencies in `pyproject.toml` for high-performance data operations and datasets:
  - `addict>=2.4.0` (easy dictionary access)
  - `datasets>=4.4.2` (robust dataset management)
  - `modelscope>=1.33.0` (model and dataset downloads)
  - `numpy>=2.4.0` (efficient numerical arrays and computing)
