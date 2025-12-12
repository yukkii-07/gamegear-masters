# 📝 更新用テンプレート集

コピー&ペーストで使える、よくある更新作業のテンプレートです。

---

## 🖱️ 新商品カードを追加（簡易版）

```html
<article class="bg-gray-800 rounded-xl p-6 border border-purple-500/30 card-hover">
    <div class="flex items-center mb-4">
        <div class="text-4xl font-bold text-purple-400 mr-4">順位</div>
        <div>
            <h3 class="text-xl font-bold">商品名</h3>
            <p class="text-sm text-gray-400">一言説明</p>
        </div>
    </div>
    <div class="grid grid-cols-3 gap-2 mb-4 text-sm">
        <div class="bg-gray-900 p-2 rounded text-center">
            <div class="text-xs text-gray-500">重量</div>
            <div class="font-bold">60g</div>
        </div>
        <div class="bg-gray-900 p-2 rounded text-center">
            <div class="text-xs text-gray-500">DPI</div>
            <div class="font-bold">32,000</div>
        </div>
        <div class="bg-gray-900 p-2 rounded text-center">
            <div class="text-xs text-gray-500">価格</div>
            <div class="font-bold text-green-400">¥20,000</div>
        </div>
    </div>
    <p class="text-sm text-gray-300 mb-4">
        ここに商品説明を入力します。特徴や魅力を簡潔に書きましょう。
    </p>
    <div class="flex gap-2">
        <a href="AmazonアフィリエイトURL" target="_blank" rel="noopener" 
           class="flex-1 bg-purple-600 hover:bg-purple-500 text-white py-2 rounded text-center text-sm transition">
            <i class="fab fa-amazon mr-1"></i>Amazon
        </a>
        <a href="楽天アフィリエイトURL" target="_blank" rel="noopener"
           class="flex-1 bg-blue-600 hover:bg-blue-500 text-white py-2 rounded text-center text-sm transition">
            <i class="fas fa-store mr-1"></i>楽天
        </a>
    </div>
</article>
```

---

## 📰 新着レビュー記事カード

```html
<article class="card-hover bg-gray-800 rounded-xl overflow-hidden border border-purple-500/30">
    <div class="bg-purple-600 h-48 flex items-center justify-center">
        <i class="fas fa-mouse text-8xl text-white opacity-50"></i>
    </div>
    <div class="p-6">
        <div class="flex items-center gap-2 mb-3">
            <span class="bg-purple-600 text-xs px-3 py-1 rounded-full">マウス</span>
            <span class="text-xs text-gray-500">2024年12月更新</span>
        </div>
        <h3 class="text-xl font-bold mb-3">記事タイトル</h3>
        <p class="text-gray-400 text-sm mb-4">
            記事の説明文を入力。どんな内容か簡潔に紹介しましょう。
        </p>
        <a href="リンク先.html" class="text-purple-400 hover:text-purple-300 font-bold inline-flex items-center">
            記事を読む <i class="fas fa-arrow-right ml-2"></i>
        </a>
    </div>
</article>
```

---

## 🏆 ランキングバッジ付き商品（1-3位用）

### 1位用

```html
<article class="relative card-hover bg-gray-800 rounded-2xl p-8 mb-8 border-2 border-yellow-500">
    <div class="rank-badge rank-1">1</div>
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
        <div class="lg:col-span-1">
            <div class="bg-gray-900 rounded-xl p-6 flex items-center justify-center h-64">
                <i class="fas fa-mouse text-9xl text-purple-400"></i>
            </div>
        </div>
        <div class="lg:col-span-2">
            <div class="flex items-start justify-between mb-4">
                <div>
                    <h3 class="text-3xl font-bold mb-2">商品名</h3>
                    <p class="text-gray-400">一言説明</p>
                </div>
                <div class="text-right">
                    <div class="text-3xl font-bold text-green-400">¥20,900</div>
                    <p class="text-xs text-gray-500">Amazon価格</p>
                </div>
            </div>

            <div class="bg-gray-900 rounded-xl p-6 mb-4">
                <!-- スペック表 -->
                <div class="space-y-3">
                    <div class="flex justify-between border-b border-gray-800 pb-2">
                        <span class="text-gray-400">重量</span>
                        <span class="font-bold text-yellow-400">60g（超軽量）</span>
                    </div>
                    <div class="flex justify-between border-b border-gray-800 pb-2">
                        <span class="text-gray-400">センサー</span>
                        <span class="font-bold">HERO 2（32,000 DPI）</span>
                    </div>
                    <!-- 必要に応じてスペックを追加 -->
                </div>
            </div>

            <div class="mb-4">
                <h4 class="font-bold mb-3 flex items-center">
                    <i class="fas fa-check-circle text-green-400 mr-2"></i>
                    おすすめポイント
                </h4>
                <ul class="space-y-2 text-sm text-gray-300">
                    <li class="flex items-start">
                        <i class="fas fa-chevron-right text-purple-400 mr-2 mt-1"></i>
                        <span>ポイント1を記入</span>
                    </li>
                    <li class="flex items-start">
                        <i class="fas fa-chevron-right text-purple-400 mr-2 mt-1"></i>
                        <span>ポイント2を記入</span>
                    </li>
                </ul>
            </div>

            <div class="flex gap-4">
                <a href="AmazonURL" target="_blank" rel="noopener"
                   class="flex-1 bg-yellow-500 hover:bg-yellow-400 text-gray-900 font-bold py-3 rounded-lg text-center transition">
                    <i class="fab fa-amazon mr-2"></i>Amazonで見る
                </a>
                <a href="楽天URL" target="_blank" rel="noopener"
                   class="flex-1 bg-blue-600 hover:bg-blue-500 text-white font-bold py-3 rounded-lg text-center transition">
                    <i class="fas fa-store mr-2"></i>楽天で見る
                </a>
            </div>
        </div>
    </div>
</article>
```

