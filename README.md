# Toshio Iwai Archive

岩井俊雄氏のアーカイブウェブサイト。

作品、展覧会、メディア掲載などの情報を公開しています。

## リポジトリ構成

```
├── opendata/          # オープンデータ (CSV)
│   └── LICENSE.md     # CC BY 4.0
├── website/           # Hugo 静的サイト
│   ├── content/       # サイトコンテンツ
│   ├── themes/        # Hugo テーマ
│   └── hugo.toml      # Hugo 設定
└── LICENSE.md         # Apache 2.0 (コード用)
```

## ウェブサイト開発

詳細は `website/readme.md` を参照してください。

### ローカル開発

```bash
cd website
hugo server -D
```

ブラウザで http://localhost:1313/ を開いてプレビューできます。

### 本番ビルド

```bash
cd website
hugo
```

ビルド成果物は `website/public/` に出力されます。

## デプロイ

GitHub Actions により自動的にビルド・デプロイされます。

- **公開URL**: https://toshioiwai-archive.github.io/

## 技術スタック

- **静的サイトジェネレーター**: Hugo v0.145.0+
- **ホスティング**: GitHub Pages
- **CI/CD**: GitHub Actions

## ライセンス

このリポジトリには2種類のライセンスが適用されています：

| 対象 | ライセンス |
|------|-----------|
| コード・設定ファイル | [Apache License 2.0](LICENSE.md) |
| オープンデータ (`opendata/`) | [CC BY 4.0](opendata/LICENSE.md) |

## オープンデータ

`opendata/` ディレクトリには、作品・展覧会・メディア掲載などのメタデータが CSV 形式で公開されています。

- **GitHub から直接**: `opendata/*.csv`
- **ウェブサイト経由**: https://toshioiwai-archive.github.io/opendata/
