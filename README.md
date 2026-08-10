# hotel-post-assets

TikTok の Content Posting API は、投稿する画像を **こちら側の公開URLから取りに来る**
（`PULL_FROM_URL`）方式しか受け付けない。そのための置き場。

- `images/YYYY-MM-DD/...` — 投稿する画像。投稿が終わったら古い日付から消える。
- `callback.html` — TikTok と連携するときに、認可コードを受け取って表示するだけのページ。

画像の著作権は各施設にある。ここに置くのは TikTok に渡すための一時的な受け渡しで、
`run.py publish` が投稿後に古い分を削除する。
