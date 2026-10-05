# English Speaking Practice

英語スピーキングを練習するための静的サイト(GitHub Pages等でそのまま公開可能)。

## ページ構成(2026-10-05追加)

- `index.html` — トップ選択ページ。「自作アプリで練習」と「ChatGPTで英会話レッスン」の2つへ振り分ける。
- `app.html` — 自作の音声英会話練習アプリ本体(旧`index.html`)。Groq API(ユーザー自身のAPIキー、ブラウザのlocalStorageに保存)を使った発音/ニュアンス判定機能を含む。
- `chatgpt.html` — ChatGPTを「オンライン英会話講師」として使うための説明専用ページ。実際のレッスンはこのサイト上ではなくChatGPTの画面上で行う(このページ自体はChatGPT APIを呼ばない)。レッスン用プロンプト全文の表示・コピー、レッスンブック(A〜F)の構成、よく使う進行コマンドの早見表を掲載。レッスンブックのファイル本体(各冊の実際の本文)はこのリポジトリでは配布しておらず、利用者自身が用意してChatGPT側にアップロードする想定。

## 経緯

元々は`index.html`単体の自作アプリのみだったが、「ChatGPTに直接プロンプトを貼って英会話練習する」という別の使い方を、同じサイト内で案内できるようにしたいという要望に基づき、トップ選択ページ+説明ページを追加した(依頼・設計判断の詳細は`gurii-gabreh/progress-tracker-dashboard`の`data/tasks.json`・`data/concept-log.json`を参照)。
