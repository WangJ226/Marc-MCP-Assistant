# Marc MCP Assistant

言語: [中文](README.zh-CN.md) | [English](README.md) | **日本語**

Marc MCP Assistant は、MSC Marc/Mentat ユーザー向けの Windows 優先・クローズドソースのワークフロー支援ツールです。Codex などの AI アシスタントを、制御されたローカル環境で Marc ワークフローに接続することを目的としています。

これは MSC/Hexagon の公式製品ではありません。Marc/Mentat 本体や Marc/Mentat ライセンスは含まれず、工学的判断を置き換えるものでもありません。

## 現在のクローズドパッケージ

現在のプライベート試用ライン：

```text
MarcMCP trial 2.5.0-trial
Platform: Windows
Delivery: private request only
Use with: local MSC Marc/Mentat + Codex MCP
```

GitHub Releases はまだ公開していません。現在は、問い合わせ後に用途を確認し、適切な場合に Windows 試用パッケージとマシンに紐づく trial license を個別提供します。

## 現在支援できること

Marc ユーザーが時間を失いやすいのは、理論だけでなく、繰り返しが多く、間違いやすく、追跡しにくい作業です。現在のクローズドパッケージは、主に次の作業を支援します。

- Codex を制御された MCP server 経由でローカル Marc/Mentat ワークフローに接続する；
- ローカル Marc/Mentat 環境が助手から見えているか確認する；
- Codex が古いパッケージや誤ったパスではなく、受け取ったクローズドパッケージを使っているか確認する；
- set、link、boundary、load、material などのモデル検査の手がかりを整理する；
- ログ、入力ファイル、exit number から solver failure の手がかりを集める；
- 一部の `.t16` 結果抽出と要約ワークフローを支援する；
- 論文、研究、エンジニアリング作業の検査・結果証拠をより明確に残す；
- サポートや診断が必要なとき、より構造化されたフィードバック経路を提供する。

目的は、ローカルの Marc ワークフローをより追跡しやすく、再確認しやすく、AI と相談しやすい形にすることです。

## 典型的な悩み

次のような悩みがある場合、試用する価値があります。

- Codex に Marc を手伝わせたいが、接続を制御したい；
- Mentat 内で同じモデルチェックを何度も行っている；
- solver failure の手がかりがログや入力ファイルに散らばっている；
- 何を確認し、何を変更し、何を抽出したかを記録したい；
- `.t16` 後処理や診断整理を手作業だけに頼りたくない。

## 対象ユーザー

次のような Marc/Mentat ユーザーに向いています。

- 研究、論文、またはエンジニアリングプロジェクトで MSC Marc/Mentat を使っている；
- model set、link、boundary、load、material setup を何度も確認している；
- solver failure、exit number、収束問題を調査している；
- Codex による Marc ワークフロー支援を試したい；
- 後処理や診断証拠をより整理したい。

## プライベート試用

試用は手動審査です。現在のバージョンに合う場合、以下を受け取れる可能性があります。

- Windows クローズドソース試用パッケージ；
- マシンに紐づく試用 license ファイル；
- 短いインストール説明と Codex 設定案内；
- 試用フィードバック用テンプレート。

試用は、有効期間、マシン、機能範囲、パッケージバージョン、サポート範囲によって制限される場合があります。目的は、実際の Marc ワークフローに役立つかを確認することであり、無制限の公開版を提供することではありません。

## 試用申請

連絡先：

- Email: `1309224565@qq.com`
- WeChat: `18169419809`

WeChat 追加時は、以下を記入してください。

```text
Marc MCP Trial
```

最初の連絡では、以下を送ってください。

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

プライベートパッケージと license を受け取った後、Codex に次の案内に沿って設定を依頼できます。

- [Codex setup prompt](docs/codex-setup-prompt.md)
- [Trial installation](docs/trial-install.md)

典型的な流れ：

```text
Receive package -> unzip locally -> run status check -> send machine code
-> receive license.json -> place license.json next to the executable under licenses
-> configure Codex MCP -> verify check_mcp_process_env -> start trial
```

## 重要な注意

このプロジェクトは以下を保証しません。

- モデルの正しさを自動保証すること；
- 収束を保証すること；
- Marc/Mentat 公式ソフトウェアを置き換えること；
- Marc/Mentat ライセンスを提供すること；
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
