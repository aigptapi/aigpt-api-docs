# AIGPT API

## 💰 AIGPT vs OpenAI — the numbers don't lie

| Service | Model | Input (1M tokens) | Output (1M tokens) |
|---|---|---|---|
| OpenAI | GPT-4o | $30.00 | $180.00 |
| **AIGPT** | **DeepSeek V4-Flash** | **$0.50** | **$1.20** |

> **Save over 90%** — same API format, no surprises.  
> Start in 5 minutes. No registration hassles, no payment barriers.

---

> Affordable, high-performance AI API powered by DeepSeek models.  
> Fully compatible with the OpenAI chat completions format.

## 🚀 Quick Start

### 1. Get your API key
Contact us at wzh786008887@outlook.com to request an API key for testing.

### 2. Make your first request

```bash
curl -X POST http://47.236.50.232:3000/v1/chat/completions \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "deepseek-v4-flash",
    "messages": [{"role": "user", "content": "Hello!"}]
  }'
```

**Expected response:**

```json
{
  "id": "chatcmpl-xxx",
  "object": "chat.completion",
  "created": 1715000000,
  "model": "deepseek-v4-flash",
  "choices": [
    {
      "index": 0,
      "message": {
        "role": "assistant",
        "content": "Hello! How can I help you today?"
      },
      "finish_reason": "stop"
    }
  ],
  "usage": {
    "prompt_tokens": 10,
    "completion_tokens": 20,
    "total_tokens": 30
  }
}
```

## 📌 Endpoint

| Method | URL |
|---|---|
| POST | `http://47.236.50.232:3000/v1/chat/completions` |

Fully compatible with [OpenAI Chat Completions API](https://platform.openai.com/docs/api-reference/chat).

## 🧠 Available Models

| Model ID | Description | Context Window | Knowledge Cut-off |
|---|---|---|---|
| `deepseek-v4-pro` | Flagship reasoning model, ideal for complex Agent tasks | 1M tokens | May 2025 |
| `deepseek-v4-flash` | Efficient chat model, the best choice for value | 1M tokens | May 2025 |

> Fully compatible with the OpenAI Chat Completions API format.  
> More powerful than GPT-4o, at 1/10 the price.


> **Save over 90%** while maintaining near-equivalent quality.  
> No registration hassles, no payment barriers, just pure API access.

## 🔑 Authentication

Include your API key in the `Authorization` header:

```
Authorization: Bearer YOUR_API_KEY
```

Keep your key confidential. Do not expose it in client-side code.

## 📊 Rate Limits

| Plan | Rate Limit | Token Limit |
|---|---|---|
| Free Trial | 60 requests/min | 100K tokens/day |
| Standard | 600 requests/min | Unlimited |

## 💰 Pricing

See `PRICING.md` for detailed pricing and volume discounts.

## 📞 Support

- Email: `wzh786008887@outlook.com`
- Response time: within 24 hours
```