---

## 📊 スペック比較表

```html
<div class="bg-gray-800 rounded-xl p-6 border border-purple-500/30">
    <h3 class="text-2xl font-bold mb-6">スペック比較表</h3>
    <div class="overflow-x-auto">
        <table class="w-full text-sm">
            <thead>
                <tr class="border-b border-gray-700">
                    <th class="text-left py-3 px-4">製品名</th>
                    <th class="text-center py-3 px-4">重量</th>
                    <th class="text-center py-3 px-4">センサー</th>
                    <th class="text-center py-3 px-4">価格</th>
                    <th class="text-center py-3 px-4">評価</th>
                </tr>
            </thead>
            <tbody>
                <tr class="border-b border-gray-800 hover:bg-gray-700 transition">
                    <td class="py-3 px-4 font-bold">商品A</td>
                    <td class="py-3 px-4 text-center">60g</td>
                    <td class="py-3 px-4 text-center">HERO 2</td>
                    <td class="py-3 px-4 text-center text-green-400">¥20,900</td>
                    <td class="py-3 px-4 text-center">⭐⭐⭐⭐⭐</td>
                </tr>
                <tr class="border-b border-gray-800 hover:bg-gray-700 transition">
                    <td class="py-3 px-4 font-bold">商品B</td>
                    <td class="py-3 px-4 text-center">54g</td>
                    <td class="py-3 px-4 text-center">Focus Pro</td>
                    <td class="py-3 px-4 text-center text-green-400">¥22,800</td>
                    <td class="py-3 px-4 text-center">⭐⭐⭐⭐⭐</td>
                </tr>
                <!-- 行を追加 -->
            </tbody>
        </table>
    </div>
</div>
```

---

## 🎨 カラーバリエーション

サイトの雰囲気を変える時に使える色の組み合わせ：

### 青系（クール）
```html
<!-- ヘッダー -->
class="bg-gradient-to-r from-blue-600 to-cyan-600"

<!-- ボタン -->
class="bg-blue-600 hover:bg-blue-700"

<!-- アクセントカラー -->
class="text-blue-400"
```

### 赤系（情熱）
```html
<!-- ヘッダー -->
class="bg-gradient-to-r from-red-600 to-pink-600"

<!-- ボタン -->
class="bg-red-600 hover:bg-red-700"

<!-- アクセントカラー -->
class="text-red-400"
```

### 緑系（ゲーミング）
```html
<!-- ヘッダー -->
class="bg-gradient-to-r from-green-600 to-emerald-600"

<!-- ボタン -->
class="bg-green-600 hover:bg-green-700"

<!-- アクセントカラー -->
class="text-green-400"
```

---

## 📢 セールバナー・お知らせ

```html
<div class="bg-gradient-to-r from-yellow-500 to-orange-500 text-white py-3 px-4 rounded-lg mb-8">
    <div class="flex items-center justify-between">
        <div class="flex items-center">
            <i class="fas fa-fire text-2xl mr-3"></i>
            <div>
                <div class="font-bold text-lg">🎉 Amazonブラックフライデー開催中！</div>
                <div class="text-sm">期間限定で最大50%OFF。見逃すな！</div>
            </div>
        </div>
        <a href="セール特集ページ.html" class="bg-white text-orange-600 px-6 py-2 rounded-lg font-bold hover:bg-gray-100 transition">
            詳細を見る →
        </a>
    </div>
</div>
```

