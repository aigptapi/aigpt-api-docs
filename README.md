# AIGPT API

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
    "model": "deepseek-chat",
    "messages": [{"role": "user", "content": "Hello!"}]
  }'
```Expected response:
```json
{
  "id": "chatcmpl-xxx",
  "object": "chat.completion",
  "created": 1715000000,
  "model": "deepseek-chat",
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

📌 Endpoint
|Method	|URL                                                                          |
|POST   	|http://47.236.50.232:3000/v1/chat/completions    |
Fully compatible with OpenAI Chat Completions API.

🧠 Available Models
|Model ID		|Description				|Context Window	|
|deepseek-chat	|Fast, general-purpose conversational model	|128K tokens	|
|deepseek-reasoner	|Advanced reasoning with deeper analysis	|128K tokens	|

🔑 Authentication
Include your API key in the Authorization header:

Authorization: Bearer YOUR_API_KEY

Keep your key confidential. Do not expose it in client-side code.

📊 Rate Limits
|Plan	|Rate Limit	|Token Limit
|Free Trial	|60 requests/min	|100K tokens/day
|Standard	|600 requests/min	|Unlimited

💰 Pricing

See PRICING.md for detailed pricing and volume discounts.

📞 Support

    Email: wzh786008887@outlook.com

    Response time: within 24 hours