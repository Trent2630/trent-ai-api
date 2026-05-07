# 🦞 叁十 AI API

[DeepSeek V4 Flash](https://api-docs.deepseek.com) 国内直连 API 服务。

## 特点

- 🇨🇳 **国内直连** — 无需翻墙，无需配置代理
- 📦 **标准 OpenAI 兼容接口** — 一行代码切换
- ⚡ **DeepSeek V4 Flash** — 1M 上下文窗口，384K 最大输出
- 💰 **官方同价** — ¥2/百万 tokens
- 📱 **微信支付** — 便捷充值

## 快速开始

### 1. 注册账号
访问服务地址：https://limit-francisco-charitable-sur.trycloudflare.com
点击「免费注册」，1 分钟完成注册。

### 2. 生成 API Key
登录后进入 Token 管理页面，创建一个新的 API Key。

### 3. 调用

```python
from openai import OpenAI

client = OpenAI(
    api_key="sk-你的key",
    base_url="https://limit-francisco-charitable-sur.trycloudflare.com/v1"
)

response = client.chat.completions.create(
    model="deepseek-chat",
    messages=[{"role": "user", "content": "你好"}]
)
print(response.choices[0].message.content)
```

## 价格

| 套餐 | 价格 | Token 量 | 适用 |
|------|------|---------|------|
| 体验包 | ¥10 | ~3500 万 | 个人试用 1-2 月 |
| 标准包 | ¥30 | ~1 亿 | 小团队月用量 |
| 畅用包 | ¥50 | ~1.75 亿 | 重度用户 |

## 联系

微信：`18620566303`

---

> 基于 [One API](https://github.com/songquanpeng/one-api) v0.6.10 搭建