---

## 🔍 アコーディオン（開閉式セクション）

```html
<!-- ボタン -->
<button data-accordion-toggle="section-id" 
        class="w-full bg-gray-800 p-4 rounded-lg text-left flex items-center justify-between hover:bg-gray-700 transition">
    <span class="font-bold text-lg">
        <i class="fas fa-table mr-2 text-purple-400"></i>
        スペック比較表を見る
    </span>
    <i class="fas fa-chevron-down accordion-icon transition-transform"></i>
</button>

<!-- 開閉するコンテンツ（初期状態は非表示） -->
<div id="section-id" class="hidden mt-4 bg-gray-800 rounded-lg p-6">
    <!-- ここにコンテンツを入れる -->
    <p class="text-gray-300">
        アコーディオンの中身です。最初は非表示で、ボタンをクリックすると表示されます。
    </p>
</div>
```

---

## 📱 SNSシェアボタン

```html
<div class="flex gap-3 items-center">
    <span class="text-gray-400 text-sm">この記事をシェア:</span>
    
    <!-- Twitter -->
    <a href="https://twitter.com/intent/tweet?url=記事のURL&text=記事タイトル" 
       target="_blank" rel="noopener"
       class="bg-blue-400 hover:bg-blue-500 text-white w-10 h-10 rounded-full flex items-center justify-center transition">
        <i class="fab fa-twitter"></i>
    </a>
    
    <!-- Facebook -->
    <a href="https://www.facebook.com/sharer/sharer.php?u=記事のURL" 
       target="_blank" rel="noopener"
       class="bg-blue-600 hover:bg-blue-700 text-white w-10 h-10 rounded-full flex items-center justify-center transition">
        <i class="fab fa-facebook-f"></i>
    </a>
    
    <!-- LINE -->
    <a href="https://social-plugins.line.me/lineit/share?url=記事のURL" 
       target="_blank" rel="noopener"
       class="bg-green-500 hover:bg-green-600 text-white w-10 h-10 rounded-full flex items-center justify-center transition">
        <i class="fab fa-line"></i>
    </a>
</div>
```

---

## 💬 コメント欄（Disqus）

```html
<!-- ページの最後、フッターの前に追加 -->
<section class="py-16 bg-gray-900">
    <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
        <h2 class="text-2xl font-bold mb-6">コメント</h2>
        <div id="disqus_thread"></div>
        <script>
            var disqus_config = function () {
                this.page.url = 'ページのURL';
                this.page.identifier = 'ページID';
            };
            (function() {
                var d = document, s = d.createElement('script');
                s.src = 'https://あなたのサイト名.disqus.com/embed.js';
                s.setAttribute('data-timestamp', +new Date());
                (d.head || d.body).appendChild(s);
            })();
        </script>
    </div>
</section>
```

---

## 🎁 関連記事リンク

```html
<div class="bg-gray-800 rounded-xl p-6 border border-purple-500/30">
    <h3 class="text-xl font-bold mb-4">
        <i class="fas fa-link text-purple-400 mr-2"></i>
        あわせて読みたい
    </h3>
    <div class="space-y-3">
        <a href="関連記事1.html" class="flex items-center gap-3 p-3 bg-gray-900 rounded-lg hover:bg-gray-700 transition">
            <i class="fas fa-mouse text-2xl text-purple-400"></i>
            <div>
                <div class="font-bold">関連記事タイトル</div>
                <div class="text-sm text-gray-400">簡単な説明文</div>
            </div>
            <i class="fas fa-arrow-right ml-auto text-gray-500"></i>
        </a>
        
        <a href="関連記事2.html" class="flex items-center gap-3 p-3 bg-gray-900 rounded-lg hover:bg-gray-700 transition">
            <i class="fas fa-keyboard text-2xl text-pink-400"></i>
            <div>
                <div class="font-bold">関連記事タイトル2</div>
                <div class="text-sm text-gray-400">簡単な説明文</div>
            </div>
            <i class="fas fa-arrow-right ml-auto text-gray-500"></i>
        </a>
    </div>
</div>
```

---

## 📌 使い方

1. 必要なテンプレートをコピー
2. HTMLファイルの適切な場所に貼り付け
3. テキスト部分（商品名、価格等）を実際の内容に置き換え
4. リンクURLを設定
5. 保存してGitHubにアップロード

---

**これらのテンプレートを使えば、HTMLの知識がなくても簡単に更新できます！✨**