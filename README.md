# SNS SafeArea Preview — テンプレート

After Effects のプレビューに SNS の UI とセーフエリアを重ねるツール「SNS SafeArea Preview」の、テンプレート（`.snstpl`）の配布ページです。

- アプリ本体（インストーラー）は [ae-sns-preview-download](https://github.com/catwalking22/ae-sns-preview-download/releases/latest) から入手してください。
- このリポジトリには、配布するテンプレートと、UI のズレの報告だけを置いています（ソースコードはありません）。

## テンプレートの入れ方

1. [Releases](https://github.com/catwalking22/ae-sns-preview-packs/releases/latest) から `sns-templates-YYYY-MM-DD.snstpl` をダウンロードします。
2. ダウンロードしたファイルをダブルクリックするか、アプリのメニューの「ファイル → テンプレートを読み込む」から選びます。
3. アプリが署名を確かめてから取り込みます。署名を確かめられないファイルは取り込みません。

インストーラーには、その時点の最新のテンプレートが入っています。SNS の UI が変わったときに、ここで新しい版を公開します。

### ファイルが本物か確かめる（任意）

各リリースに SHA-256 を載せています。PowerShell で次を実行し、同じ値か確かめてください。

```powershell
Get-FileHash .\sns-templates-YYYY-MM-DD.snstpl -Algorithm SHA256
```

## UI のズレの報告

プレビューの UI や危険エリアが、実際の SNS アプリとずれているときは、[Issue](https://github.com/catwalking22/ae-sns-preview-packs/issues/new/choose) から報告してください。アプリの「ヘルプ → UIのズレを報告する」から開くと、アプリとテンプレートの版が自動で入ります。

- Issue は誰でも見られます。**公開前の動画や、他の人のアカウント名・投稿・個人情報が写ったスクリーンショットは貼らないでください。**

## 注意

- 各 SNS の名称は、それぞれの会社の商標です。このツールは各社とは関係がありません。
- アイコンは独自に作った簡略な図形で、各 SNS の公式のものではありません。
