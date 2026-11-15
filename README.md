# asterstyle.jp

「自然を食す。」サイト（https://asterstyle.jp）のリポジトリ。

## 🌐 本番環境

- **本番URL**: https://asterstyle.jp
- **ホスティング**: Netlify（GitHub `main` ブランチと連携、push で自動デプロイ）
- **DNSレジストラ**: お名前.com（独自ドメイン）
- **メール**: Google Workspace（既存設定、変更禁止）

## 🚀 更新フロー

```bash
# 作業開始前：最新を取得
git pull

# ファイル編集後：変更を送信
git add .
git commit -m "変更内容の説明"
git push
```

push後、1〜2分で https://asterstyle.jp に反映されます。
Netlify側での手動操作は不要です。

## 📁 サイト構成

- `index.html` - トップページ
- `stories.html` - STORIES一覧
- `story-*.html` - 個別記事
- `people.html` - PEOPLE一覧
- `person-*.html` - 個別プロフィール
- `event.html` - 食卓の会・一覧
- `event-*.html` - 個別イベント
- `assets/` - CSS、JS、画像（新サイトで使用）
- `images/` - 旧画像フォルダ（OGP画像含む・保持）

## ⚠️ 重要な注意事項

### 削除・変更禁止
- `images/` フォルダ - 過去にSNSでシェアされたOGP画像を含む
- `googlea23b220c0a1bd3c9.html` - Google Search Console 所有権確認用
- `.nojekyll` - 将来のホスティング変更に備えて保持

### SEO評価の維持
旧URL（`aso.html`、`ensou_haramura.html`、`akagyu_aso.html`）は、
新URLへのリダイレクトファイルに置き換えています。
中身を書き換えると過去のSEO評価が失われるため変更禁止。

### 画像の追加ルール
- 新規画像は `/assets/images/` に配置
- 命名規則：`{撮影者名}_{場所}_{番号}.{拡張子}` 推奨
  （例: `erokumae_aso_20.jpg`）

## 📬 連絡先

- リポジトリ管理: 秋田 正倫（akitamasa503）
- サイトオーナー: 青山 拓（アスタースタイル株式会社）
