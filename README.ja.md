# Jcble_mam

[简体中文](README.zh-CN.md) | [English](README.en.md) | [Español](README.es.md) | [한국어](README.ko.md)

`jcble-mam` は、企業のコンテンツ運用、コピーライティング、オンラインマーケティング、multi-Agent 協業チームを構築・運用するための汎用 Codex skill です。

対応する Markdown 言語：

- 簡体字中国語 `zh-CN`
- 英語 `en`
- スペイン語 `es`
- 日本語 `ja`
- 韓国語 `ko`

## 利用シーン

- 企業文書の管理
- ソリューション企画と提案書作成
- ソーシャルメディアのテーマ企画
- 企業紹介 PPT とソリューション PPT の設計
- 製品コピーライティング
- 製品、ソリューション、販促画像のビジュアルブリーフ
- グローバル市場情報の収集
- 業界ニュースの追跡
- 海外顧客の探索
- アウトリーチメールの下書き作成
- 週次・月次のコンテンツ、プラットフォーム、リードの振り返り
- 永続的な multi-Agent Codex セッションのセットアップ
- 多言語 Markdown の作成、翻訳、ローカライズ

## Skill 名

インストール用の skill 名は次の通りです：

```text
jcble-mam
```

`Jcble_mam` は表示名およびユーザー向けエイリアスとして維持します。このワークフローは汎用で、どの企業にも適用できます。

## インストール

このリポジトリを Codex skills ディレクトリにクローンします：

```bash
git clone https://github.com/Mecil9/jcble-mam.git ~/.agents/skills/jcble-mam
```

その後、新しい Codex セッションを開始して skill レジストリを更新します。

## 設定

使用前に、以下のプレースホルダーを自社のワークスペースに合わせて変更します：

```text
COMPANY_WORKSPACE=/path/to/company/workspace
COMPANY_KNOWLEDGE_BASE=/path/to/company/knowledge-base
COMPANY_MARKETING_WORKSPACE=/path/to/company/content-marketing-workspace
```

会社で異なるフォルダ名を使っている場合は、reference ファイルを更新するか、同等のインデックスファイルを作成してください。

## 主なファイル

- `SKILL.md` - トリガー条件と基本ワークフロー
- `references/agent-team-roles.md` - multi-Agent 役割ライブラリ
- `references/session-orchestration.md` - Codex セッションの作成、命名、同期、メッセージルーティング
- `references/company-material-boundaries.md` - 会社資料の境界と機密データのルール
- `references/multilingual-workflow.md` - 多言語 Markdown のルール、ローカライズ境界、レビューリスト
- `assets/task-card-template.md` - タスクカードテンプレート
- `assets/message-template.md` - メッセージバステンプレート
- `assets/retrospective-template.md` - 週次・月次振り返りテンプレート

## 安全上の注意

外部公開前に：

- 顧客、契約、財務、給与、認証情報、個人情報などの機密情報を削除する
- 公開する主張は承認済みのソースファイルで確認する
- アウトリーチメールは人間の承認まで下書きとして扱う
- 生成画像を実在の製品、現場、顧客シーンとして扱わない

## License

MIT
