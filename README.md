# mykodusupport.github.io（サイト全体の公開用パッケージ）

GitHub Pages の「ユーザーサイト」用リポジトリ `mykodusupport.github.io` にそのまま入れる一式です。

## 構成（フォルダ＝URL）

```
https://mykodusupport.github.io/
├─ index.html          … ホーム（アプリ一覧）        → /
├─ assets/
│   └─ mykodu-icon.png … まいこづのアプリアイコン
├─ mykodu/
│   └─ index.html      … ぼくのお小遣い帳のLP      → /mykodu/
└─ .nojekyll
```

- TimeBrave のページを作るときは `timebrave/index.html` を足すだけです（URLは /timebrave/）。
- 法務データ（プライバシーポリシー等）は当面、既存の mykodu-legal リポジトリのまま運用します。
  ホームからは既存URL（https://mykodusupport.github.io/mykodu-legal/privacy-policy.html 等）へリンクしています。
  ※ 既存の法務URLは App Store に登録済みの可能性があるため、消したり移したりしないでください。
  将来このサイト配下（/mykodu/privacy/ 等）へ寄せる場合は、App Store Connect 側のURL差し替えとセットで行います。

## 公開手順（GitHubにログインできる状態で）

1. GitHub で新規リポジトリ `mykodusupport.github.io` を作成（Public、README等は作らない）
2. このフォルダの中身一式（index.html / assets / mykodu / .nojekyll）をリポジトリ直下にアップロード
   - Web画面の「uploading an existing file」でも可（mykodu/index.html は約13MB、Webアップロード上限25MB以内）
   - フォルダごとドラッグ&ドロップすると階層が保たれます
3. コミットすると GitHub Pages が自動で有効になり、数分で https://mykodusupport.github.io/ に反映されます
   （ユーザーサイト用リポジトリは Pages 設定を別途ONにする必要はありません）

## 更新のしかた

- LPを直したら `mykodu/index.html` を差し替えて再アップロード
- アプリが増えたらホーム（index.html）にカードを足し、`アプリ名/index.html` を追加
