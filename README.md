# 柏の葉ものしりクイズ - Webアプリ

## ファイル構成

```
index.html                    ← メインのWebアプリ（これ1つで動作します）
images/
  quiz_photos/                ← 出題用写真（26枚）
    q1.jpg ～ q26.jpg
  characters_excel/           ← Excel内キャラクタ画像（26枚）
    c1.png ～ c26.png
  characters_green/           ← かっしー（緑）キャラクタ画像（27枚）
    green_1.png ～ green_27.png
  characters_pink/            ← リーフィ（ピンク）キャラクタ画像（42枚）
    pink_1.png ～ pink_42.png
  reference_screens/          ← デザイン参考画面（3枚）
    top_screen.jpg
    quiz_screen.jpg
    ranking_screen.jpg
```

## デプロイ方法

`index.html` を1つアップロードするだけで動作します。
全画像はbase64でHTML内に埋め込み済みです。

### GitHub Pages
1. リポジトリを作成
2. `index.html` をアップロード
3. Settings → Pages → Branch: main → Save
4. `https://ユーザー名.github.io/リポジトリ名/` でアクセス

### Netlify Drop
1. https://app.netlify.com/drop にアクセス
2. `index.html` をドラッグ＆ドロップ

## 仕様
- 全26問からランダム10問出題
- 選択肢もランダム順
- 10秒カウントダウン（早押し得点）
- 1問最大10,000点、10問合計最大100,000点
- ランキングTop10 + 参加人数表示
- BGM・効果音付き（Web Audio API）
- レスポンシブ対応（スマートフォン最適化）
