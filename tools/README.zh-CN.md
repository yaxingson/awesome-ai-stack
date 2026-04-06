# 工具

## API

### 模型厂商

#### Qwen

示例：

```sh
curl -X POST https://dashscope.aliyuncs.com/compatible-mode/v1/chat/completions \
-H "Authorization: Bearer $DASHSCOPE_API_KEY" \
-H "Content-Type: application/json" \
-d '{
    "model": "qwen-plus",
    "messages": [
        {
            "role": "system",
            "content": "You are a helpful assistant."
        },
        {
            "role": "user",
            "content": "你是谁？"
        }
    ]
}'

```

[API文档](https://help.aliyun.com/zh/model-studio/model-api-reference/)

#### DeepSeek

示例：

```sh
curl -L -X POST 'https://api.deepseek.com/chat/completions' \
-H 'Content-Type: application/json' \
-H 'Accept: application/json' \
-H 'Authorization: Bearer ${DEEPSEEK_API_KEY}' \
--data-raw '{
  "messages": [
    {
      "content": "You are a helpful assistant",
      "role": "system"
    },
    {
      "content": "Hi",
      "role": "user"
    }
  ],
  "model": "deepseek-chat",
  "thinking": {
    "type": "disabled"
  },
  "frequency_penalty": 0,
  "max_tokens": 4096,
  "presence_penalty": 0,
  "response_format": {
    "type": "text"
  },
  "stop": null,
  "stream": false,
  "stream_options": null,
  "temperature": 1,
  "top_p": 1,
  "tools": null,
  "tool_choice": "none",
  "logprobs": false,
  "top_logprobs": null
}'

```

[API文档](https://api-docs.deepseek.com/zh-cn/)

#### MiniMax

示例：

```sh
curl --request POST \
  --url https://api.minimaxi.com/v1/text/chatcompletion_v2 \
  --header 'Authorization: Bearer <token>' \
  --header 'Content-Type: application/json' \
  --data '
{
  "model": "MiniMax-M2.7",
  "messages": [
    {
      "role": "system",
      "name": "MiniMax AI"
    },
    {
      "role": "user",
      "content": "你好",
      "name": "用户"
    }
  ]
}
'

```

[API文档](https://platform.minimaxi.com/docs/guides/models-intro)

### 聚合平台

#### OpenRouter

[文档](https://openrouter.ai/docs/quickstart)

#### N1N

[文档](https://docs.n1n.ai/)


### 第三方服务


## SDK

### Python

- `openai`
- [`anthropic`](https://github.com/anthropics/anthropic-sdk-python)
- `dashscope`


### Node.js

- `@anthropic-ai/sdk`





## CLI

### 自主编码

- `Claude Code`
- `Codex CLI`
- `Gemini CLI`














