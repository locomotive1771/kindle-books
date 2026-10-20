# Kindle出版リポジトリ

外出先（スマホ・新幹線など）から Claude Code のクラウドセッションで Kindle 本を作るためのリポジトリ。

## 構成
```
books/
  _template/        # 新しい本を始めるときにコピーする雛形
  <本のID>/
    plan.md         # 企画（テーマ・読者・目次・価格）
    manuscript/     # 章ごとの原稿（01_xxx.md, 02_xxx.md ...）
    cover/          # 表紙の指示書・画像
    metadata.md     # KDP登録情報（タイトル・説明文・キーワード7個・カテゴリ3つまで）
```

## 作業ルール
- 原稿は章ごとに Markdown で書く。1 回の作業が終わるたびに commit と push をする（クラウドの作業環境は消えるため）
- 文字数は char-count スキルで確認する
- AI っぽい文章の癖は stop-slop スキルで直す
- KDP へのアップロードと出版ボタンを押すのは本人が行う（Claude は KDP にログインしない）
- 個人情報・パスワード・API キーはここに置かない
