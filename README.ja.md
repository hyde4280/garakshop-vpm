# Garak's Shop VPM

[English](README.md)

VRChat Creator Companion (VCC) 向けの VPM (VRChat Package Manager) リスティングです。Garak's Shop のパッケージはここに掲載されます。リスティング自体は GitHub Actions が [`source.json`](source.json) からビルドし、GitHub Pages で公開します。

## VCC への追加

- リスティング URL: `https://hyde4280.github.io/garakshop-vpm/index.json`
- ワンクリック: VCC がインストールされた PC のブラウザで[リスティングページ](https://hyde4280.github.io/garakshop-vpm/)を開き、**Add to VCC** を押してください。(GitHub は README 内の `vcc://` リンクをクリック可能にしないため、ボタンはそのページに置いています。)
- または VCC で: Settings > Packages > Add Repository を開き、リスティング URL を貼り付けます。

## パッケージ

掲載中: `jp.garakshop.shower` ([リポジトリ](https://github.com/hyde4280/jp.garakshop.shower))。予定: `jp.garakshop.cellloader`、`jp.garakshop.elevator`。各パッケージは独自の公開リポジトリを持ち (開発リポジトリから `git subtree split` で切り出してリリースします)、`source.json` の `githubRepos` に追加されます。

## リスティングの更新

パッケージが新しいリリースを公開しても、リスティングは**自動では再ビルドされません**。リリース後は "Build Repo Listing" ワークフローを手動で実行 (Actions > Build Repo Listing > Run workflow) するか、`source.json` への変更を `main` へ push してください。

パッケージを追加するには、その GitHub リポジトリ (`owner/name`、パッケージ zip を含む Release が必要) を `source.json` の `githubRepos` に入れて `main` へ push します。

## ライセンス

リスティングのファイルは MIT License で提供します。各パッケージには独自のライセンスがあります (各リポジトリに別段の記載がなければ MIT)。
