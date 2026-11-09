# ai-lab

> **English summary** — Useful open-source programs, libraries and plugins built around AI and automation, plus small runnable demos that make hard techniques easy to understand. Every project runs offline in a mock mode where keys or models are needed, and its README explains it step by step.

AI·자동화 분야에서 **바로 가져다 쓸 수 있는 프로그램·라이브러리·플러그인**과, 어려운 기술을 **직접 돌려 보며 이해하는 데모**를 모았습니다.
키나 모델이 필요한 프로젝트도 연습(mock) 모드로 끝까지 실행해 볼 수 있고, README가 설치부터 사용까지 단계별로 설명합니다.

## 프로그램·CLI

| 이름 | 분야 | 무엇을 하나요 | 버전 |
|---|---|---|---|
| [awsglance — AWS 계정 상황판](https://github.com/LeeGyeongPil/awsglance) | 개발 도구 | AWS 계정 하나의 변경 이력·위험한 설정·지금 확인할 것을 읽기 전용으로 모아 규칙 12개로 판정해 보여 주는 웹 상황판. 자격증명 없이 연습 모드로 먼저 써 볼 수 있습니다. | v0.1.0 |
| [ko-copycheck: 한국어 글 표절 검사 도구](https://github.com/LeeGyeongPil/ko-copycheck) | 개발 도구 | 제출물 폴더를 오프라인으로 비교해 베낀 글과 바꿔 쓴 글을 순위표와 나란히 보기 HTML로 보여 주는 CLI. winnowing 지문과 문장 Dice 유사도를 씁니다. | v0.1.0 |
| [pdf-redpen: LLM 검토 결과를 PDF 형광펜으로](https://github.com/LeeGyeongPil/pdf-redpen) | 개발 도구 | LLM이 인용한 문장을 PDF의 실제 좌표에 연결해 표준 형광펜·메모 주석으로 표시하는 CLI와 라이브러리입니다. 놓친 것을 다시 묻는 재현율 보강 질의를 지원합니다. | v0.1.2 |
| [cache-autopsy: 프롬프트 캐시가 왜 깨졌는지 알려 주는 CLI](https://github.com/LeeGyeongPil/cache-autopsy) | LLM API | 이미 쌓인 요청·응답 기록만으로 프롬프트 캐시 적중률, 놓친 토큰·비용, 깨진 원인(도구 순서, 타임스탬프 등)을 오프라인으로 보여 주고 CI 게이트로도 쓸 수 있습니다. | v0.1.0 |

## 라이브러리

| 이름 | 분야 | 무엇을 하나요 | 버전 |
|---|---|---|---|
| [known-secret-guard: 알려진 비밀값 유출 가드](https://github.com/LeeGyeongPil/known-secret-guard) | 개발 도구 | 에이전트가 이미 아는 비밀값을 base64·URL 인코딩·16진수·반으로 쪼갠 모습으로 내보내는 것을 변형 집합으로 잡는 파이썬 라이브러리·CLI·PreToolUse 훅입니다. | v0.1.0 |
| [llm-format-guard: LLM 답변의 형식·길이 지시 준수 점검 라이브러리](https://github.com/LeeGyeongPil/llm-format-guard) | 평가·관측 | 사용자가 말한 줄 수·글자 수·표 같은 형식 지시를 대화에서 뽑아 다시 알려 주고, 답변을 결정적으로 재서 어긴 경우에만 한 번 고쳐 쓰게 하는 의존성 없는 파이썬 라이브러리입니다. | v0.1.0 |
| [hwpdown — HWP·HWPX를 LLM이 읽기 좋은 마크다운으로](https://github.com/LeeGyeongPil/hwpdown) | RAG·검색 | 공개 규격(HWP 5.0, OWPML)을 직접 파싱해 병합 표·각주·자동 번호를 보존한 마크다운으로 바꾸는 순수 파이썬 라이브러리·CLI입니다. | v0.1.0 |

## 데모

| 이름 | 분야 | 무엇을 하나요 | 버전 |
|---|---|---|---|
| [에이전트 루프와 MCP 한눈에 보기](https://github.com/LeeGyeongPil/ai-lab-agent-loop-mcp) | 에이전트 | AI 에이전트가 생각하고 MCP 도구를 부르고 결과를 읽는 과정을 실시간 타임라인으로 보여 주는 데모와 입문 안내서. 모의 모델로 바로 실행하거나 로컬 Ollama로 돌릴 수 있습니다. | v0.1.1 |
| [LoRA 파인튜닝 체험 데모](https://github.com/LeeGyeongPil/ai-lab-lora-finetune) | 데이터·파인튜닝 | 예제 100개로 작은 모델에 말투를 가르치고, 학습 전후 답변과 손실 곡선을 HTML 보고서로 확인하는 LoRA 데모 | v0.1.1 |
| [evalgate: 프롬프트 평가 게이트](https://github.com/LeeGyeongPil/ai-lab-llm-eval-gate) | 평가·관측 | 프롬프트를 바꾸면 작은 테스트 세트로 자동 채점하고, 점수가 기준보다 떨어지면 CI를 실패시키는 의존성 없는 도구. 녹화된 답변으로 오프라인에서 바로 체험할 수 있습니다. | v0.1.1 |
| [LLM 게이트웨이: 여러 모델을 하나로 묶고 폴백·비용 비교](https://github.com/LeeGyeongPil/ai-lab-llm-gateway) | LLM API | OpenAI 형식·Anthropic·Gemini·로컬 Ollama를 한 인터페이스로 호출하고, 설정만 바꿔 모델을 교체하며 재시도·폴백·라우팅을 직접 돌려 봅니다. 호출마다 토큰·추정 비용·지연을 표로 비교하고, 키 없이 mock 모드로 체험할 수 있습니다. | v0.1.2 |
| [로컬 LLM 속도 벤치마크 (Ollama)](https://github.com/LeeGyeongPil/ai-lab-local-llm-bench) | 로컬 추론 | 내 노트북의 Ollama에 명령 하나로 측정을 돌려 입력 길이와 동시 요청 수가 첫 토큰 지연(TTFT)·초당 토큰·메모리에 주는 영향을 표로 봅니다. 모델·키 없이 녹화된 측정값을 재생하는 연습용 mock 모드를 제공합니다. 양자화 비교와 그래프는 후속 마일스톤입니다. | v0.1.0 |
| [RAG 리랭킹 전후 비교 데모](https://github.com/LeeGyeongPil/ai-lab-rag-rerank) | RAG·검색 | 검색 1단계 결과와 리랭커를 거친 결과를 나란히 놓고, 순위 변화·근거 문장·점수 분포·성적표로 리랭킹의 효과를 직접 확인하는 로컬 데모입니다. | v0.1.1 |

## 공통 사용법

각 레포 README의 '설치'·'빠르게 시작하기'를 따르면 됩니다. 대부분 [uv](https://docs.astral.sh/uv/)(Python) 또는 Node.js만 있으면 되고,
실제 모델 모드가 필요한 프로젝트는 [Ollama](https://ollama.com) 같은 준비물을 README에 적어 두었습니다.
모든 프로젝트는 MIT 라이선스입니다. 사용한 모델·데이터의 라이선스는 각 README에 있습니다.

## English

| Project | Type | What it does |
|---|---|---|
| [awsglance](https://github.com/LeeGyeongPil/awsglance) | tool | A read-only web dashboard for one AWS account that shows who changed what, risky settings and what to check now using 12 plain rules; includes a no-credentials practice mode. |
| [ko-copycheck](https://github.com/LeeGyeongPil/ko-copycheck) | tool | Offline CLI that compares a folder of Korean prose submissions and ranks overlaps using winnowing fingerprints and sentence Dice similarity. |
| [pdf-redpen](https://github.com/LeeGyeongPil/pdf-redpen) | tool | CLI and library that ground quotes from an LLM review to real PDF coordinates and mark them as standard highlight and note annotations, with a recall pass for missed issues. |
| [cache-autopsy](https://github.com/LeeGyeongPil/cache-autopsy) | tool | Offline CLI that shows prompt cache hit rate, missed tokens and cost, and the likely cause of each miss from stored Anthropic and OpenAI request logs. |
| [known-secret-guard](https://github.com/LeeGyeongPil/known-secret-guard) | library | Library, CLI and PreToolUse hook that catch known secrets leaving an agent in encoded or split form by matching a precomputed variant set. |
| [llm-format-guard](https://github.com/LeeGyeongPil/llm-format-guard) | library | Dependency-free Python library that extracts format and length instructions from a chat, re-injects them, measures answers deterministically and repairs only when it strictly reduces violations. |
| [hwpdown](https://github.com/LeeGyeongPil/hwpdown) | library | Pure-Python library and CLI that parses public HWP 5.0 and HWPX specs into Markdown for LLM/RAG, keeping merged tables, footnotes and numbering. |
| [ai-lab-agent-loop-mcp](https://github.com/LeeGyeongPil/ai-lab-agent-loop-mcp) | demo | A demo and beginner guide that shows an AI agent loop live: each thought, MCP tool call and observation on a timeline. Runs with a mock model or local Ollama. |
| [ai-lab-lora-finetune](https://github.com/LeeGyeongPil/ai-lab-lora-finetune) | demo | Teach a 0.5B model a speaking style with 100 examples via LoRA and inspect an HTML report of loss and before/after answers. |
| [ai-lab-llm-eval-gate](https://github.com/LeeGyeongPil/ai-lab-llm-eval-gate) | demo | A dependency-free tool that scores prompt changes on a small test set and fails CI when scores drop below a floor or beyond the noise range. Runs offline by replaying recorded answers. |
| [ai-lab-llm-gateway](https://github.com/LeeGyeongPil/ai-lab-llm-gateway) | demo | Call several LLM providers through one interface, swap models by config, and try retry, fallback and routing. Compare tokens, estimated cost and latency per call. Mock mode needs no API key. |
| [ai-lab-local-llm-bench](https://github.com/LeeGyeongPil/ai-lab-local-llm-bench) | demo | Benchmark a local Ollama server with one command and see how input length and concurrency affect TTFT, tokens/s and memory. A keyless mock mode replays recorded timings. Quantization comparison and charts come in later milestones. |
| [ai-lab-rag-rerank](https://github.com/LeeGyeongPil/ai-lab-rag-rerank) | demo | A local demo that puts first-stage retrieval next to cross-encoder reranking, showing rank moves, evidence highlights, score distribution and a scoreboard. |
