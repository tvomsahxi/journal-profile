# journal-profile

GitHub Pages（Jekyll）で書く日記ブログです。

公開URL: https://tvomsahxi.github.io/journal-profile/

## 日記の書き方

1. `_posts/` フォルダに `YYYY-MM-DD-タイトル.md` という名前でファイルを作る
   （例: `_posts/2026-10-01-autumn.md`。タイトル部分は半角英数字とハイフンがおすすめ）
2. ファイルの先頭に次の情報（front matter）を書く

   ```markdown
   ---
   layout: post
   title: "記事のタイトル"
   date: 2026-10-01 21:00:00 +0900
   categories: diary
   ---

   ここから本文（Markdown で書けます）
   ```

3. コミットして `main` ブランチに push すると、1〜2分でサイトに反映されます。

GitHub の Web 画面上で「Add file → Create new file」から直接書くこともできます。
ひな形は `_drafts/template.md` にあります。

## 公開の設定（最初に1回だけ）

リポジトリの **Settings → Pages** で、

- Source: `Deploy from a branch`
- Branch: `main` / `/ (root)`

を選んで Save します。

## 手元でプレビューする（任意）

```sh
bundle install
bundle exec jekyll serve
```

http://localhost:4000/journal-profile/ で確認できます。

## 設定の変更

ブログ名や説明文は `_config.yml` の `title` / `description` を書き換えてください。
