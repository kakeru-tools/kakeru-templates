# Kakeru n8n テンプレート集｜ノーコードAI業務自動化

YouTubeチャンネル「**カケル｜ノーコードAI自動化**」で解説している n8n ワークフローのテンプレート（JSON）を無料配布しています。
動画を見ながらインポートすれば、コードを書かずに同じ自動化を作れます。

## テンプレート一覧

| # | テンプレート | 何ができるか | 解説動画 |
|---|---|---|---|
| 1 | [video01_gmail_to_sheets.json](n8n/video01_gmail_to_sheets.json) | Gmailの問い合わせをスプレッドシートに自動記録 | (公開後にリンク) |
| 3 | [video_03_gmail_ai_bunrui.json](n8n/video_03_gmail_ai_bunrui.json) | 問い合わせメールをAIで自動分類→ラベル付け＆一次返信ドラフト | (公開後にリンク) |
| 4 | [video04_invoice_to_sheets.json](n8n/video04_invoice_to_sheets.json) | 請求書・領収書PDFをAIが読み取り→電帳法対応の索引簿に自動記録 | (公開後にリンク) |
| 6 | [video06_meishi_to_contacts.json](n8n/video06_meishi_to_contacts.json) | 名刺を撮るだけ→AIがデータ化→連絡先リストに自動追記 | (公開後にリンク) |
| 7 | [video07_news_ai_summary_slack.json](n8n/video07_news_ai_summary_slack.json) | 毎朝7時にニュースをAIが3行要約→Slackに自動投稿 | (公開後にリンク) |
| 8 | [video08_meeting_minutes.json](n8n/video08_meeting_minutes.json) | 会議の録音→AIが議事録（要約・決定事項・宿題）→台帳に自動記録 | (公開後にリンク) |

## 使い方（インポート手順）

1. 使いたいテンプレートのJSONファイルをダウンロード
   （ファイルを開いて右上の **Download raw file** ボタン、または `Ctrl+S`）
2. n8n を開く → 右上の **…** メニュー → **Import from File** → ダウンロードしたJSONを選択
3. 各ノードの `REPLACE_WITH_YOUR_...` となっている箇所を自分の値に置き換える
   - 認証情報（Google / Gemini / Slack）の作り方は各動画で解説しています
   - 各ノードの **メモ（Notes）** に、つまずきやすいポイントと対処を書いてあります
4. **Test workflow** で動作確認 → 問題なければ **Active** に

## 注意事項

- テンプレートは無保証です。ご自身の環境でテストしてからお使いください。
- AIの出力（要約・分類・読み取り）は完璧ではありません。重要な判断の前は必ず元データを確認してください。
- メール・名刺・会議録音など**個人情報や機密情報**を扱う場合は、所属組織のルールに従ってください。
- n8n はセルフホスト（自分のPC/サーバー）なら無料で使えます。

## ライセンス

MIT License — 自由に使用・改変・再配布できます。詳細は [LICENSE](LICENSE) を参照。
