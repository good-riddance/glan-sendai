# GLAN.SENDAI 物件専用サイト

仙台市青葉区小田原のアパート「GLAN.SENDAI 〜Urban Wood Residence〜」の専用ランディングページ。

## ファイル構成

```
glan-sendai/
├── index.html       メインHTML(これだけで完結)
├── README.md        このファイル
├── SETUP-GUIDE.md   GitHub Pages公開ガイド
└── images/          画像置き場(差し替え用)
    ├── HR-01.jpg            ヒーロー1枚目: 外観
    ├── HR-02.jpg            ヒーロー2枚目
    ├── HR-03.jpg            ヒーロー3枚目
    ├── HR-04.jpg            ヒーロー4枚目
    ├── HR-05.jpg            ヒーロー5枚目
    ├── GL-01.jpg            ギャラリー1枚目
    ├── GL-02.jpg            ギャラリー2枚目
    ├── GL-03.jpg            ギャラリー3枚目
    ├── GL-04.jpg            ギャラリー4枚目
    ├── GL-05.jpg            ギャラリー5枚目
    ├── GL-06.jpg            ギャラリー6枚目
    ├── GL-07.jpg            ギャラリー7枚目
    ├── GL-08.jpg            ギャラリー8枚目
    ├── GL-09.jpg            ギャラリー9枚目
    ├── GL-10.jpg            ギャラリー10枚目
    ├── GL-11.jpg            ギャラリー11枚目
    ├── GL-12.jpg            ギャラリー12枚目
    ├── GL-13.jpg            ギャラリー13枚目
    ├── GL-14.jpg            ギャラリー14枚目
    ├── GL-15.jpg            ギャラリー15枚目
    ├── GL-16.jpg            ギャラリー16枚目
    ├── Room-101.jpg         101号室間取り図
    ├── Room-102.jpg         102号室間取り図
    └── Room-103.jpg         103号室間取り図
```

**命名規則のルール**
- **HR-XX** (Hero): ヒーローのカルーセル画像 5枚
- **GL-XX** (Gallery): ギャラリーセクションのタイル画像 16枚
- **Room-XXX**: 各部屋の間取り図(部屋番号と対応)

合計24ファイルです。

画像が無くても表示は崩れません(プレースホルダーで表示される)。`images/`フォルダに上記ファイル名でJPGを置けば自動的に差し替わります。

## 推奨画像サイズ

- exterior.jpg(ヒーロー): 横1600px以上、横長。容量200KB以下を目標
- room-* / kitchen / bathroom / washroom / entrance: 横800px、正方形でクロップされる前提
- floor-*(間取り図): 横500px、白背景

## ローカルでの確認方法

`index.html` をダブルクリックすればブラウザで開きます。Googleマップだけはネット接続が必要です。

## GitHub Pagesで公開する手順

### 1. GitHubアカウント作成(まだなら)

https://github.com/signup

### 2. リポジトリを作る

- リポジトリ名: 例えば `glan-sendai`
- Public(無料公開のため)
- "Add a README file"のチェックは入れない

### 3. ファイルをアップロード

リポジトリページで "uploading an existing file" → `index.html` と `images/` フォルダ内のファイルをドラッグ&ドロップ → "Commit changes"

### 4. GitHub Pagesを有効化

- リポジトリの Settings → Pages
- Source: `Deploy from a branch`
- Branch: `main` / `/(root)` を選択 → Save
- 1〜2分待つと https://(ユーザー名).github.io/glan-sendai/ で公開される

### 5. 独自ドメインを使う場合(任意)

ドメインを取得済みなら(お名前.com、Cloudflare Registrarなど)、Settings → Pages → Custom domain にドメイン名を入力。DNS側でCNAMEレコードを `(ユーザー名).github.io` に向ける。

## 写真を後から差し替える

1. リポジトリの `images/` フォルダを開く
2. 該当ファイルをクリック → 鉛筆アイコン(削除)→ 同名で再アップロード
3. または GitHub Desktop / git CLI から `git push`
4. 数十秒で本番サイトに反映

## SEO対策メモ

- titleタグ・meta description・OGP設定済み
- Schema.org構造化データ(ApartmentComplex)埋め込み済み → Googleの検索結果でリッチに表示される可能性
- "GLAN仙台" "グラン仙台" "仙台駅 新築 1LDK 仙台市青葉区小田原" あたりで上位を狙う

## Googleマップ検索ヒット対策

賃貸物件単体ではGoogleビジネスプロフィール登録が通らないのが通例。代替案:

1. 株式会社グッドリダンスを事業所として登録(既にあれば)、説明文に物件名を入れる
2. このサイトのSEOを上げる(titleタグの調整、外部からの被リンク)
3. SUUMO、ホームズ、CHINTAIなど大手にも掲載されているなら、それぞれにこのサイトのURLを貼ってもらえると被リンクになる

## 物件情報(参照用)

- 物件名: GLAN.SENDAI(グラン仙台)
- 所在地: 宮城県仙台市青葉区小田原4丁目
- 築年: 2026年2月
- 構造: 木造3階建
- 緯度経度: 38.267126, 140.889009
- 最寄駅: JR仙台駅 徒歩13分 / 地下鉄広瀬通駅 徒歩19分
- 取扱: エイブル仙台駅前店 022-221-3663
- エイブル建物ページ: https://www.able.co.jp/archive/miyagi/bld-5471188/
