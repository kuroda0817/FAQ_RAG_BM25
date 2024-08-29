# 官公庁FAQ検索検証用プログラム
官公庁FAQ回答のために知識のキーワード検索とベクトル検索を行いたい。
まず足掛かりとして、質問に対する回答集を知識として扱い、正解の回答を検索できるかによって評価する。
## 実装項目
- csvデータの形式変換
- キーワード検索
  - BM25による回答のランク付け
  - topNに入る確率での評価
- ベクトル検索
  - OpenAI embeddingによる質問および回答集のベクトル変換
  - cos類似度計算による回答のランク付け
  - topNに入る確率での評価
## 環境構築
jupyter notebook(pyhon3.9)で動作確認。
google colabなどでも動作するはず...。
## データセット
官公庁よくある質問集データセット(https://huggingface.co/datasets/matsuxr/JaGovFaqs-22k)をダウンロードし、適切なディレクトリに配置すること。
