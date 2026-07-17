# vexio-reel-media

VEXIO Instagramリール動画の一時公開ホスティング用リポジトリ。

Instagram Graph APIでリール(REELS)を投稿する際、動画ファイルは公開URLで参照する必要がある。
このリポジトリに動画をpushし、GitHubのraw URL経由でInstagram側に読み込ませる。

投稿完了後は容量圧迫を避けるため、古い動画ファイルを定期的に削除してよい
（投稿自体はInstagram側に残るため、このリポジトリの動画は使い捨てでよい）。

管理は `divisions/operations/automation/instagram/post_reel.py`（VEXIO-OSリポジトリ側）から行う。
