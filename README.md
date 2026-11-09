# ai-lab

> **English summary** — Useful open-source programs, libraries and plugins built around AI and automation, plus small runnable demos that make hard techniques easy to understand. Every project runs offline in a mock mode where keys or models are needed, and its README explains it step by step.

AI·자동화 분야에서 **바로 가져다 쓸 수 있는 프로그램·라이브러리·플러그인**과, 어려운 기술을 **직접 돌려 보며 이해하는 데모**를 모았습니다.
키나 모델이 필요한 프로젝트도 연습(mock) 모드로 끝까지 실행해 볼 수 있고, README가 설치부터 사용까지 단계별로 설명합니다.

## 데모

| 이름 | 분야 | 무엇을 하나요 | 버전 |
|---|---|---|---|
| [에이전트 루프와 MCP 한눈에 보기](https://github.com/LeeGyeongPil/ai-lab-agent-loop-mcp) | 에이전트 | AI 에이전트가 생각하고 MCP 도구를 부르고 결과를 읽는 과정을 실시간 타임라인으로 보여 주는 데모와 입문 안내서. 모의 모델로 바로 실행하거나 로컬 Ollama로 돌릴 수 있습니다. | v0.1.1 |
| [LoRA 파인튜닝 체험 데모](https://github.com/LeeGyeongPil/ai-lab-lora-finetune) | 데이터·파인튜닝 | 예제 100개로 작은 모델에 말투를 가르치고, 학습 전후 답변과 손실 곡선을 HTML 보고서로 확인하는 LoRA 데모 | v0.1.1 |
| [evalgate: 프롬프트 평가 게이트](https://github.com/LeeGyeongPil/ai-lab-llm-eval-gate) | 평가·관측 | 프롬프트를 바꾸면 작은 테스트 세트로 자동 채점하고, 점수가 기준보다 떨어지면 CI를 실패시키는 의존성 없는 도구. 녹화된 답변으로 오프라인에서 바로 체험할 수 있습니다. | v0.1.1 |
| [RAG 리랭킹 전후 비교 데모](https://github.com/LeeGyeongPil/ai-lab-rag-rerank) | RAG·검색 | 검색 1단계 결과와 리랭커를 거친 결과를 나란히 놓고, 순위 변화·근거 문장·점수 분포·성적표로 리랭킹의 효과를 직접 확인하는 로컬 데모입니다. | v0.1.1 |

## 공통 사용법

각 레포 README의 '설치'·'빠르게 시작하기'를 따르면 됩니다. 대부분 [uv](https://docs.astral.sh/uv/)(Python) 또는 Node.js만 있으면 되고,
실제 모델 모드가 필요한 프로젝트는 [Ollama](https://ollama.com) 같은 준비물을 README에 적어 두었습니다.
모든 프로젝트는 MIT 라이선스입니다. 사용한 모델·데이터의 라이선스는 각 README에 있습니다.

## English

| Project | Type | What it does |
|---|---|---|
| [ai-lab-agent-loop-mcp](https://github.com/LeeGyeongPil/ai-lab-agent-loop-mcp) | demo | A demo and beginner guide that shows an AI agent loop live: each thought, MCP tool call and observation on a timeline. Runs with a mock model or local Ollama. |
| [ai-lab-lora-finetune](https://github.com/LeeGyeongPil/ai-lab-lora-finetune) | demo | Teach a 0.5B model a speaking style with 100 examples via LoRA and inspect an HTML report of loss and before/after answers. |
| [ai-lab-llm-eval-gate](https://github.com/LeeGyeongPil/ai-lab-llm-eval-gate) | demo | A dependency-free tool that scores prompt changes on a small test set and fails CI when scores drop below a floor or beyond the noise range. Runs offline by replaying recorded answers. |
| [ai-lab-rag-rerank](https://github.com/LeeGyeongPil/ai-lab-rag-rerank) | demo | A local demo that puts first-stage retrieval next to cross-encoder reranking, showing rank moves, evidence highlights, score distribution and a scoreboard. |
