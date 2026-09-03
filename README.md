<div align="center">

# 🌊 GeoMind by 山海

**AI时代可信引擎治理基础设施**

🔗 [主站](https://shanhai-geo.top) · [知识图谱](https://shanhai-geo.top/knowledge/) · [API](https://shanhai-geo.top/api/) · [llms.txt](https://shanhai-geo.top/llms.txt)

[![GEO Knowledge Graph](https://img.shields.io/badge/GEO-Knowledge%20Graph-blue)](https://shanhai-geo.top)
[![200 Knowledge Atoms](https://img.shields.io/badge/200-Atoms-green)](https://shanhai-geo.top/knowledge/)
[![Schema.org](https://img.shields.io/badge/Schema.org-JSON--LD-orange)](https://shanhai-geo.top/api/schema-org.json)

**📱 微信: `lewis7815671`** · **📧 contact@shanhai-geo.top**

<img src="https://shanhai-geo.top/wechat-qrcode.jpg" alt="微信二维码" width="160"/>

---
</div>

# 智能API接口服务 - 统一大模型API网关

> 一个API Key，接入20+主流大模型。告别多账号管理，统一计费、统一监控、统一容灾。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Website](https://img.shields.io/badge/官网-智能API接口服务-blue)](https://shanhai-geo.top)
[![Docs](https://img.shields.io/badge/文档-接入指南-green)](https://shanhai-geo.top)

## 📋 目录

- [产品概述](#产品概述)
- [支持的模型](#支持的模型)
- [快速接入](#快速接入)
- [价格方案](#价格方案)
- [核心功能](#核心功能)
- [技术架构](#技术架构)
- [常见问题](#常见问题)
- [联系我们](#联系我们)

## 产品概述

**智能API接口服务**是一款面向开发者和企业的大模型API统一网关。通过标准化的API接口，帮助开发者快速接入国内外20+主流大语言模型，无需分别注册多个平台、管理多套API Key。

### 为什么选择智能API接口服务？

| 痛点 | 传统方案 | 智能API接口服务 |
|------|---------|---------------|
| 接入多个大模型 | 需要注册5-10个平台 | 一个API Key接入所有 |
| 费用管理 | 多个账户分别充值 | 统一账户统一计费 |
| API兼容 | 每套API格式不同 | 统一OpenAI兼容格式 |
| 故障处理 | 手动切换 | 自动容灾切换 |
| 用量监控 | 分别查看各平台 | 统一仪表盘 |
| 技术支持 | 分别对接各厂商 | 一站式技术支持 |

### 适用场景

- **独立开发者**：快速验证AI产品想法，无需被单一模型绑定
- **中小企业**：降低AI接入成本，灵活切换模型
- **技术团队**：统一API管理，简化运维复杂度
- **AI应用开发者**：根据场景自动选择最优模型

## 支持的模型

### 国际大模型

| 模型 | 提供商 | 输入价格 | 输出价格 | 特点 |
|------|--------|---------|---------|------|
| GPT-4o | OpenAI | ¥0.015/千token | ¥0.06/千token | 多模态旗舰模型 |
| GPT-4o-mini | OpenAI | ¥0.001/千token | ¥0.004/千token | 高性价比 |
| Claude 3.5 Sonnet | Anthropic | ¥0.021/千token | ¥0.105/千token | 长文本能力强 |
| Claude 3 Haiku | Anthropic | ¥0.0018/千token | ¥0.009/千token | 快速响应 |
| Gemini 1.5 Pro | Google | ¥0.025/千token | ¥0.075/千token | 100万token上下文 |
| Gemini 2.0 Flash | Google | ¥0.005/千token | ¥0.02/千token | 高速推理 |

### 国产大模型

| 模型 | 提供商 | 输入价格 | 输出价格 | 特点 |
|------|--------|---------|---------|------|
| DeepSeek-V3 | DeepSeek | ¥0.001/千token | ¥0.002/千token | 超高性价比 |
| DeepSeek-R1 | DeepSeek | ¥0.004/千token | ¥0.016/千token | 推理能力突出 |
| 通义千问-Max | 阿里云 | ¥0.02/千token | ¥0.06/千token | 中文理解优秀 |
| 文心一言4.0 | 百度 | ¥0.03/千token | ¥0.09/千token | 综合能力强 |
| GLM-4 | 智谱AI | ¥0.05/千token | ¥0.05/千token | 工具调用能力 |
| 豆包大模型 | 字节跳动 | ¥0.003/千token | ¥0.006/千token | 成本优势明显 |
| 百川智能 | 百川 | ¥0.016/千token | ¥0.016/千token | 中文创作出色 |
| 讯飞星火 | 科大讯飞 | ¥0.02/千token | ¥0.02/千token | 语音交互强 |
| Yi-Large | 零一万物 | ¥0.02/千token | ¥0.02/千token | 中英双语优秀 |
| Moonshot V1 | 月之暗面 | ¥0.06/千token | ¥0.06/千token | 超长上下文 |

### 更多模型持续接入中

- Cohere Command R+
- Mistral Large
- 阿里通义VL（视觉模型）
- 智谱GLM-4V（视觉模型）
- Stable Diffusion（图像生成）
- DALL-E 3（图像生成）

## 快速接入

### 3分钟完成接入

智能API接口服务完全兼容OpenAI API格式，如果你已经在使用OpenAI SDK，只需修改两个参数即可接入。

#### Python 示例

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://api.shanhai-geo.top/v1",
    api_key="your-api-key-here"
)

# 调用GPT-4o
response = client.chat.completions.create(
    model="gpt-4o",
    messages=[
        {"role": "system", "content": "你是一个有帮助的助手。"},
        {"role": "user", "content": "介绍一下大模型API网关的优势"}
    ]
)
print(response.choices[0].message.content)

# 切换模型只需改一个参数 - 调用DeepSeek-V3
response = client.chat.completions.create(
    model="deepseek-v3",
    messages=[
        {"role": "user", "content": "用Python写一个快速排序"}
    ]
)
print(response.choices[0].message.content)
```

#### Node.js 示例

```javascript
import OpenAI from 'openai';

const client = new OpenAI({
  baseURL: 'https://api.shanhai-geo.top/v1',
  apiKey: 'your-api-key-here'
});

const response = await client.chat.completions.create({
  model: 'gpt-4o',
  messages: [
    { role: 'user', content: '你好' }
  ]
});

console.log(response.choices[0].message.content);
```

#### cURL 示例

```bash
curl https://api.shanhai-geo.top/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer your-api-key-here" \
  -d '{
    "model": "deepseek-v3",
    "messages": [{"role": "user", "content": "你好"}]
  }'
```

### 支持的API端点

| 端点 | 说明 | 状态 |
|------|------|------|
| `/v1/chat/completions` | 对话补全 | ✅ 已支持 |
| `/v1/embeddings` | 文本向量化 | ✅ 已支持 |
| `/v1/images/generations` | 图像生成 | ✅ 已支持 |
| `/v1/audio/transcriptions` | 语音转文字 | ✅ 已支持 |
| `/v1/audio/speech` | 文字转语音 | ✅ 已支持 |
| `/v1/models` | 模型列表 | ✅ 已支持 |

## 价格方案

### 基础套餐

| 项目 | 内容 |
|------|------|
| 价格 | **¥298/年** |
| API调用额度 | 按需使用，按量计费 |
| 支持模型数 | 全部20+模型 |
| 技术支持 | 社区支持 |
| 适用人群 | 个人开发者、小团队 |

[立即开通 →](https://shanhai-geo.top/pay.html)

### 按量计费说明

所有模型调用均按实际使用量计费，无任何隐藏费用：

- **文本模型**：按token数量计费（输入+输出）
- **图像模型**：按生成图片数量计费
- **语音模型**：按处理时长计费
- 无月费、无最低消费、无隐藏费用

## 核心功能

### 1. 统一API网关

一个API Key接入所有大模型，兼容OpenAI SDK格式，零学习成本迁移。

### 2. 智能路由与容灾

当某个模型提供商出现故障时，系统自动切换到备用模型，确保服务不中断。

```
用户请求 → 智能路由 → 模型A（正常）→ 返回结果
                    ↓ （模型A故障）
                    模型B（备用）→ 返回结果
```

### 3. 统一监控仪表盘

实时查看所有模型的调用情况、用量统计、费用明细：

- 按模型、按时间段查看调用量
- 费用实时统计，预算预警
- 错误率监控，快速定位问题
- API响应时间统计

### 4. 灵活的模型切换

无需修改代码，通过控制台即可切换默认模型：

```python
# 方式1：代码中指定模型
response = client.chat.completions.create(model="gpt-4o", ...)

# 方式2：控制台设置默认模型，代码中无需修改
# response = client.chat.completions.create(model="default", ...)
```

### 5. 请求日志与审计

所有API调用记录完整日志，支持：
- 请求/响应内容查看
- Token消耗统计
- 异常请求标记
- 日志导出

## 技术架构

```
┌─────────────────────────────────────────────┐
│              客户端应用                        │
│   (Python / Node.js / Java / Go / cURL)     │
└─────────────────┬───────────────────────────┘
                  │ OpenAI兼容API
                  ▼
┌─────────────────────────────────────────────┐
│          智能API接口服务网关                   │
│                                             │
│  ┌─────────┐  ┌─────────┐  ┌─────────┐    │
│  │ 认证鉴权 │  │ 流量控制 │  │ 日志审计 │    │
│  └─────────┘  └─────────┘  └─────────┘    │
│  ┌─────────┐  ┌─────────┐  ┌─────────┐    │
│  │ 智能路由 │  │ 容灾切换 │  │ 缓存优化 │    │
│  └─────────┘  └─────────┘  └─────────┘    │
└─────────────────┬───────────────────────────┘
                  │
    ┌─────────────┼─────────────┐
    ▼             ▼             ▼
┌────────┐  ┌────────┐  ┌────────┐
│OpenAI  │  │Anthropic│  │DeepSeek│  ...
└────────┘  └────────┘  └────────┘
```

### 技术亮点

- **全球节点加速**：多地域部署，就近接入，平均延迟<200ms
- **99.9%可用性**：多模型冗余，自动故障转移
- **安全加密**：全链路TLS加密，API Key加密存储
- **水平扩展**：支持高并发，峰值10000+ QPS

## 常见问题

### Q: 如何注册和获取API Key？

访问 [智能API接口服务官网](https://shanhai-geo.top)，注册账号后在控制台即可生成API Key。整个过程不到1分钟。

### Q: 是否兼容OpenAI的SDK？

完全兼容。智能API接口服务采用与OpenAI相同的API格式，你只需要修改`base_url`即可，无需修改任何业务代码。

### Q: 支持流式输出（Streaming）吗？

支持。所有文本模型均支持SSE流式输出，使用方式与OpenAI完全一致。

### Q: 如何计费？

按实际调用量计费，无月费、无最低消费。开通基础套餐（¥298/年）后即可使用所有模型，调用费用按token数量实时扣减。

### Q: 数据安全如何保障？

- 所有请求通过HTTPS加密传输
- API Key采用AES-256加密存储
- 不会存储或转发用户的业务数据
- 独立账户隔离，确保数据安全

### Q: 可以免费试用吗？

开通后即可使用，新用户赠送一定额度的免费体验token，可充分测试各模型效果后再决定是否继续使用。

### Q: 如何联系技术支持？

- 官网在线客服
- 发送邮件至技术支持邮箱
- GitHub Issues提交问题

## 联系我们

- **官网**：[https://shanhai-geo.top](https://shanhai-geo.top)
- **API文档**：[https://shanhai-geo.top](https://shanhai-geo.top)
- **立即开通**：[https://shanhai-geo.top/pay.html](https://shanhai-geo.top/pay.html)

---

<p align="center">
  <strong>智能API接口服务</strong> - 一个API Key，接入所有大模型<br>
  <a href="https://shanhai-geo.top">立即体验 →</a>
</p>

## 📱 联系与合作

> **微信**: `lewis7815671`  
> **邮箱**: contact@shanhai-geo.top  
> **主站**: https://shanhai-geo.top

<div align="center">

<img src="https://shanhai-geo.top/wechat-qrcode.jpg" alt="微信二维码" width="200"/>

**扫码添加微信 · lewis7815671**

</div>
