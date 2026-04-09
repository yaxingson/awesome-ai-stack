# 🛠️ 工具

## API

### 模型厂商

#### OpenAI


#### Anthropic


#### Google


#### xAI


#### Qwen

API示例：






[API文档](https://help.aliyun.com/zh/model-studio/model-api-reference/)

#### DeepSeek

API示例：

<details>
  <summary>补全对话</summary>
  <div>

  ```http
  @BASE_URL = https://api.deepseek.com 
  @API_KEY = sk-****************************

  POST {{BASE_URL}}/chat/completions HTTP/1.1
  Content-Type: application/json
  Accept: application/json
  Authorization: Bearer {{API_KEY}}

  {
    "model": "deepseek-chat",
    "messages": [
      {
        "role": "system",
        "content": "You are a helpful assistant."
      },
      {
        "role": "user",
        "content": "你是谁？"
      }
    ],
    "thinking":{
      "type":"disabled"
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
  }
  ```
  
  </div>
</details>

<details>
  <summary>`FIM(Fill-In-the-Middle)`补全</summary>
  <div>

  ```http
  @BASE_URL = https://api.deepseek.com/beta
  @API_KEY = sk-****************************

  POST {{BASE_URL}}/completions HTTP/1.1
  Content-Type: application/json
  Accept: application/json
  Authorization: Bearer {{API_KEY}}

  {
    "model": "deepseek-chat",
    "prompt": "很久很久以前, ",
    "echo": false,
    "frequency_penalty": 0,
    "logprobs": 0,
    "max_tokens": 1024,
    "presence_penalty": 0,
    "stop": null,
    "stream": false,
    "stream_options": null,
    "suffix": null,
    "temperature": 1,
    "top_p": 1
  }

  ```
  
  </div>
</details>

<details>
  <summary>列出模型</summary>
  <div>

  ```http
  @BASE_URL = https://api.deepseek.com
  @API_KEY = sk-****************************

  GET {{BASE_URL}}/models HTTP/1.1
  Accept: application/json
  Authorization: Bearer {{API_KEY}}

  ```

  </div>
</details>

<details>
  <summary>查询余额</summary>
  <div>

  ```http
  @BASE_URL = https://api.deepseek.com
  @API_KEY = sk-****************************

  GET {{BASE_URL}}/user/balance HTTP/1.1
  Accept: application/json
  Authorization: Bearer {{API_KEY}}

  ```

  </div>
</details>

[API文档](https://api-docs.deepseek.com/zh-cn/)

#### MiniMax

API示例：

<details>
  <summary>补全对话</summary>
  <div>

  ```http
  @BASE_URL = https://api.minimaxi.com
  @API_KEY = sk-****************************

  POST {{BASE_URL}}/v1/text/chatcompletion_v2 HTTP/1.1
  Content-Type: application/json
  Authorization: Bearer {{API_KEY}}

  {
    "model": "M2-her",
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

  ```

  </div>
</details>


[API文档](https://platform.minimaxi.com/docs/guides/models-intro)

### 聚合平台

#### [OpenRouter](https://openrouter.ai/docs/quickstart)


#### [n1n](https://docs.n1n.ai/)


### [SiliconFlow](https://docs.siliconflow.cn/cn/userguide/introduction)


### 第三方服务


## SDK

### Python

- `openai`
- [`anthropic`](https://github.com/anthropics/anthropic-sdk-python)
- `dashscope`


### Node.js

- `@anthropic-ai/sdk`


## 库和框架

### 模型训练

- [PyTorch]()
- [TensorFlow]()
- [Scikit-learn]()
- [Unsloth]()
- [Hugging Face Transformers]()

### 推理和部署

- [vLLM]()
- [TGI (Text Generation Inference)]()
- [TensorRT-LLM]()

### 检索增强生成

- [LangChain]()
- [LlamaIndex]()
- [Milvus]()
- [Faiss]()

### 构建Agent

- [LangGraph]()
- [CrewAI]()
- [MetaGPT]()
- [OpenAI Agents SDK]()
- [BabyAGI]()
- [AutoGPT]()

## CLI

- [ollama]()
- [tlm]()
