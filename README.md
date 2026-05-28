# 🦞 DeepChannel — DeepSeek API 中转

> 个人技术实验项目 | 赞助制 | 全球可用

## ⚠️ 重要声明

- 深渠（DeepChannel）是由个人运营的非企业化技术实验项目
- 你的付款是**自愿赞助/捐赠**，API 密钥是附赠礼遇
- 使用即代表你已同意全部法律文件
- **所有赞助不可退款**

## 📜 法律文件（使用前必读）

| 文件 | 说明 |
|------|------|
| [TERMS-OF-SERVICE.md](TERMS-OF-SERVICE.md) | 主协议（含国际仲裁、GDPR、上游断供等条款） |
| [PRICING-AND-PLANS.md](PRICING-AND-PLANS.md) | 套餐定价方案 |

## 🚀 快速开始

### 1. 选择套餐
查看 [PRICING-AND-PLANS.md](PRICING-AND-PLANS.md)，V4 Flash 11档（$0.69起）/ V4 Pro 11档（$0.49起）。

### 2. 赞助支付
通过 Wise 支付至指定账户，备注格式：
```
你的邮箱@gmail.com | Agree ToS
```

### 3. 收取 Key
48 小时内发送 API 密钥至你的邮箱。

### 4. 调用

```python
from openai import OpenAI

client = OpenAI(
    api_key="sk-你的key",
    base_url="https://你的隧道地址/v1"
)

response = client.chat.completions.create(
    model="deepseek-chat",
    messages=[{"role": "user", "content": "你好"}]
)
```

## 📊 模型

| 模型 | 定位 | 每百万售价 |
|------|------|:--:|
| DeepSeek V4 Flash | 量大管饱，日常高频 | $0.9583 |
| DeepSeek V4 Pro | 旗舰性能，复杂推理 | $2.682 |

## 🔗 相关

- 基于 [One API](https://github.com/songquanpeng/one-api) 搭建
- 上游模型：[DeepSeek](https://api-docs.deepseek.com)
