# 📐 标准

## API

### OpenAI

#### 聊天请求

示例：

```sh
curl https://api.openai.com/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -d '{
    "model": "gpt-4o-mini",
    "messages": [
      {
        "role": "system",
        "content": "你是一个乐于助人的助手。"
      },
      {
        "role": "user",
        "content": "用一句话介绍什么是大语言模型。"
      }
    ],
    "max_tokens": 100,
    "temperature": 0.7
  }'

```

参数说明:

- `model`
- `messages`
  - `role`
  - `content`
- `max_tokens`
- `temperature`
- `stream`

#### 图像生成请求

示例：

```sh
curl https://api.openai.com/v1/images/generations \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -d '{
    "prompt": "一只可爱的水獭宝宝戴着黄色帽子坐在沙发上",
    "n": 1,
    "size": "1024x1024"
  }'

```

参数说明：

- `prompt`
- `n`
- `size`


### Anthropic

示例：

```sh
curl https://api.anthropic.com/v1/messages \
  -H "Content-Type: application/json" \
  -H "x-api-key: $ANTHROPIC_API_KEY" \
  -H "anthropic-version: 2023-06-01" \
  -d '{
    "model": "claude-sonnet-4-20250514",
    "max_tokens": 1024,
    "temperature": 0.7,
    "top_p": 0.9,
    "messages": [
      {"role": "user", "content": "Write a short poem about coding"}
    ]
  }'

```
参数说明：

- `model`
- `max_tokens`
- `temperature`
- `top_p`
- `messages`
  - `role`
  - `content`
- `system`


## MCP


### 精选项目

- [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers)
- [upstash/context7](https://github.com/upstash/context7)
- [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp)
- [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp)
- [github/github-mcp-server](https://github.com/github/github-mcp-server)


## SKILL


### 精选项目

- [anthropics/skills](https://github.com/anthropics/skills)
- [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)
- [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills)
- [VoltAgent/awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills)
- [sickn33/antigravity-awesome-skills](https://github.com/sickn33/antigravity-awesome-skills)

## A2A


## ACP

