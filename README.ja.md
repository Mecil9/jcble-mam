# Jcble_mam

[English](README.md) | [简体中文](README.zh-CN.md) | [Español](README.es.md) | 日本語 | [한국어](README.ko.md)

`jcble-mam` は、企業のコンテンツ運用、コピーライティング、オンラインマーケティング、multi-Agent セッション連携を Codex で扱うための skill です。

Codex を、文書管理、提案書作成、製品コピー、SNS テーマ企画、ビジュアルブリーフ、市場調査、顧客探索、アウトリーチメール下書き、週次・月次の振り返りを行うコンテンツ・マーケティングチームとして機能させます。

## 主な機能

- 企業向けのコンテンツ・マーケティング Agent チームを作成します。
- 編集統括、文書管理、提案企画、コピーライティング、製品コピー、PPT 企画、ビジュアルブリーフ、市場調査、顧客探索、メール下書き、レビュー、振り返りの役割を定義します。
- 役割ごとの永続的な Codex セッションとメッセージバス運用をサポートします。
- 簡体字中国語、英語、スペイン語、日本語、韓国語の Markdown 出力をサポートします。
- 外部向けコンテンツを承認済みの根拠と人間のレビューに結び付けます。

## Codex へのインストール

このリポジトリを Codex skills ディレクトリにクローンします：

```bash
git clone https://github.com/Mecil9/jcble-mam.git ~/.agents/skills/jcble-mam
```

その後、新しい Codex セッションを開始して skill レジストリを更新します。

Codex の skills ディレクトリが異なる場合は、その場所にクローンし、フォルダ名を次のままにしてください：

```text
jcble-mam
```

## 基本的な使い方

インストール後、Codex に自然言語で依頼します。例：

```text
jcble-mam を使って、自社向けのコンテンツ・マーケティング Agent チームを作成してください。
```

```text
jcble-mam を使って、この製品資料を Web サイト用コピーとアウトリーチメールの下書きにしてください。
```

```text
jcble-mam を使って、編集者、コピーライター、市場調査、ビジュアルブリーフ、レビュー Agent の独立した Codex セッションを作成してください。
```

```text
jcble-mam を使って、この提案概要を英語、スペイン語、日本語、韓国語で作成してください。
```

## ワークスペース設定

会社ファイルと一緒に使う前に、次のプレースホルダーを自社ワークスペースに合わせます：

```text
COMPANY_WORKSPACE=/path/to/company/workspace
COMPANY_KNOWLEDGE_BASE=/path/to/company/knowledge-base
COMPANY_MARKETING_WORKSPACE=/path/to/company/content-marketing-workspace
```

会社で異なるフォルダ名を使っている場合は、reference ファイルを更新するか、同等のインデックスファイルを作成してください。

## 含まれるファイル

- `SKILL.md` - トリガー条件と基本ワークフロー
- `references/agent-team-roles.md` - multi-Agent 役割ライブラリ
- `references/session-orchestration.md` - Codex セッションの作成、命名、同期、メッセージルーティング
- `references/company-material-boundaries.md` - 会社資料の境界と機密データのルール
- `references/multilingual-workflow.md` - 多言語 Markdown のルール、ローカライズ境界、レビューリスト
- `assets/task-card-template.md` - タスクカードテンプレート
- `assets/message-template.md` - メッセージバステンプレート
- `assets/retrospective-template.md` - 週次・月次振り返りテンプレート

## 安全上の注意

外部に公開または送信する前に：

- 顧客、契約、財務、給与、認証情報、個人情報などの機密情報を削除する
- 公開する主張は承認済みのソースファイルで確認する
- アウトリーチメールは人間の承認まで下書きとして扱う
- 生成画像を実在の製品、現場、顧客シーンとして扱わない

## License

MIT
