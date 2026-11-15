# Changelog

本项目的所有显著变更都会记录在这个文件里。

格式基于 [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)，
版本号遵循 [Semantic Versioning](https://semver.org/spec/v2.0.0.html)。

## [Unreleased]

### Added

- README 顶部增加 CI badge，新增「发布产物」章节（三平台 deb/AppImage/rpm、NSIS/msi、dmg 说明）
- 新增本 CHANGELOG（keep-a-changelog 格式）

## [0.1.0] - 2026-11-15

### Added

- Tauri 2 桌面应用模板：React 19 + TypeScript 6（strict）+ Tailwind CSS v4 + shadcn/ui（radix-nova，neutral）
- 测试：vitest（jsdom）前端测试 + cargo test Rust 测试
- CI（GitHub Actions）：frontend 矩阵（ubuntu/windows）跑类型检查 + 测试 + 构建；rust job 跑 cargo test
- 发布流水线：`v*` tag 触发，校验 tag 版本与 `src-tauri/tauri.conf.json` version 一致后，tauri-action 三平台出包（deb/AppImage/rpm、NSIS/msi、dmg）

[Unreleased]: https://github.com/ecoreal/tauri-starter/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/ecoreal/tauri-starter/releases/tag/v0.1.0
