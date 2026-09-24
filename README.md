# Qwen3.8 Flash API (qwen3.8-flash / qwen3.8flash) — llm guide with published pricing

> **input $0.0914; cached_input $0.0114; explicit_cached_input $0.0114** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-1fbf82)** · **[Get an API key](https://go.apimart.ai/k-c67a25)**

Everything here refers to **qwen3.8-flash** — also written **qwen3.8flash** or **qwen3.8 flash**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `input` | $0.0914 |
| `cached_input` | $0.0114 |
| `explicit_cached_input` | $0.0114 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $9.1429 |
| 1,000 | $91.4288 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"qwen3.8-flash","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
