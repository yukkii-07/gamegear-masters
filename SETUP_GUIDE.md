# 🚀 GameGear Masters - 運用開始までの完全ガイド

このガイドでは、サイトの公開から日々の運用・更新方法まで、すべてをわかりやすく解説します。

---

## 📋 目次

1. [サイト公開までの手順（初回のみ）](#1-サイト公開までの手順初回のみ)
2. [アフィリエイトリンクの設定](#2-アフィリエイトリンクの設定)
3. [日々の運用・更新方法](#3-日々の運用更新方法)
4. [よくある変更・追加作業](#4-よくある変更追加作業)
5. [トラブルシューティング](#5-トラブルシューティング)

---

## 1. サイト公開までの手順（初回のみ）

### ステップ1: ファイルの確認 ✅

以下のファイルがすべて揃っているか確認してください：

```
GameGear Masters/
├── index.html                 ✅ トップページ
├── gaming-mouse.html          ✅ マウスページ
├── gaming-keyboard.html       ✅ キーボードページ
├── gaming-headset.html        ✅ ヘッドセットページ
├── gaming-monitor.html        ✅ モニターページ
├── gaming-chair.html          ✅ チェアページ
├── gaming-mousepad.html       ✅ マウスパッドページ
├── js/
│   └── main.js               ✅ JavaScript
├── README.md                  ✅ プロジェクト説明
└── SETUP_GUIDE.md            ✅ このファイル
```

### ステップ2: GitHubアカウント作成（無料）

**なぜGitHubが必要？**
- ファイルを安全に保管できる
- 無料でサイトを公開できる（GitHub Pages）
- 更新履歴が自動で保存される
- いつでも元に戻せる

**手順:**
1. https://github.com/ にアクセス
2. 「Sign up」をクリック
3. メールアドレス・パスワードを入力して登録
4. メール認証を完了

### ステップ3: GitHubにファイルをアップロード 📤

#### 方法A: GitHub Desktop（おすすめ・初心者向け）

**GitHub Desktopのインストール:**
1. https://desktop.github.com/ からダウンロード
2. インストール後、GitHubアカウントでログイン

**リポジトリ作成:**
1. 「File」→「New Repository」をクリック
2. 設定:
   - Name: `gamegear-masters`（英数字のみ）
   - Description: `ゲーミングデバイスレビューサイト`
   - Local Path: ファイルがあるフォルダを選択
   - ✅ Initialize this repository with a README（チェック）
3. 「Create Repository」をクリック

**ファイルをアップロード:**
1. GitHub Desktopで作成したリポジトリを開く
2. すべてのHTMLファイルをリポジトリフォルダにコピー
3. 左側に変更ファイル一覧が表示される
4. 下部の「Summary」に `初回アップロード` と入力
5. 「Commit to main」をクリック
6. 右上の「Push origin」をクリック（GitHub.comにアップロード）

#### 方法B: Web上で直接アップロード（簡単・推奨）

1. https://github.com/new にアクセス
2. Repository name: `gamegear-masters`
3. Public（公開）を選択
4. ✅ Add a README file にチェック
5. 「Create repository」をクリック
6. 「uploading an existing file」をクリック
7. すべてのファイルをドラッグ&ドロップ
8. 「Commit changes」をクリック

### ステップ4: GitHub Pagesで公開 🌐

**手順:**
1. GitHubのリポジトリページを開く
2. 「Settings」タブをクリック
3. 左メニューから「Pages」をクリック
4. Source: `Deploy from a branch`
5. Branch: `main` を選択、フォルダは `/ (root)` を選択
6. 「Save」をクリック
7. **5分ほど待つ**と、上部に緑色のバーで URL が表示される
   - 例: `https://あなたのユーザー名.github.io/gamegear-masters/`

**🎉 これでサイトが公開されました！**

---

## 2. アフィリエイトリンクの設定

### Amazonアソシエイト登録

**手順:**
1. https://affiliate.amazon.co.jp/ にアクセス
2. 「無料アカウント作成」をクリック
3. 必要情報を入力:
   - Amazonアカウント（持っていなければ作成）
   - サイト情報（GitHub PagesのURL）
   - 運営者情報
   - 支払い情報（銀行口座）
4. 審査申請（通常1-3日）
5. 承認されたら、アソシエイトIDが発行される

**アフィリエイトリンクの作成:**
1. Amazonアソシエイトにログイン
2. 上部の検索バーで商品名を検索（例: Logicool G PRO X SUPERLIGHT 2）
3. 「リンク作成」ボタンをクリック
4. 「テキストリンク」を選択
5. 生成されたURLをコピー

**HTMLファイルへの設定:**

現在のコード（プレースホルダー）:
```html
<a href="#" class="...">
    <i class="fab fa-amazon mr-2"></i>Amazonで見る
</a>
```

↓ 以下のように変更:
```html
<a href="https://www.amazon.co.jp/dp/B0XXXXXXXX?tag=あなたのアソシエイトID-22" 
   target="_blank" rel="noopener"
   class="...">
    <i class="fab fa-amazon mr-2"></i>Amazonで見る
</a>
```

### 楽天アフィリエイト登録

**手順:**
1. https://affiliate.rakuten.co.jp/ にアクセス
2. 「新規会員登録」をクリック
3. 楽天会員IDでログイン（なければ作成）
4. サイト情報を登録
5. 即日利用開始可能

**リンク作成:**
1. 楽天市場で商品を検索
2. 商品ページで「商品リンク」をクリック
3. 生成されたURLをコピー
4. HTMLファイルの `href="#"` を置き換え

---

## 3. 日々の運用・更新方法

### 基本の更新フロー

```
ローカルでファイル編集
    ↓
動作確認（ブラウザでindex.htmlを開く）
    ↓
GitHubにアップロード
    ↓
5分後に本番サイトに反映
```

### 更新手順（GitHub Desktop使用）

**ステップ1: ファイルを編集**
- メモ帳、VS Code等でHTMLファイルを開く
- 必要な箇所を変更
- 保存（Ctrl+S / Cmd+S）

**ステップ2: ローカルで確認**
- 編集したHTMLファイルをダブルクリック
- ブラウザで表示を確認
- 問題なければ次へ

**ステップ3: GitHubに反映**
1. GitHub Desktopを開く
2. 左側に変更ファイルが表示される
3. 「Summary」に変更内容を入力（例: `1位の商品を更新`）
4. 「Commit to main」をクリック
5. 「Push origin」をクリック

**ステップ4: 本番確認**
- 5分ほど待つ
- `https://あなたのユーザー名.github.io/gamegear-masters/` にアクセス
- Ctrl+F5（強制再読み込み）で最新版を確認

### 更新手順（GitHub Web使用 - PCスキル不要）

1. https://github.com/あなたのユーザー名/gamegear-masters にアクセス
2. 編集したいファイル（例: `gaming-mouse.html`）をクリック
3. 右上の鉛筆アイコン（✏️）をクリック
4. ファイルを編集
5. 下部の「Commit changes」をクリック
6. 変更内容を入力して「Commit changes」ボタンをクリック

---

## 4. よくある変更・追加作業

### 4-1. 商品を追加する

**例: ゲーミングマウスに新商品を追加**

**場所:** `gaming-mouse.html`

**手順:**
1. ファイルを開く
2. ランキングセクションを見つける（`<section id="ranking">`）
3. 既存の商品カード（`<article class="...">`）をコピー
4. 以下の部分を変更:

```html
<article class="bg-gray-800 rounded-xl p-6 border border-purple-500/30 card-hover">
    <div class="flex items-center mb-4">
        <div class="text-4xl font-bold text-purple-400 mr-4">8</div>  <!-- ← 順位を変更 -->
        <div>
            <h3 class="text-xl font-bold">新商品名</h3>  <!-- ← 商品名を変更 -->
            <p class="text-sm text-gray-400">特徴を入力</p>  <!-- ← 特徴を変更 -->
        </div>
    </div>
    <div class="grid grid-cols-3 gap-2 mb-4 text-sm">
        <div class="bg-gray-900 p-2 rounded text-center">
            <div class="text-xs text-gray-500">重量</div>
            <div class="font-bold">65g</div>  <!-- ← スペックを変更 -->
        </div>
        <!-- 他のスペックも同様に変更 -->
    </div>
    <p class="text-sm text-gray-300 mb-4">
        商品説明を入力  <!-- ← 説明を変更 -->
    </p>
    <a href="アフィリエイトリンク" class="...">  <!-- ← リンクを追加 -->
        詳細を見る
    </a>
</article>
```

### 4-2. 価格を変更する

**価格表示部分を探す:**
```html
<div class="text-3xl font-bold text-green-400">¥20,900</div>
```

↓ 新しい価格に変更:
```html
<div class="text-3xl font-bold text-green-400">¥19,800</div>
```

**Ctrl+F（検索機能）で一括変更:**
1. `Ctrl+F` で検索ボックスを開く
2. 「¥20,900」と入力
3. すべて見つかった箇所を確認
4. 該当する箇所を「¥19,800」に置き換え

### 4-3. 新しいレビュー記事を追加する

**トップページの「最新レビュー」セクションに追加:**

**場所:** `index.html` の `<section id="reviews">` 内

**既存の記事カードをコピー:**
```html
<article class="card-hover bg-gray-800 rounded-xl overflow-hidden border border-purple-500/30">
    <div class="bg-purple-600 h-48 flex items-center justify-center">
        <i class="fas fa-mouse text-8xl text-white opacity-50"></i>  <!-- ← アイコンを変更 -->
    </div>
    <div class="p-6">
        <div class="flex items-center gap-2 mb-3">
            <span class="bg-purple-600 text-xs px-3 py-1 rounded-full">マウス</span>  <!-- ← カテゴリー -->
            <span class="text-xs text-gray-500">2024年12月更新</span>  <!-- ← 日付を変更 -->
        </div>
        <h3 class="text-xl font-bold mb-3">記事タイトル</h3>  <!-- ← タイトルを変更 -->
        <p class="text-gray-400 text-sm mb-4">記事の説明文</p>  <!-- ← 説明を変更 -->
        <a href="リンク先.html" class="...">  <!-- ← リンク先を指定 -->
            記事を読む <i class="fas fa-arrow-right ml-2"></i>
        </a>
    </div>
</article>
```

### 4-4. ランキング順位を入れ替える

**手順:**
1. 入れ替えたい商品カードをそれぞれコピー
2. 順番を入れ替えて貼り付け
3. 順位表示部分を更新:
   - `<div class="text-4xl font-bold text-purple-400 mr-4">4</div>` の数字を変更
   - ランキングバッジ（1-3位）の場合: `<div class="rank-badge rank-1">1</div>` を変更

### 4-5. サイト名やロゴを変更する

**全ページ共通:**

サイト名が表示されている箇所を検索:
```html
<h1 class="font-gaming text-2xl font-bold gradient-gaming bg-clip-text text-transparent">
    <i class="fas fa-gamepad mr-2"></i>GameGear Masters  <!-- ← ここを変更 -->
</h1>
```

**一括置換（推奨）:**
1. VS Code等のエディタで全ファイルを開く
2. `Ctrl+Shift+F`（全ファイル検索）
3. 「GameGear Masters」を検索
4. すべて新しい名前に置換

### 4-6. 色・デザインを変更する

**主要カラーを変更:**

Tailwind CSSのクラス名を変更するだけでOK:

| 現在の色 | クラス名 | 変更例 |
|---------|---------|--------|
| 紫色 | `purple-600` | `blue-600`（青） / `red-600`（赤） |
| ピンク | `pink-600` | `rose-600`（ローズ） |
| 緑色 | `green-600` | `emerald-600`（エメラルド） |

**例: マウスページのテーマカラーを紫→青に変更**

検索: `purple-`
置換: `blue-`

### 4-7. Google Analyticsを追加する

**手順:**
1. https://analytics.google.com/ でアカウント作成
2. 測定IDを取得（例: `G-XXXXXXXXXX`）
3. 全HTMLファイルの `</head>` タグの直前に以下を追加:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
</head>
```

---

## 5. トラブルシューティング

### Q1: 更新したのにサイトに反映されない

**原因と対処:**
- **キャッシュが残っている** → `Ctrl+F5` で強制再読み込み
- **GitHub Pagesの反映待ち** → 5-10分待つ
- **ファイル名が間違っている** → ファイル名の綴りを確認（大文字小文字も区別）

### Q2: モバイルメニューが動かない

**確認ポイント:**
1. `js/main.js` ファイルが正しくアップロードされているか確認
2. HTMLに以下が書かれているか確認:
   ```html
   <script src="js/main.js"></script>
   ```
3. ブラウザのコンソールを開いてエラーがないか確認（F12キー）

### Q3: リンクが動かない

**確認ポイント:**
- `href="#"` のまま残っていないか確認
- リンク先のファイル名が正しいか確認（例: `gaming-mouse.html`）
- 大文字小文字を間違えていないか確認

### Q4: デザインが崩れた

**対処法:**
1. GitHub Desktopで「History」タブを開く
2. 崩れる前のCommitを右クリック
3. 「Revert This Commit」をクリック
4. 「Push origin」で元に戻す

### Q5: アフィリエイトリンクが動かない

**確認ポイント:**
- Amazonアソシエイトの審査が完了しているか
- アソシエイトIDが正しく入力されているか
- リンクに `https://` が含まれているか

---

## 📅 推奨運用スケジュール

### 毎日
- [ ] Amazonアソシエイトの成果をチェック
- [ ] Google Analyticsでアクセス数を確認

### 週1回
- [ ] 価格変動チェック（値上げ・値下げがあれば更新）
- [ ] 在庫状況確認（売り切れ商品のリンクを修正）
- [ ] 新商品リリース情報チェック

### 月1回
- [ ] ランキング順位の見直し
- [ ] 新商品レビューを1-2件追加
- [ ] Google Search Consoleで検索順位確認

### 3ヶ月に1回
- [ ] 全商品情報の見直し（古い情報の更新）
- [ ] 新カテゴリー追加の検討
- [ ] サイトデザインの改善

---

## 📚 便利なツール・サービス

### 画像編集
- **Canva** (https://www.canva.com/) - 無料でバナー作成
- **Photopea** (https://www.photopea.com/) - 無料のPhotoshop代替

### SEOチェック
- **Google Search Console** (https://search.google.com/search-console)
- **Ubersuggest** (https://neilpatel.com/ubersuggest/) - キーワード調査

### アクセス解析
- **Google Analytics 4** (https://analytics.google.com/)
- **Microsoft Clarity** (https://clarity.microsoft.com/) - ヒートマップ

### エディタ
- **VS Code** (https://code.visualstudio.com/) - 無料・高機能
- **Notepad++** (https://notepad-plus-plus.org/) - 軽量エディタ

---

## 🎓 学習リソース

### HTML/CSS基礎
- **MDN Web Docs** (https://developer.mozilla.org/ja/)
- **ドットインストール** (https://dotinstall.com/)

### アフィリエイト
- **Amazonアソシエイトヘルプ** (https://affiliate.amazon.co.jp/help)
- **楽天アフィリエイトガイド** (https://affiliate.rakuten.co.jp/guides/)

---

## ✅ 初回セットアップチェックリスト

運用開始前に以下をすべて完了させましょう：

- [ ] GitHubアカウント作成
- [ ] リポジトリ作成・ファイルアップロード
- [ ] GitHub Pagesで公開
- [ ] Amazonアソシエイト登録・審査通過
- [ ] 楽天アフィリエイト登録
- [ ] 全商品のアフィリエイトリンク設定
- [ ] Google Analytics設定
- [ ] Google Search Console登録
- [ ] 各ページの動作確認（PC・スマホ）
- [ ] アフィリエイトリンクのクリックテスト

---

## 💡 成功のコツ

1. **継続が大事**: 週1回は必ず更新する
2. **ユーザー目線**: 「自分が買うなら何を知りたいか」を考える
3. **正直なレビュー**: 良い点だけでなく欠点も書く（信頼性UP）
4. **データを見る**: Google Analyticsで人気記事を分析
5. **SNSも活用**: Twitter/Xで記事を拡散

---

## 📞 サポートが必要な時

### コミュニティで質問
- **Stack Overflow** (https://ja.stackoverflow.com/) - プログラミング全般
- **GitHub Community** (https://github.community/) - GitHub関連

### 公式サポート
- **GitHub Support** (https://support.github.com/)
- **Amazonアソシエイトサポート** (サイト内から問い合わせ)

---

**これであなたも今日からアフィリエイター！頑張ってください！🚀✨**

最終更新: 2024年12月