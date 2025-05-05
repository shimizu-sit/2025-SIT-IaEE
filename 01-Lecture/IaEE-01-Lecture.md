---
marp: true
theme: mytheme
class: lead
paginate: true
math: katex
title: 情報・工学探究：メディアプログラミング第1回授業資料
header: 情報・工学探究：メディアプログラミング
footer: 第1回　見て，感じて，描いてみよう | T.Shimizu © 2025
---

# 情報・工学探究
## 第1回　メディアプログラミング授業資料
**見て，感じて，描いてみよう**

授業担当：情報学部 情報学科 情報メディ専攻 清水 哲也

---

<!-- 2 -->


# 本日のスケジュール（90分）

| 時間 | 内容 |
|---|---|
| 0:00–0:10 | 授業導入・自己紹介、「メディアとは何か？」 |
| 0:10–0:25 | p5.js/OpenProcessingの概要と描画の基本 |
| 0:25–0:45 | 例題：抽象アートを作ろう |
| 0:45–0:55 | 解説：生成的アートの考え方 |
| 0:55–1:25 | 課題制作：「感情」や「音楽」をテーマに |
| 1:25–1:30 | ふりかえり・感想 |

---

<!-- 3 -->

# 「メディア」ってなんだろう？

-	メディア＝情報を伝える手段（例：新聞、映像、音楽）
-	デジタル時代のメディア：視覚・音・動き・インタラクション
-	プログラミングでメディアを自分で作る体験をしよう！

---

<!-- 4 -->

# 本日使用するツール

- 	iPad（第10世代）＋ Bluetoothキーボード
- Google Chrome ブラウザ
- OpenProcessing
- p5.js ライブラリを使用

---

<!-- 5 -->

# p5.jsとは？

-	JavaScriptベースのビジュアルプログラミングライブラリ
-	図形、色、動き、インタラクションを簡単に実装
-	教育、アート、Webで広く利用されている

---

<!-- 6 -->


# OpenProcessingとは？
-	ブラウザ上でp5.jsを動かせるエディタ
-	世界中の作品が見られる・編集できる
-	登録不要でも利用可能

---

<!-- 7 -->

# 基本の構成

```javascript
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
  ellipse(200, 200, 100, 100);
}
```

-	setup()：最初に1回実行
-	draw()：毎フレーム実行される

---

<!-- 8 -->

# よく使う図形

```javascript
rect(50, 50, 100, 100);
ellipse(200, 200, 100, 50);
line(0, 0, 300, 300);
```

-	四角形、円、線が描ける

---

<!-- 9 -->

# 色をつける

```javascript
fill(255, 0, 0); // 塗り色
stroke(0);       // 線の色
background(240); // 背景色
```

---

<!-- 10 -->


# マウスに反応する

```javascript
function draw() {
  background(255);
  ellipse(mouseX, mouseY, 50, 50);
}
```

-	`mouseX`, `mouseY`でマウスの位置を取得

---

<!-- 11 -->

# クリックで図形を追加

```
function setup() {
  createCanvas(300, 300);
  background(255);
}

function mousePressed() {
  fill(random(255), random(255), random(255));
  ellipse(mouseX, mouseY, 30, 30);
}
```

---

<!-- 12 -->


# ランダムな動き

```
function draw() {
  fill(random(255), random(255), random(255));
  ellipse(random(width), random(height), 20, 20);
}
```

---

<!-- 13 -->


# 例題：抽象アートを作ろう

- 	random()：ランダムな数を生成
-	mousePressed()：クリックで追加
-	noStroke(), fill(), background() を工夫

---

<!-- 14 -->

# サンプルコード1：動くカラフルな円

```
function draw() {
  fill(random(255), random(255), random(255), 100);
  noStroke();
  ellipse(random(width), random(height), 30, 30);
}
```

---

<!-- 15 -->

# サンプルコード2：マウスで描く

```
function setup() {
  createCanvas(400, 400);
  background(255);
}

function mouseDragged() {
  fill(random(255));
  ellipse(mouseX, mouseY, 10, 10);
}
```

---

<!-- 16 -->

# サンプルコード3：画面をタップで反応

```
function mousePressed() {
  fill(random(255), random(255), random(255));
  rect(mouseX, mouseY, 50, 50);
}
```

---

<!-- 17 -->

# 解説：生成的アートとは？

