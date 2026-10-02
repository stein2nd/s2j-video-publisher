# S2J Video Publisher - CHANGELOG

## unreleased

## 0.0.1 - 2026-10-03

### Added

* プラグインの説明 (`README.md`) と仕様の起点 (`docs_mod/specs.md`)
* ドキュメント lint (`@s2j/docs-linter` ^1.0.26、`npm run lint:docs`、GitHub Actions)
* npm v12以降向けの `.npmrc` (`allow-git=all`) と `package.json` の `allowScripts`
* 管理画面向けの React と Vite (`react` ^19.3.0、`vite` ^8.3.2)
* 間接依存の Rollup を ^4.64.0に固定 (`package.json` の `overrides`)
* Cursor のコマンド許可設定 (`.cursor/allowlist.json`)
* Node とビルド成果物向けの `.gitignore`

### Changed

* `.vscode/settings.json` で `json.schemaDownload.enable` を有効化

