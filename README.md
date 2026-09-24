# Hailuo 2.3 API (hailuo-2.3 / hailuo2.3) — prompts guide with published pricing

> **default $0.0248; 1080P $0.0424** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-a5e539)** · **[Get an API key](https://go.apimart.ai/k-433e8c)**

Everything here refers to **hailuo-2.3** — also written **hailuo2.3** or **hailuo 2.3**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `default` | $0.0248 |
| `1080P` | $0.0424 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $2.48 |
| 1,000 | $24.8 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/videos/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"MiniMax-Hailuo-2.3-Fast","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