-	「コンピュータの偶然性」を活かしたアート
-	例：毎回違うパターンが生成される
-	プログラムがルールを与え、結果は多様

---

<!-- 18 -->

# 有名な生成アートの例

-	Generative Design
-	Vera Molnár
-	Tyler Hobbs (Fidenza)

---

<!-- 19 -->

# 今日の課題

## 『感情』や『音楽』をテーマに

- 自分だけのデジタルビジュアル作品を制作
-	テーマ例：好きな曲、気分、思い出
- 	色、形、動きの組合せで気持ちを表現

---

<!-- 20 -->

# 制作のヒント

-	random()で偶然性を加える
-	mousePressed()で操作を加える
-	カラーコードや円・線の組合せで自分らしさを
-	背景・透明度で“余白”を表現

---

<!-- 21 -->

# 振り返り

-	今日使った関数を思い出してみよう
-	今日のプログラムは何を表していた？
-	「感情」や「音楽」を表す工夫はできた？

---

<!-- 22 -->

# 参考リンク
- 	p5.js公式サイト
-	p5.jsリファレンス
-	OpenProcessing
-	The Coding Train

---

<!-- 23 -->

# 【付録】使用した関数まとめ

---

<!-- 24 -->

# 基本構成

```
function setup() {
  createCanvas(400, 400);
}
function draw() {
  background(255);
}
```

---

<!-- 25 -->

# 色・背景・線

```
fill(r, g, b);
stroke(r, g, b);
background(gray);
noStroke();
```

---

<!-- 26 -->

# 図形

```
rect(x, y, w, h);
ellipse(x, y, w, h);
line(x1, y1, x2, y2);
```

---

<!-- 27 -->

# マウス操作

```
mouseX, mouseY
mousePressed()
mouseDragged()
```

---

<!-- 28 -->

# ランダム

```
random(255);
random(width);
```

---

<!-- 29 -->

# アルファ（透明度）

```
fill(r, g, b, alpha);
```

---

<!-- 30 -->

# テキスト

```
text("Hello", x, y);
textSize(24);
```

---

<!-- 31 -->

# おつかれさまでした！

次回はセンサーなどを使ったインタラクティブアートに挑戦！

OpenProcessingで好きな作品を探してみよう！



<!-- 2 -->
# 授業の目的

- プログラミングを通じて表現する楽しさを体験
- 大学での情報系の学びをイメージ
- インタラクティブな技術に触れる

---

<!-- 3 -->
# 第1回の流れ（90分）

### はじめてのp5.jsで「描いて動かす」

1. 自己紹介・ガイダンス（10分）
2. p5.js / OpenProcessing紹介（10分）
3. OpenProcessingの使い方（10分）
4. 図形を描く基礎（15分）
5. 【演習】自由に描いてみよう（15分）
6. 第1回課題の説明（10分）
7. 課題制作タイム（20分）

---

<!-- 4 -->
# OpenProcessingの使い方

- [https://openprocessing.org](https://openprocessing.org)
- ログイン不要でも利用可能（保存には登録が必要）
- 「Create Sketch」で新規作成
- 左側にコード、右側に実行画面
- "Play"ボタンで動作確認

---

<!-- 5 -->
# p5.js の基本構文

```js
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
  ellipse(200, 200, 100, 100);
}
```

- `setup()`：最初に1回だけ実行
- `draw()`：繰り返し実行
- `ellipse(x, y, w, h)`：円を描く

---

<!-- 6 -->
# 第1回課題

## 『自分らしいデジタルポスターを作ろう』

- 自分の趣味や好きなものをテーマに自由に表現
- `background`, `fill`, `rect`, `ellipse`, `text` などを使って構成
- 完成した作品を発表できるようにしておこう

---

<!-- 11 -->
# 参考資料・リンク

- [p5.js公式サイト](https://p5js.org/)
- [OpenProcessing](https://openprocessing.org/)
- センサーAPI: [https://p5js.org/reference/#/p5/deviceMoved](https://p5js.org/reference/#/p5/deviceMoved)
- 作例ギャラリー: [https://openprocessing.org/browse/](https://openprocessing.org/browse/)

---

<!-- 12 -->
# ご清聴ありがとうございました

🎨 プログラミングは、表現の新しいカタチ！

大学で、さらに深く学んでみよう。

湘南工科大学 情報学部
T. Shimizu

