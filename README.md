[README.md](https://github.com/user-attachments/files/30790185/README.md)
# ゴロクサン 563A運用ノート（PWA版）

## これは何
563Aの購入・分配金・基準価額を記録し、グラフ表示とX投稿ドラフトの自動生成を行うアプリです。
データはこの端末のブラウザ内（localStorage）に保存されます。他の端末とは同期しません。

## Androidのホーム画面にアプリとして追加する手順

### 1. ホスティングする（無料・簡単な方法：GitHub Pages）
1. GitHubで新しいリポジトリを作成（例: gorokusan-tracker）
2. このフォルダの中身（index.html, manifest.json, sw.js, icon-192.png, icon-512.png）をすべてアップロード
3. リポジトリの Settings → Pages → Source を「main branch」に設定して保存
4. 数分後に `https://ユーザー名.github.io/gorokusan-tracker/` でアクセスできるようになります

（GitHubを使わない場合は Vercel や Netlify の無料プランに、このフォルダをそのままドラッグ＆ドロップしてデプロイする方法もあります）

### 2. Androidのホーム画面に追加する
1. スマホのChromeで、公開したURLを開く
2. 右上の「⋮」メニュー → 「ホーム画面に追加」または「アプリをインストール」をタップ
3. ホーム画面にアイコンが追加され、以降はアプリのようにフルスクリーンで起動します

## 注意点
- データはこの端末のブラウザにのみ保存されます。機種変更やブラウザのデータ削除で消えるため、
  必要であればX投稿ドラフトのコピーなどで定期的に控えを残すことをおすすめします。
- 完全にネイティブなAndroidアプリ（Play Store公開）にしたい場合は、このWebアプリを
  Capacitorなどでラップしてビルドする必要があります。その場合はAndroid Studio・
  署名鍵・Google Play開発者アカウント（登録料）が別途必要です。
