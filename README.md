# HTML CSS Parts List

## Tips
---
### Jsは閉じbodyタグ直前
- JSが読み込み完了するまで真っ白になるのを防ぐため
- 上からGAとかは上記に書いたり、CSSはあっておきたいので上部に記載する
- そのためsanitize.cssやreset.cssなどはsyle.cssよりも先に読み込ませるために上部に記載する

### WEB font は Google font でOK
- よく使われるフォントnoto sans
- フォントはRegular400 Bold700をよく使う

### ネット関係によって読み込み対策に
- 各MacやWindowsごとにデフォルトで用意されているフォントを代替案として設定しておく

### spanタグは飾り付けを行いたい時とかに囲う

### sectionタグにh1に入れると事実上h2になるらしい

## セクショニング・コンテンツを利用する
- 潜在的に見出しとアウトラインを持っている
- クローラやユニバーサルデザインの観点から望ましい

### 適当なリンクを入れる時は #をよく入れる

### メイン・コンテンツ以外のサブ的ない要素には asideタグを利用する

### hr や br の閉じタグ/はつけてもつけなくても良い

### 画像の種類
- jpeg
  - 細かい画像が得意

- png(png-8, png-24, png-36)
  - 細かい表現は不得意。軽い。透過が得意（透過使うと重くなる）

- gif
  - 透過可能ｍ画質が荒い、アニメーション（CSS・JSなどで対応するためあんま使わない）

- svg
  - タグの１つのため文字情報そのため早いさらにJSで操作することが可能。ベクターファイルをHTMLに変換したもの
  - 細かい表現は不得意


### box-sizing: border-boxの意味
- padding と %と計算をすべて内包してくれるので計算が楽になる

### smallタグはコピーライト専用でOK

### iframe 外部のHTMLを呼び出せる
- あくまで呼び出しのみで呼び出し先のHTMLは操作できない

### ◯を作る時
- `border-radius: 50%` と `overflow: hidden`にする

### Clickable な要素に対しては基本cusor pointerをつけた方がユーザフレンドリー

### 位置調整
- 親要素に `postion: relative` つけて子要素に `postion: absolute` をつけると親要素の範囲内で自由に位置を変更できる

### デフォルトのスタイルのサニタイズ
- リンクタグはデフォルト青になるため黒にする

### 黒も#333, #111が目に優しくて良いとされている

### CSSのクラスを記述する際はHTMLからコピーするのが便利

### 静的ファイルはassetsとかによく格納する

### 同じクラスを拡張する形で書いていくときれいになりやすい

### h1タグの複数はあり？？

### 画面で最初に見える位置をHeroなど呼ぶ

### 中央寄せ
- ブロック要素に対して `margin: 0 auto` にすると中央寄せに

### データリストタグの順序
- データタグは`<dt>`>`<dd>`の順序で書かないと行けない

### 利用する動画は10MB超えてくるときつい

### strongタグは利用する場合２個位までが目安

### videoタグ
- videoでくくってsourceを複数記述することで読み込めなかった時の代替案を設定できる
- `autoplay loop muted preload` は記述するのがおすすめ

### 位置中央寄せ
- absoluteの時の`top:50%` `left: 50%` `transform: translate(-50%, -50%)`

### 動画や画像幅の画面幅に移す時はwidth100% height100%は間が空いてしまう
- 元の画角で長い方に105%などを指定して、短い方をautoにする

### JSだとローカルサーバを用意しないと動かない場合がある
- node.jsやホスティングすると動く

### navタグ
- 基本headerタグのナビゲーションとしか使わない

### レスポンシブデザイン
- 768px タブレット・スマホの基準値
- SP・タブレットは`width: 100%`にする対応が多い？？

### テーブルタグ
- 自動的にdisplayがtable要素になる
- また勝手に`<tbody>`などグルーピングのタグ入ってしまったりする（ブラウザの仕様）

## Reference
- Google Font
https://fonts.google.com/

- Dummy Image
https://dummyimage.com/

- Free Icon
https://www.flaticon.com/

- Free Logo
https://worldvectorlogo.com/ja/downlo...

- Free Video
https://www.pexels.com/videos/

- particles.js
https://github.com/VincentGarreau/par...

- Favicon Generator
https://realfavicongenerator.net/

- Hosting Service
https://www.netlify.com/
