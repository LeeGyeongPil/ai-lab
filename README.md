# ai-lab

> **English summary** — Useful open-source programs, libraries and plugins built around AI and automation, plus small runnable demos that make hard techniques easy to understand. Every project runs offline in a mock mode where keys or models are needed, and its README explains it step by step.

AI·자동화 분야에서 **바로 가져다 쓸 수 있는 프로그램·라이브러리·플러그인**과, 어려운 기술을 **직접 돌려 보며 이해하는 데모**를 모았습니다.
키나 모델이 필요한 프로젝트도 연습(mock) 모드로 끝까지 실행해 볼 수 있고, README가 설치부터 사용까지 단계별로 설명합니다.

## 프로그램·CLI

| 이름 | 분야 | 무엇을 하나요 | 버전 |
|---|---|---|---|
| [n8n-tidy: n8n 워크플로 JSON 의미 diff·정규화 도구](https://github.com/LeeGyeongPil/n8n-tidy) | 자동화 | n8n 워크플로 JSON 을 git 에 넣을 때 생기는 잡음을 지우고, 노드·연결·프롬프트 변경을 읽기 쉬운 의미 단위 diff 로 보여 주는 명령줄 도구입니다. pre-commit 검사와 git diff 연결도 지원합니다. | v0.1.0 |
| [lora-preflight: LoRA 어댑터 서빙 사전 점검](https://github.com/LeeGyeongPil/lora-preflight) | 데이터·파인튜닝 | PEFT LoRA 어댑터를 vLLM·llama.cpp·Ollama 에 올리기 전에, 설정과 safetensors 헤더만 읽어 런타임별 통과·실패와 수정 명령을 알려 주는 CLI 도구입니다. | v0.1.0 |
| [loraport: LoRA 어댑터 형식 변환·검증](https://github.com/LeeGyeongPil/loraport) | 데이터·파인튜닝 | 맥(mlx-lm)에서 학습한 LoRA 어댑터를 PEFT 형식으로 옮기고, 옮긴 뒤에도 가중치 변화량(dW)이 같은지 모듈별로 수치 확인하는 CLI. | v0.1.0 |
| [pairpick: 선호 쌍 라벨링 브라우저 앱](https://github.com/LeeGyeongPil/pairpick) | 데이터·파인튜닝 | 응답 두 개 중 나은 쪽을 키보드로 고르면 TRL(DPO·KTO)과 LLaMA-Factory가 읽는 파일을 내보냅니다. 서버 없이 브라우저에서만 동작합니다. | v0.1.0 |
| [sft-template-lens: 파인튜닝 데이터 채팅 템플릿 검사기](https://github.com/LeeGyeongPil/sft-template-lens) | 데이터·파인튜닝 | 파인튜닝 JSONL을 모델의 실제 채팅 템플릿과 토크나이저로 렌더해, 학습되는 토큰(손실 마스크)·길이 잘림·형식 오류를 학습 전에 보여 줍니다. 브라우저(업로드 없음)와 Node CLI 모두 지원합니다. | v0.1.0 |
| [awsglance — AWS 계정 상황판](https://github.com/LeeGyeongPil/awsglance) | 개발 도구 | AWS 계정 하나의 변경 이력·위험한 설정·지금 확인할 것을 읽기 전용으로 모아 규칙 12개로 판정해 보여 주는 웹 상황판. 자격증명 없이 연습 모드로 먼저 써 볼 수 있습니다. | v0.1.0 |
| [fixplan: 취약점 알림을 조치 계획으로](https://github.com/LeeGyeongPil/fixplan) | 개발 도구 | 취약점 알림마다 모든 권고를 해소하는 최소 상향 버전을 계산하고, PHP·Node·Python 런타임 제약을 확인해 KEV·EPSS 순으로 정렬하는 CLI. | v0.1.0 |
| [ko-copycheck: 한국어 글 표절 검사 도구](https://github.com/LeeGyeongPil/ko-copycheck) | 개발 도구 | 제출물 폴더를 오프라인으로 비교해 베낀 글과 바꿔 쓴 글을 순위표와 나란히 보기 HTML로 보여 주는 CLI. winnowing 지문과 문장 Dice 유사도를 씁니다. | v0.1.0 |
| [LimitPilot: 사용량 기반 Claude 계정 자동 전환 도구](https://github.com/LeeGyeongPil/limitpilot) | 개발 도구 | 5시간·주간 사용률이 임계에 닿으면 다음 계정으로 자동 전환하는 상주 도구입니다. OS 키체인에 자격증명을 두고, 메뉴바 위젯·대시보드·감시 데몬을 의존성 0 패키지로 제공하며 연습용 목 모드로 안전하게 체험할 수 있습니다. | v0.1.0 |
| [litellm-lint: LiteLLM 프록시 설정 검사기](https://github.com/LeeGyeongPil/litellm-lint) | 개발 도구 | LiteLLM 프록시 config.yaml 의 오타 키, 빠진 환경 변수, 끊어진 폴백·별칭 참조, 하드코딩된 시크릿을 배포 전에 정적으로 잡아 주는 비공식 린터입니다. pre-commit 훅과 JSON Schema 내보내기를 지원합니다. | v0.1.0 |
| [llm-page-lint: LLM이 만든 HTML 페이지의 시각 결함 린터](https://github.com/LeeGyeongPil/llm-page-lint) | 개발 도구 | 헤드리스 Chromium에서 글자 겹침·잘림·화면 밖 이탈·이미지 위 낮은 대비 등 8종 결함을 정답 이미지 없이 결정적으로 측정하고, JSON·HTML 보고서와 종료 코드로 CI 게이트에 쓸 수 있는 CLI·라이브러리. | v0.1.2 |
| [pdf-redpen: LLM 검토 결과를 PDF 형광펜으로](https://github.com/LeeGyeongPil/pdf-redpen) | 개발 도구 | LLM이 인용한 문장을 PDF의 실제 좌표에 연결해 표준 형광펜·메모 주석으로 표시하는 CLI와 라이브러리입니다. 놓친 것을 다시 묻는 재현율 보강 질의를 지원합니다. | v0.1.2 |
| [guarddiff: 가드레일 켜고 끄기 비교 평가 도구](https://github.com/LeeGyeongPil/guarddiff) | 평가·관측 | 같은 문항으로 가드레일 조합별 공격 성공률·과차단·지연·비용을 비교하고, 가드 차단과 모델 거절을 구분해 보여 주는 CLI·라이브러리입니다. | v0.1.0 |
| [handoffmap: 에이전트 추적을 위임 흐름도로 접기](https://github.com/LeeGyeongPil/handoffmap) | 평가·관측 | OpenTelemetry GenAI·OpenInference 추적 파일을 읽어 누가 누구에게 넘겼는지, 도구로 부른 에이전트와 병렬 구간을 Mermaid 순서도와 에이전트별 표로 보여 주는 CLI. | v0.1.0 |
| [promptplan: Langfuse 프롬프트 plan/apply CLI](https://github.com/LeeGyeongPil/promptplan) | 평가·관측 | 프롬프트 파일 폴더와 Langfuse 를 비교해 변경을 미리 보여 주고(plan), 바뀐 것만 새 버전으로 올리거나 라벨만 옮기는(apply) CLI. PR 코멘트와 CI 배포에 맞춰져 있다. | v0.1.0 |
| [cache-autopsy: 프롬프트 캐시가 왜 깨졌는지 알려 주는 CLI](https://github.com/LeeGyeongPil/cache-autopsy) | LLM API | 이미 쌓인 요청·응답 기록만으로 프롬프트 캐시 적중률, 놓친 토큰·비용, 깨진 원인(도구 순서, 타임스탬프 등)을 오프라인으로 보여 주고 CI 게이트로도 쓸 수 있습니다. | v0.1.0 |
| [llm-batchkit: LLM Batch API 파일 검사·분할·병합·재시도 도구](https://github.com/LeeGyeongPil/llm-batchkit) | LLM API | OpenAI·Azure OpenAI·Anthropic Batch API 입력 파일을 업로드 전에 줄 단위로 검사하고, 한도에 맞게 나눠 제출한 뒤, 흩어진 결과·오류 파일을 요청 단위로 다시 모아 실패분만 재시도 파일로 만드는 CLI·라이브러리입니다. 키 없이 mock 서버로 전체 과정을 연습할 수 있습니다. | v0.1.0 |
| [toolcall-conformance: 도구 호출 호환성 검사기](https://github.com/LeeGyeongPil/toolcall-conformance) | LLM API | Ollama·llama.cpp·vLLM·LiteLLM 같은 OpenAI 호환 서버가 도구 호출 규격(스트리밍 델타, tool_choice, 결과 되먹임)을 지키는지 11개 항목으로 검사하는 CLI. 키·GPU 없이 내장 목 서버로 시연합니다. | v0.1.0 |
| [ollama-carry: Ollama 모델 오프라인 이동 도구](https://github.com/LeeGyeongPil/ollama-carry) | 로컬 추론 | 인터넷이 막힌 PC로 Ollama 모델을 옮기는 Dart CLI. 매니페스트와 블롭을 묶어(공유 블롭은 한 번만) FAT32 크기로 나누고, 받는 쪽에서 블롭마다 SHA-256을 검증한 뒤 설치합니다. 연습용 목 모드로 Ollama 없이도 따라 해 볼 수 있습니다. | v0.1.0 |
| [ollama-ctxguard: Ollama 컨텍스트 창 가드 프록시](https://github.com/LeeGyeongPil/ollama-ctxguard) | 로컬 추론 | Ollama 의 /v1 경로가 무시하는 num_ctx 를 모델별 설정대로 적용하고, 프롬프트가 조용히 잘렸는지 응답마다 판정해 알려 주는 로컬 프록시입니다. | v0.1.0 |
| [mcp-schema-shim: MCP 도구 스키마 제공자 호환 계층](https://github.com/LeeGyeongPil/mcp-schema-shim) | MCP·도구 연결 | MCP 도구의 JSON Schema 가 Gemini·OpenAI strict·Anthropic strict 함수 호출 규칙에 맞는지 검사하고 변환하며, 모델이 보낸 인자를 원래 스키마 모양으로 되돌립니다. CLI·stdio 프록시·라이브러리로 쓸 수 있습니다. | v0.1.0 |
| [embed-ab: 임베딩 모델 A/B 검색 비교 도구](https://github.com/LeeGyeongPil/embed-ab) | RAG·검색 | 내 문서와 질문으로 두 임베딩 모델의 검색 품질을 재현율·nDCG·MRR과 신뢰구간, 결과 겹침으로 비교해 모델 교체·재색인 여부를 수치로 결정하게 해 주는 CLI입니다. | v0.1.0 |
| [parseoff: 내 PDF로 파서 비교하기](https://github.com/LeeGyeongPil/parseoff) | RAG·검색 | 설치된 PDF 파서를 내 문서에 모두 돌려 원본 페이지 이미지 옆에 결과를 나란히 보여 주고, 정답 없이 계산되는 지표와 라이선스·설치 크기 경고를 함께 알려 주는 CLI. | v0.1.0 |
| [pgvector-doctor: 필터 검색 HNSW recall 진단](https://github.com/LeeGyeongPil/pgvector-doctor) | RAG·검색 | 내 검색 SQL 의 HNSW 인덱스 recall 을 정확 검색과 비교해 필터 값별로 재고, 목표 recall 을 가장 싸게 맞추는 ef_search·iterative_scan 설정을 추천합니다. | v0.1.0 |

## 라이브러리

| 이름 | 분야 | 무엇을 하나요 | 버전 |
|---|---|---|---|
| [spinstop: 에이전트 도구 호출 루프 가드](https://github.com/LeeGyeongPil/spinstop) | 에이전트 | 에이전트가 같은 도구 호출을 되풀이하거나 맴돌 때 도구 실행 전에 감지해 차단하는 TypeScript 라이브러리와 replay CLI. | v0.1.0 |
| [imeplay — 한국어 IME 조합 입력 E2E 테스트](https://github.com/LeeGyeongPil/imeplay) | 개발 도구 | Enter로 전송하는 채팅 입력창에서 한글 조합 중 Enter가 두 번 전송되거나 마지막 글자가 중복되는 버그를 Playwright 테스트 한 줄로 재현·점검하는 라이브러리와 CLI. | v0.1.0 |
| [known-secret-guard: 알려진 비밀값 유출 가드](https://github.com/LeeGyeongPil/known-secret-guard) | 개발 도구 | 에이전트가 이미 아는 비밀값을 base64·URL 인코딩·16진수·반으로 쪼갠 모습으로 내보내는 것을 변형 집합으로 잡는 파이썬 라이브러리·CLI·PreToolUse 훅입니다. | v0.1.0 |
| [한국어 말투 일관성 검사기 (ko-speechlevel)](https://github.com/LeeGyeongPil/ko-speechlevel) | 평가·관측 | LLM 답변에서 존댓말이 반말로 바뀌는 문장을 위치(offset)와 함께 찾아내는 규칙 기반 검사기. 라이브러리·CLI·스트리밍·promptfoo 단언·vitest 매처를 제공하고 런타임 의존성이 없습니다. | v0.1.2 |
| [korean-asr-eval: 한국어 음성인식 CER 평가](https://github.com/LeeGyeongPil/korean-asr-eval) | 평가·관측 | 한국어 받아쓰기 결과를 이름·지문이 붙은 정규화 프로파일로 채점해 CER·WER을 재현 가능하게 계산하고, 채점 규칙에 따라 모델 순위가 바뀌는지 비교합니다. | v0.1.0 |
| [llm-format-guard: LLM 답변의 형식·길이 지시 준수 점검 라이브러리](https://github.com/LeeGyeongPil/llm-format-guard) | 평가·관측 | 사용자가 말한 줄 수·글자 수·표 같은 형식 지시를 대화에서 뽑아 다시 알려 주고, 답변을 결정적으로 재서 어긴 경우에만 한 번 고쳐 쓰게 하는 의존성 없는 파이썬 라이브러리입니다. | v0.1.0 |
| [ko-pii-roundtrip: 한국어 개인정보 가명 처리·복원](https://github.com/LeeGyeongPil/ko-pii-roundtrip) | LLM API | LLM 호출 전에 이름·주민번호·전화 등을 되돌릴 수 있는 가명으로 바꾸고, 스트리밍 답변에서도 조각 경계와 상관없이 원래 값과 조사를 복원하는 TypeScript 라이브러리. | v0.1.1 |
| [langlock: 로컬 LLM 출력 문자 체계 고정](https://github.com/LeeGyeongPil/langlock) | 로컬 추론 | 한국어로 답하라고 해도 섞여 나오는 한자·가나를 디코딩 단계에서 막는 라이브러리. 바이트 단위 BPE 토크나이저의 반쯤 쓰인 UTF-8 글자까지 추적해 한글은 살리고 금지 문자만 차단합니다. Hugging Face·llama-cpp-python 어댑터와 logit_bias·GBNF·정규식 내보내기, CLI를 제공합니다. | v0.1.1 |
| [MCP Apps 호스트 브리지 (Dart·Flutter)](https://github.com/LeeGyeongPil/mcp-apps-host-dart) | MCP·도구 연결 | MCP Apps의 ui:// 화면을 Dart·Flutter 앱에서 띄우는 호스트 쪽 라이브러리. 핸드셰이크, 도구 호출 권한 정책, 기본 CSP, WebView 메시지 브리지를 제공합니다. | v0.1.1 |
| [hangul-readout: 한국어 TTS 읽기 전처리 라이브러리](https://github.com/LeeGyeongPil/hangul-readout) | 멀티모달 | TTS에 넘기기 직전 숫자·단위·날짜·전화번호를 사람이 읽는 말로 바꾸고, LLM 스트림을 문장 단위로 안전하게 자르는 의존성 없는 TypeScript 라이브러리·CLI. | v0.1.0 |
| [tts-pace: TTS 말속도 측정·맞춤 라이브러리](https://github.com/LeeGyeongPil/tts-pace) | 멀티모달 | 음성의 말속도(쉼을 뺀 초당 음절 수)를 재고, TTS 엔진의 속도 노브와 피치를 유지하는 템포 변환으로 목표 속도에 맞추는 파이썬 라이브러리·CLI입니다. | v0.1.0 |
| [whisper-scrub: Whisper 환각 문장 정리](https://github.com/LeeGyeongPil/whisper-scrub) | 멀티모달 | 무음·잡음 구간의 가짜 문장과 반복 루프를 신호 기반 규칙으로 찾아 지우고, 정답 없이도 전사 품질을 점검하는 라이브러리·CLI. | v0.1.0 |
| [한글 검색 토크나이저](https://github.com/LeeGyeongPil/hangul-search-tokenizer) | RAG·검색 | 조사·어미를 떼어 한국어 키워드 검색의 재현율을 높이는 무의존 동기 토크나이저. MiniSearch·Orama·FlexSearch·VitePress 어댑터와 재현율·정밀도·색인 크기 벤치를 제공합니다. | v0.1.0 |
| [hwpdown — HWP·HWPX를 LLM이 읽기 좋은 마크다운으로](https://github.com/LeeGyeongPil/hwpdown) | RAG·검색 | 공개 규격(HWP 5.0, OWPML)을 직접 파싱해 병합 표·각주·자동 번호를 보존한 마크다운으로 바꾸는 순수 파이썬 라이브러리·CLI입니다. | v0.1.0 |

## 플러그인·확장

| 이름 | 분야 | 무엇을 하나요 | 버전 |
|---|---|---|---|
| [graphtrail: LangGraph 체크포인트 뷰어](https://github.com/LeeGyeongPil/graphtrail) | 에이전트 | LangGraph SqliteSaver 데이터베이스를 코드 실행 없이 안전하게 읽어 실행 타임라인을 재구성하고, 단계 간 상태를 비교하고, JSON·Markdown·HTML 로 내보내는 CLI 와 읽기 전용 VS Code 확장. | v0.1.2 |

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
| [n8n-tidy](https://github.com/LeeGyeongPil/n8n-tidy) | tool | A CLI that strips noise from n8n workflow JSON and shows node, connection and prompt changes as a readable semantic diff, with git and pre-commit integration. |
| [lora-preflight](https://github.com/LeeGyeongPil/lora-preflight) | tool | A CLI that reads a PEFT LoRA adapter's config and safetensors header and predicts whether vLLM, llama.cpp and Ollama will accept it, with a fix command for each problem. |
| [loraport](https://github.com/LeeGyeongPil/loraport) | tool | A CLI that converts LoRA adapters between mlx-lm and PEFT formats and proves per-module dW is unchanged. |
| [pairpick](https://github.com/LeeGyeongPil/pairpick) | tool | A browser-only app to pick the better of two responses by keyboard and export TRL (DPO, KTO) and LLaMA-Factory preference files. |
| [sft-template-lens](https://github.com/LeeGyeongPil/sft-template-lens) | tool | Renders fine-tuning JSONL with a model's real chat template and tokenizer to show loss masks, truncation and format errors before training. Browser and Node CLI. |
| [awsglance](https://github.com/LeeGyeongPil/awsglance) | tool | A read-only web dashboard for one AWS account that shows who changed what, risky settings and what to check now using 12 plain rules; includes a no-credentials practice mode. |
| [fixplan](https://github.com/LeeGyeongPil/fixplan) | tool | A CLI that computes the minimal upgrade clearing every advisory per package (Composer, PyPI, npm), checks runtime constraints, and ranks by KEV and EPSS. |
| [ko-copycheck](https://github.com/LeeGyeongPil/ko-copycheck) | tool | Offline CLI that compares a folder of Korean prose submissions and ranks overlaps using winnowing fingerprints and sentence Dice similarity. |
| [limitpilot](https://github.com/LeeGyeongPil/limitpilot) | tool | A resident tool that switches Claude accounts automatically when session or weekly usage nears a limit. Keeps credentials in the OS keychain, ships a menu-bar widget, dashboard and daemon with zero dependencies, and has a safe practice mode. |
| [litellm-lint](https://github.com/LeeGyeongPil/litellm-lint) | tool | Unofficial static linter for LiteLLM proxy config.yaml that catches typo'd keys, missing env vars, dangling fallbacks/aliases and literal secrets before deploy. |
| [llm-page-lint](https://github.com/LeeGyeongPil/llm-page-lint) | tool | A CLI and library that deterministically measures eight visual defects in LLM-generated HTML pages using headless Chromium, with JSON/HTML reports and exit codes for CI gates. |
| [pdf-redpen](https://github.com/LeeGyeongPil/pdf-redpen) | tool | CLI and library that ground quotes from an LLM review to real PDF coordinates and mark them as standard highlight and note annotations, with a recall pass for missed issues. |
| [guarddiff](https://github.com/LeeGyeongPil/guarddiff) | tool | A CLI and library that compares guardrail variants on identical prompts and reports attack success, over-blocking, latency and cost, separating guard blocks from model refusals. |
| [handoffmap](https://github.com/LeeGyeongPil/handoffmap) | tool | A CLI that folds OpenTelemetry GenAI or OpenInference agent traces into a Mermaid flow and a per-agent table showing handoffs, agents-as-tools and parallel runs. |
| [promptplan](https://github.com/LeeGyeongPil/promptplan) | tool | A CLI that diffs a folder of prompt files against Langfuse (plan) and applies only real changes as new versions or label moves (apply), built for PR review and CI. |
| [cache-autopsy](https://github.com/LeeGyeongPil/cache-autopsy) | tool | Offline CLI that shows prompt cache hit rate, missed tokens and cost, and the likely cause of each miss from stored Anthropic and OpenAI request logs. |
| [llm-batchkit](https://github.com/LeeGyeongPil/llm-batchkit) | tool | A CLI and library that lints Batch API input files, splits them to fit limits, submits shards, merges scattered output and error files per request, and builds a retry file for failures only. A keyless mock server demo is included. |
| [toolcall-conformance](https://github.com/LeeGyeongPil/toolcall-conformance) | tool | A CLI that checks whether OpenAI-compatible servers follow the tool-call protocol, with 11 checks, JSONL evidence and a built-in mock server. |
| [ollama-carry](https://github.com/LeeGyeongPil/ollama-carry) | tool | A Dart CLI that carries chosen Ollama models to an offline PC: bundles manifests and blobs, splits into FAT32-sized parts, and checks every blob with SHA-256 before installing. |
| [ollama-ctxguard](https://github.com/LeeGyeongPil/ollama-ctxguard) | tool | A local proxy that applies per-model num_ctx to Ollama's OpenAI-compatible /v1 path and reports whether the prompt was silently truncated on each response. |
| [mcp-schema-shim](https://github.com/LeeGyeongPil/mcp-schema-shim) | tool | Checks MCP tool input schemas against Gemini, OpenAI strict and Anthropic strict function-calling rules, rewrites them to fit, and restores returned arguments to the original schema shape. |
| [embed-ab](https://github.com/LeeGyeongPil/embed-ab) | tool | A CLI that A/B-tests two embedding models on your own data with recall, nDCG, MRR, confidence intervals and top-k overlap, so you can decide on a model swap or re-index with numbers. |
| [parseoff](https://github.com/LeeGyeongPil/parseoff) | tool | A CLI that runs every installed PDF parser on your own documents, shows results next to page images, and reports ground-truth-free metrics plus license and size warnings. |
| [pgvector-doctor](https://github.com/LeeGyeongPil/pgvector-doctor) | tool | Measures pgvector HNSW recall against exact search per filter value for your own query and recommends the cheapest ef_search and iterative_scan setting. |
| [spinstop](https://github.com/LeeGyeongPil/spinstop) | library | A TypeScript library and replay CLI that detects repeated, near-repeated and cyclic agent tool calls and blocks them before the tool runs. |
| [imeplay](https://github.com/LeeGyeongPil/imeplay) | library | A Playwright library and CLI that reproduces Hangul IME composition so chat inputs can be regression-tested for double-submit and duplicated last character bugs. |
| [known-secret-guard](https://github.com/LeeGyeongPil/known-secret-guard) | library | Library, CLI and PreToolUse hook that catch known secrets leaving an agent in encoded or split form by matching a precomputed variant set. |
| [ko-speechlevel](https://github.com/LeeGyeongPil/ko-speechlevel) | library | A rule-based checker that finds Korean sentences whose speech level slips (e.g. polite to casual) with exact offsets. Ships as library, CLI, streaming checker, promptfoo assertion and vitest matcher; no runtime dependencies. |
| [korean-asr-eval](https://github.com/LeeGyeongPil/korean-asr-eval) | library | Score Korean ASR output with named, fingerprinted normalization profiles; reproducible CER/WER and model comparison across scoring rules. |
| [llm-format-guard](https://github.com/LeeGyeongPil/llm-format-guard) | library | Dependency-free Python library that extracts format and length instructions from a chat, re-injects them, measures answers deterministically and repairs only when it strictly reduces violations. |
| [ko-pii-roundtrip](https://github.com/LeeGyeongPil/ko-pii-roundtrip) | library | TypeScript library that swaps Korean personal data for reversible placeholders before LLM calls and restores originals (with particle correction) even in chunked streaming responses. |
| [langlock](https://github.com/LeeGyeongPil/langlock) | library | Keeps local LLM output in the intended script (e.g. no stray Han/Kana in Korean answers) by masking logits with a stateful, byte-level-BPE-aware mask. Hugging Face and llama-cpp-python adapters, logit_bias/GBNF/regex export, and a CLI. |
| [mcp-apps-host-dart](https://github.com/LeeGyeongPil/mcp-apps-host-dart) | library | Host-side library to render MCP Apps ui:// views in Dart and Flutter apps: handshake, tool-call permission policy, default CSP and a WebView message bridge. |
| [hangul-readout](https://github.com/LeeGyeongPil/hangul-readout) | library | A zero-dependency TypeScript library and CLI that rewrites Korean text the way people read it aloud before TTS, and chunks LLM token streams into sentences without splitting numbers. |
| [tts-pace](https://github.com/LeeGyeongPil/tts-pace) | library | A Python library and CLI that measures speaking rate and fits TTS output to a target pace with a speed knob and bounded pitch-preserving tempo change. |
| [whisper-scrub](https://github.com/LeeGyeongPil/whisper-scrub) | library | Library and CLI that detects and removes Whisper hallucinations using signal-based rules and checks transcript quality without ground truth. |
| [hangul-search-tokenizer](https://github.com/LeeGyeongPil/hangul-search-tokenizer) | library | A zero-dependency synchronous Korean tokenizer that strips josa and eomi for better keyword search, with adapters and a recall/precision/index-size benchmark. |
| [hwpdown](https://github.com/LeeGyeongPil/hwpdown) | library | Pure-Python library and CLI that parses public HWP 5.0 and HWPX specs into Markdown for LLM/RAG, keeping merged tables, footnotes and numbering. |
| [graphtrail](https://github.com/LeeGyeongPil/graphtrail) | plugin | A CLI and read-only VS Code extension that reads LangGraph SqliteSaver databases without executing any code, rebuilds the run timeline, diffs states and exports reports. |
| [ai-lab-agent-loop-mcp](https://github.com/LeeGyeongPil/ai-lab-agent-loop-mcp) | demo | A demo and beginner guide that shows an AI agent loop live: each thought, MCP tool call and observation on a timeline. Runs with a mock model or local Ollama. |
| [ai-lab-lora-finetune](https://github.com/LeeGyeongPil/ai-lab-lora-finetune) | demo | Teach a 0.5B model a speaking style with 100 examples via LoRA and inspect an HTML report of loss and before/after answers. |
| [ai-lab-llm-eval-gate](https://github.com/LeeGyeongPil/ai-lab-llm-eval-gate) | demo | A dependency-free tool that scores prompt changes on a small test set and fails CI when scores drop below a floor or beyond the noise range. Runs offline by replaying recorded answers. |
| [ai-lab-llm-gateway](https://github.com/LeeGyeongPil/ai-lab-llm-gateway) | demo | Call several LLM providers through one interface, swap models by config, and try retry, fallback and routing. Compare tokens, estimated cost and latency per call. Mock mode needs no API key. |
| [ai-lab-local-llm-bench](https://github.com/LeeGyeongPil/ai-lab-local-llm-bench) | demo | Benchmark a local Ollama server with one command and see how input length and concurrency affect TTFT, tokens/s and memory. A keyless mock mode replays recorded timings. Quantization comparison and charts come in later milestones. |
| [ai-lab-rag-rerank](https://github.com/LeeGyeongPil/ai-lab-rag-rerank) | demo | A local demo that puts first-stage retrieval next to cross-encoder reranking, showing rank moves, evidence highlights, score distribution and a scoreboard. |
