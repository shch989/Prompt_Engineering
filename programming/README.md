# 프롬프트 엔지니어링에 관한 실용을 정리해둔 문서입니다.

## 기본 템플릿
```
import os
import openai
openai.api_key = os.getenv("OPENAI_API_KEY")

completion = openai.ChatCompletion.create(
  model = "gpt-3.5-turbo",
  messages=[
    {"role": "user", "content": "Hello!"}
  ]
)

print(completion.choices[0].message)
```