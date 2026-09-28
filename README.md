# AI 基础学习练习代码

个人学习 AI 开发基础过程中的练习代码仓库。

## 内容

| 文件 | 说明 |
| --- | --- |
| `code/LLM-api.py` | FastAPI + 智谱 GLM API 的流式对话接口练习（SSE 流式输出） |

## 运行

```bash
# 1. 设置 API Key 环境变量
export ZHIPU_API_KEY="你的key"

# 2. 安装依赖
pip install fastapi uvicorn openai

# 3. 启动服务
uvicorn code.LLM-api:app --reload
```

接口：`POST /api/ai/chat`，入参 `{"question": "..."}`，返回 SSE 流式响应。
