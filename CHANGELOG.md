# S2J Video Publisher - CHANGELOG

## unreleased

## 0.0.1 - 2026-10-05

### Changed

* `docs_mod/specs.md` の接続スコープに `youtube.readonly` を追加し、接続中のチャンネル名を接続画面に出す
* 実行契機を WP-Cron の1分間隔に固定。遅れは最終の実行時刻で判断し、有効化時と登録時には調べない
* 監査後のカテゴリー初期値を People & Blogs (`22`) にし、子ども向け宣言と改変または合成の申告は未選択にする
* Composer の参照を、S2J Slug Generater と同じく Packagist のパッケージ名だけにする
* 監査前の `videos.update` の確認は、人が動画1本で見る結果であり、自動テストの項目ではない、と補足

## 0.0.1 - 2026-10-04

### Changed

* `@s2j/docs-linter` を ^1.0.27に更新
* `docs_mod/specs.md` をプラグイン仕様ドラフトに拡充 (接続、専用テーブルの台帳、1分ごとの公開切替、監査後のブラウザ直送)

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
