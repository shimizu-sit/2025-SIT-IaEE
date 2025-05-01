---
marp: true
theme: mytheme
class: lead
paginate: true
math: katex
title: インタラクティブ表現で学ぶプログラミング
header: 第2回 情報・工学探究
footer: インタラクティブ表現で学ぶプログラミング | T.Shimizu © 2025
---

# 情報・工学探究
## 第2回講義資料
**インタラクティブ表現で学ぶプログラミング入門**

講義担当：情報学部 情報学科 情報メディ専攻 清水 哲也

---

<!-- 7 -->
# 第2回の流れ（90分）

### インタラクティブ作品に挑戦！

1. 前回のふりかえり・ゴール説明（10分）
2. インタラクティブコード紹介（15分）
3. 【演習】傾きやタッチを使った表現（20分）
4. 第2回課題の説明（5分）
5. 課題制作タイム（35分）
6. 発表・ふりかえり（5分）

---

<!-- 8 -->
# センサーの活用例（iPad対応）

```js
function draw() {
  background(255);
  fill(100, 100, 255);
  ellipse(width/2, height/2, rotationX*10, rotationY*10);
}
```

- `rotationX`, `rotationY`：iPadの傾きで変化
- `touchStarted()`：画面タッチを検知

---

<!-- 9 -->
# 第2回課題

## 『インタラクティブアートを作ろう』

- タッチ操作や傾きを使って、変化する作品を作る
- 例：傾けると色が変わる、タッチで音が鳴る、など
- 前回の図形・色の知識を活かす

---

<!-- 10 -->
# ふりかえりとまとめ

- 「表現×プログラミング」の可能性に触れた
- 大学での学びへのヒントになった？
- できたこと・面白かったことを振り返ろう

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

