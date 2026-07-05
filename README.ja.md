# Marc MCP Assistant

言語: [中文](README.zh-CN.md) | [English](README.md) | **日本語**

Marc MCP Assistant は、MSC Marc/Mentat ユーザー向けの Windows 優先・クローズドソースのワークフロー支援ツールです。MCP を通じて Codex などの AI エージェントを制御されたローカル Marc ワークフローへ接続し、モデル確認、解析失敗の手掛かり整理、選択的な後処理、作業記録をより追跡しやすくすることを目的としています。

これは MSC/Hexagon の公式製品ではありません。Marc/Mentat 本体、Marc/Mentat ライセンス、工学的判断の代替は提供しません。

## 現在のバージョン状況

```text
Current private trial line: MarcMCP trial 2.5.0-trial
Platform: Windows
Stage: private beta
Delivery: contact author first, then private package + trial license
Use with: local MSC Marc/Mentat + Codex MCP
Public GitHub Release: not open yet
```

現在のバージョンは、案内付きのプライベート試用に使える段階です。新機能は継続的に開発中であり、実際の Marc/Mentat ユーザーからの問題、要望、フィードバックを歓迎します。

## 現在のバージョンで対応していること

現在のクローズドパッケージは、実務的な Marc ワークフロー支援を重視しています。

- Codex 用の制御されたローカル MCP server を起動する；
- package 状態と license 状態を確認する；
- 試用 license 申請に必要な machine code を表示する；
- Codex が古いパッケージや誤ったパスではなく、受け取ったパッケージを使っているか確認する；
- ローカル MSC Marc/Mentat 環境を検出できるか確認する；
- 支援ワークフロー用のローカル Marc project workspace を初期化する；
- 基本的な MCP doctor と環境チェックを実行する；
- set、link、boundary、load、material などのモデル確認の手掛かりを整理する；
- log、input file、exit number から solver failure の手掛かりを集める；
- 一部の `.t16` 結果抽出と要約ワークフローを支援する；
- 論文、研究、エンジニアリングプロジェクトのために、確認・変更・結果抽出の証跡を残しやすくする；
- サポートや診断が必要な場合のフィードバック経路を整理する。

## 減らしたい問題

Marc ユーザーが時間を失いやすいのは、理論だけでなく、繰り返しが多く、間違いやすく、追跡しにくい作業です。このプロジェクトは次の問題を減らすことを目指しています。

- Mentat モデル詳細の繰り返し手動確認；
- Codex がどの exe、どの package、どの workflow を使っているのか分かりにくいこと；
- 解析失敗後の log、input file、screenshot、error clue が散在すること；
- 後処理記録が手作業に依存し、後から再確認しにくいこと；
- 何を確認し、何を変更し、何を抽出したかを説明しにくいこと；
- Marc の問題を AI assistant や support 相手に整理して説明しにくいこと。

目的は Marc を完全自動化することではありません。ローカル Marc ワークフローをより制御しやすく、追跡しやすく、再確認しやすくし、AI と議論しやすい形にすることです。

## 継続開発中

今後の開発項目には、次のようなものがあります。

- より広い Marc/Mentat ワークフロー対応；
- solver failure 診断テンプレートの改善；
- よく使われる `.t16` 後処理支援の追加；
- 中国語、英語、日本語ドキュメントの改善；
- 試用、フィードバック、サポート、更新フローの改善；
- 実際のユーザー問題に基づく private package の継続更新。

特定分野の Marc/Mentat ワークフローがある場合、フィードバックを歓迎します。実際のユーザー問題は、次に改善すべき機能を決めるうえで最も重要な情報です。

## 対象ユーザー

次のような Marc/Mentat ユーザーに向いています。

- 研究、論文、またはエンジニアリングプロジェクトで MSC Marc/Mentat を使っている；
- model set、link、boundary、load、material setup を何度も確認している；
- solver failure、exit number、収束問題を調査している；
- Codex による Marc ワークフロー支援を試したい；
- 後処理や診断証跡をより整理したい。

## プライベート試用

試用は手動審査です。現在のバージョンに合う場合、次を受け取れる可能性があります。

- Windows クローズドソース試用パッケージ；
- machine-bound trial license file；
- 短いインストール説明と Codex 設定案内；
- 試用フィードバック用テンプレート。

試用は、有効期間、マシン、機能範囲、パッケージバージョン、サポート範囲によって制限される場合があります。目的は、実際の Marc ワークフローに役立つかを確認することであり、無制限の公開版を提供することではありません。

## 試用申請

連絡先:

- Email: `1309224565@qq.com`
- WeChat: `18169419809`

WeChat 追加時は、次を記入してください。

```text
Marc MCP Trial
```

最初の連絡では、次を送ってください。

```text
Marc/Mentat version:
Windows version:
Research or engineering field:
Current problem:
Solver exit number, if any:
Whether screenshots or log excerpts are available:
Need: trial / one-time diagnosis / monthly use / project support
```

最初から完全なモデルファイルを送らないでください。スクリーンショット、短いログ抜粋、匿名化した問題説明で十分です。

## パッケージ受領後

プライベートパッケージと license を受け取った後、次の案内に沿って Codex に設定を依頼できます。

- [Codex setup prompt](docs/codex-setup-prompt.md)
- [Trial installation](docs/trial-install.md)

典型的な流れ:

```text
Receive package -> unzip locally -> run status check -> send machine code
-> receive license.json -> place license.json next to the executable under licenses
-> configure Codex MCP -> verify check_mcp_process_env -> start trial
```

## 重要な注意

このプロジェクトは次を保証しません。

- モデルの正しさの自動保証；
- 収束の保証；
- Marc/Mentat 公式ソフトウェアの代替；
- Marc/Mentat ライセンスの提供；
- 無制限の無料利用；
- コアソースコードの公開。

モデルの安全性、工学的仮定、最終判断はユーザーの責任です。

## ドキュメント

- [Apply for trial](docs/apply.md)
- [Codex setup prompt](docs/codex-setup-prompt.md)
- [Trial installation](docs/trial-install.md)
- [Closed package notes](docs/trial-package.md)
- [FAQ](docs/faq.md)
- [Privacy](docs/privacy.md)
- [Contact](docs/contact.md)
- [Demo plan](docs/demo-plan.md)
