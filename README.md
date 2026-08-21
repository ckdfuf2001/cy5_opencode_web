# cy5-webui

[threehymns/opencode-webui](https://github.com/threehymns/opencode-webui) 클론에 아래 기능을 추가한 포크입니다.

## 데모

<video src="chunks/demo_chunk_01.mp4" controls muted loop playsinline width="100%"></video>

## 원본 대비 추가된 기능

- **파일 탐색기 & 문서 뷰어** — 트리 탐색·업로드는 물론, PDF/DOCX/XLSX/PPTX/MSG 파일을 브라우저에서 바로 미리봅니다. DRM 문서는 로컬 MS Office COM 변환으로 처리하고, 텍스트 추출·제자리 편집 API를 제공합니다.
- **스케줄러** — cron 기반으로 커맨드/프롬프트를 예약 실행합니다. 달력 뷰에서 예약·실행 이력을 한눈에 보고, 즉시 실행·활성 기간·담당 에이전트 지정이 가능합니다.
- **백엔드 분리** — Bun+Hono 백엔드가 OpenCode 서버의 생명주기를 관리하고 REST/SSE를 프록시합니다. 단일 exe 포터블 패키징이 가능합니다.
- **커맨드 관리** — 슬래시 커맨드/스킬/툴/에이전트를 UI에서 등록·편집하고, 실행 히스토리와 프로젝트/전역 스코프를 관리합니다.