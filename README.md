# OSINT

情報収集・調査・可視化に利用する OSINT（Open Source Intelligence）ツールをまとめるリポジトリです。
各ツールを個別のディレクトリに配置し、この README に概要と関連ドキュメントへのリンクを記載します。

## ツール一覧

| ツール | ディレクトリ | 概要 |
| --- | --- | --- |
| [OSIRIS](#osiris) | [`OSIRIS/`](./OSIRIS/) | 航空機、公開カメラ、災害、ニュースなどの情報を地図上に集約する Web ダッシュボード。 |

## OSIRIS

**OSIRIS（Open Source Intelligence & Reconnaissance Integrated System）** は、複数の公開情報源を地図と調査パネルに集約する OSINT プラットフォームです。
地域ごとの状況把握に加え、ドメインや IP アドレスなどを対象とした調査、AI による情報分析を行えます。

### 主な機能

- **地図による状況把握**：航空機、船舶・港湾、公開カメラ、地震、火災、気象、衛星、紛争地域などの情報をレイヤーとして表示。
- **ニュース・公開投稿の確認**：ニュース配信や公開 Telegram チャンネルの投稿を地図上の情報とあわせて確認。
- **調査ツール（RECON）**：DNS、WHOIS、証明書、IP・ネットワーク情報、脆弱性情報、暗号資産ウォレットなどを調査。
- **AI 支援（OI）**：自然言語による地図操作・情報検索と、公開情報や追加資料に基づく予測・レポート生成。利用には対応する AI プロバイダーの API キーが必要。
- **調査エリアの保存・出力**：地図上にエリアを描画して保存し、範囲や範囲内の情報を GeoJSON・CSV で出力。

### 技術構成・参照先

- **主な技術**：Next.js、React、TypeScript、MapLibre GL JS。
- **ライセンス**：[MIT License](./OSIRIS/LICENSE)。
- **詳細・起動手順**：[OSIRIS の README](./OSIRIS/README.md)。
- **Docker での利用**：[DOCKER.md](./OSIRIS/DOCKER.md)。
- **環境変数の設定例**：[.env.example](./OSIRIS/.env.example)。機能によって外部サービスの API キーや別途バックエンドの設定が必要です。
