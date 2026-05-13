# TODO (myscraps)

## Milestone: v0.0.2 - サイトを自分のものにする＋開発環境を整える

### セキュリティ・バグ修正

無し。

### コード・機能

サイトの個人化：

- [ ] 1. index.astro のヒーローテキストを書き換える
  - src/pages/index.astro の "AstroPaper is a minimal..." のくだりを自分の言葉に
- [ ] 2. about.md を自己紹介に書き換える
  - src/pages/about.md を自分のプロフィールに
- [ ] 3. SOCIALS / SHARE_LINKS を整理する
  - 不要な SNS 共有ボタンを削除、自分のアカウント URL に差し替え

開発環境の整備：

- [ ] 1. Node.js バージョンを固定する
  - .mise.toml を作成して `node = "x.x.x"` を記載
- [ ] 2. リンター・フォーマッターを整備する
  - package.json には ESLint + Prettier がすでに存在する
  - Biome への移行も選択肢として検討（ADR を書く）
- [ ] Neovim + LazyVim の開発環境整備
  - Ref [Editor setup | Docs](https://docs.astro.build/en/editor-setup/)
- [ ] AI tools 周りの整備
  - Ref [Building Astro sites with AI tools | Docs](https://docs.astro.build/en/guides/build-with-ai/)

### テスト・CI

無し。

### ドキュメント

無し。

### プロジェクト管理

無し。

## Milestone: v0.0.3 - TBD

### セキュリティ・バグ修正

無し。

### コード・機能

無し。

### テスト・CI

無し。

### ドキュメント

無し。

### プロジェクト管理

無し。

## Backlog（いつかやる）

### セキュリティ・バグ修正

無し。

### コード・機能

無し。

### テスト・CI

無し。

### ドキュメント

無し。

### プロジェクト管理

- [ ] プロジェクト名の命名を再検討
  - より良いネーミングがあったら変えたい
  - 今の命名（`myscraps`）も、悪くは無いが良くもない
- [ ] **LLM Wiki** や RAG みたいなものを構築することを検討する

### 将来検討

- [ ] docs: README.md の「For Users」セクションを書くべきか検討する
  - このブログの読者は基本的に自分自身のため、不要かもしれない
  - 書くとすれば「ブログの URL・検索の使い方」程度の薄い内容になる
- [ ] GitHub の Pull Request 機能を使うかどうか決める
  - Wiki・Issues は使わない方針だが、PR については未決定
  - 決定後、README.md の Policy セクションを更新する
- [ ] コンテンツ部分の分離を検討する
  - "myscraps" には 2 つの側面がある
    - 1. TIL 的な技術メモを記したマークダウンファイル
    - 1. それ公開している静的サイト
  - ここ（このリポジトリ）では「静的サイト」の部分だけを管理するようにしたい
  - 混ざってるのが良くない
  - 「コンテンツを書く」をこのリポジトリの責務とせず、このリポジトリでは
    フロントエンドスキルの習得を目的とした静的サイトの公開に焦点を当てたい
  - 別のところから TIL メモを読み込んで、それを加工してコンテンツとし、公開するみたいなのはどうか
