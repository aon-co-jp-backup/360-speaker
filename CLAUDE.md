
## aruaru-llm 呼び出しの Connect 化 (2026-11-05)

- aruaru-llm の REST 全廃に伴い、本リポジトリの呼び出し先を `POST /aruaru_llm.v1.Llm/<Method>`(JSON本文)へ変更した(旧 `/v1/...` は aruaru-llm 側で削除済み)。
- 対象は aruaru-llm を呼ぶ箇所のみ。本リポジトリ自身のAPI・他サービス(aruaru-search 等)の呼び出しは別途。
- 未検証: ビルド/実サーバー往復(aruaru-llm の `connect-migration` ブランチが VPS 未反映のため)。aruaru-llm の main マージ・VPS反映と同時に反映すること。
