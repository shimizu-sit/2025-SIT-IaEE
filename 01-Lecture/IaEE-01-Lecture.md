---
marp: true
theme: mytheme
class: lead
paginate: true
math: katex
title: インタラクティブ表現で学ぶプログラミング
header: 第1回 情報・工学探究
footer: インタラクティブ表現で学ぶプログラミング | T.Shimizu © 2025
---

# 情報・工学探究
## 第1回講義資料
**インタラクティブ表現で学ぶプログラミング入門**

講義担当：情報学部 情報学科 情報メディ専攻 清水 哲也

---

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

