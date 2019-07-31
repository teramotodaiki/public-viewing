# ニコニコ風にコメントを流すやつ

## 使い方

YouTube で見る（わかりやすい）

https://www.youtube.com/embed/H1ixkUwvuI8

### チャットする人

https://public-viewing.firebaseapp.com/ にアクセスする

### パブリックビューイングに設置する人

https://public-viewing.firebaseapp.com/view.html にアクセスする

- このままでも https://public-viewing.firebaseapp.com/ からのチャットは流れます
- YouTube Live のコメントを流したい場合は Google でログインします

### Google でログイン

- **YouTube Live を放送しているチャンネルの管理者になっている Google アカウント** を用意します
- 右下の SIGN IN をクリックしてログインします
  - この時警告が表示されますが、こんな感じで許可してください
  - [![Image from Gyazo](https://i.gyazo.com/26d2bc7dd63d00138810861edf6cc232.gif)](https://gyazo.com/26d2bc7dd63d00138810861edf6cc232)
- どのライブ動画を使うのか、順番に確認されます。OK を押してください
- 上手くいけば流れます

## TODO

- 文字が重なった時に下に行くようにする
- YouTube Data API の制限で、チャット取得 API の polling の制限がキツすぎる問題をどうにかする
  - 試しにうごかしたら 3000ms くらいインターバルをあけろと言われた（チャットの勢いによってはもっと大きくなるらしい）
  - ディレイがあるのはしょうがないとしても、一気にドバッと流れるのは良くないので、ズレを再現したい
