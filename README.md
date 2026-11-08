# ai-lab

> **English summary** — A catalog of small, runnable demos that make AI techniques easy to understand. Each repo runs with one command, works offline in mock mode, and explains itself step by step with screenshots.

AI 기술을 **직접 돌려 보며 쉽게 이해하는** 데모 모음입니다.
모든 데모는 명령 하나로 실행되고, 키·모델 없이도 끝까지 도는 연습(mock) 모드가 있으며, README가 스크린샷과 함께 단계별로 설명합니다.

## 데모 목록

| 데모 | 분야 | 무엇을 해 보나요 | 버전 |
|---|---|---|---|
| [에이전트 루프와 MCP 한눈에 보기](https://github.com/LeeGyeongPil/ai-lab-agent-loop-mcp) | 에이전트 | AI 에이전트가 생각하고 MCP 도구를 부르고 결과를 읽는 과정을 실시간 타임라인으로 보여 주는 데모와 입문 안내서. 모의 모델로 바로 실행하거나 로컬 Ollama로 돌릴 수 있습니다. | v0.1.0 |
| [LoRA 파인튜닝 체험 데모](https://github.com/LeeGyeongPil/ai-lab-lora-finetune) | 데이터·파인튜닝 | 예제 100개로 작은 모델에 말투를 가르치고, 학습 전후 답변과 손실 곡선을 HTML 보고서로 확인하는 LoRA 데모 | v0.1.0 |
| [RAG 리랭킹 전후 비교 데모](https://github.com/LeeGyeongPil/ai-lab-rag-rerank) | RAG·검색 | 검색 1단계 결과와 리랭커를 거친 결과를 나란히 놓고, 순위 변화·근거 문장·점수 분포·성적표로 리랭킹의 효과를 직접 확인하는 로컬 데모입니다. | v0.1.0 |

## 공통 사용법

```bash
git clone https://github.com/LeeGyeongPil/<데모 이름>.git
cd <데모 이름>
uv run <시작 명령>   # 각 README의 '30초 만에 실행하기' 참고
```

- 준비물: [uv](https://docs.astral.sh/uv/) (Python 패키지 관리 도구). 실제 모델 모드에는 [Ollama](https://ollama.com)가 필요한 데모도 있습니다.
- 각 데모는 MIT 라이선스입니다. 사용한 모델·데이터의 라이선스는 각 README에 적었습니다.

## English

| Demo | What you try |
|---|---|
| [ai-lab-agent-loop-mcp](https://github.com/LeeGyeongPil/ai-lab-agent-loop-mcp) | A demo and beginner guide that shows an AI agent loop live: each thought, MCP tool call and observation on a timeline. Runs with a mock model or local Ollama. |
| [ai-lab-lora-finetune](https://github.com/LeeGyeongPil/ai-lab-lora-finetune) | Teach a 0.5B model a speaking style with 100 examples via LoRA and inspect an HTML report of loss and before/after answers. |
| [ai-lab-rag-rerank](https://github.com/LeeGyeongPil/ai-lab-rag-rerank) | A local demo that puts first-stage retrieval next to cross-encoder reranking, showing rank moves, evidence highlights, score distribution and a scoreboard. |
