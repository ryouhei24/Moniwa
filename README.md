# Moniwa

### 開発概要
* フロントエンド: HTML & CSS
* バックエンド: Node.js(JavaScript)
* データベース: SQLite
***

### git操作
0. 【初期設定】 リモートリポジトリをローカルの空のディレクトリにクローンする
```
git clone https://github.com/ryouhei24/Moniwa.git
```

1. リモートリポジトリの最新の状態をローカル環境に取り込む
```
git checkout main
git pull origin main
```
ローカルでのmainブランチは必ずリモートリポジトリと同じ状態にしておく。<br>
**作業をする場合は必ず新しいブランチ（既存のブランチ）に移動してから**

2. ブランチを作成して移動する
```
git checkout -b [ブランチ名]
```
もしくは、既存のブランチに移動
```
git checkout [ブランチ名]
```
ローカルにあるブランチの確認
```
git branch
```

> **ブランチ名の決め方**<br>
機能の追加 → `feature/[追加する機能名]`
不具合修正 → `fix/[修正する機能名]`


3. 作業が一段落したら
```
git add . 
#もしくは git add [変更したファイル名]
git commit -m "ここに作業内容を書く"
```

4. ローカルのブランチをリモートリポジトリにプッシュする
```
git push origin [今いるブランチ名]
```

5. Githubでプルリクエストをする<br>
**mergeは必ずプルリクエストを確認してから実行する**
