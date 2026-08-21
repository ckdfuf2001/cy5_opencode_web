# cy5-webui

[threehymns/opencode-webui](https://github.com/threehymns/opencode-webui) 클론에 아래 기능을 추가한 포크입니다. 현재는 배포본만 제공하고 있습니다.


## 원본 대비 추가된 기능
- **자동 커맨드 생성 가이드** — 자동화 커맨드 생성을 위한 Agents.md 가 포함되어 배포됩니다.
- **백엔드 분리** — Bun+Hono 백엔드가 OpenCode 서버의 생명주기를 관리하고 REST/SSE를 프록시합니다. 단일 exe 포터블 패키징이 가능합니다. (opencode.exe 1.18.18 이후 버전 지원, bin/opencode.exe 파일 교체)
- **파일 탐색기 & 문서 뷰어** — 트리 탐색·업로드는 물론, PDF/DOCX/XLSX/PPTX/MSG 파일을 브라우저에서 바로 미리봅니다. DRM 문서는 로컬 MS Office COM 변환으로 처리하고, 텍스트 추출·제자리 편집 API를 제공합니다. (서버 PC의 MS Office 와 com 통신함으로, 서버 PC에 MS Office가 설치되어야 합니다)
- **스케줄러** — cron 기반으로 커맨드/프롬프트를 예약 실행합니다. 달력 뷰에서 예약·실행 이력을 한눈에 보고, 즉시 실행·활성 기간·담당 에이전트 지정이 가능합니다. (별도 sqlite db저장)
- **커맨드 관리** — 슬래시 커맨드/스킬/툴/에이전트를 UI에서 등록·편집하고, 실행 히스토리와 프로젝트/전역 스코프를 관리합니다. (별도 sqlite db저장)

  
## 데모
기본 가이드 - Agents.md 
<img width="960" height="720" alt="1 기본가이드" src="https://github.com/user-attachments/assets/3bddfdb1-3719-4590-8117-53ff126ce9ec" />

커맨드 등록 - 샘플
<img width="960" height="720" alt="2 커맨드등록(1)" src="https://github.com/user-attachments/assets/c2924db9-8ee9-400f-9182-e474564d7fc1" />

퍼미션,커맨드 관리 
<img width="960" height="720" alt="3 퍼미션,커맨드 관리" src="https://github.com/user-attachments/assets/abfb5379-2089-4bb7-b4b6-095e4aba2099" />

커맨드 실행
<img width="960" height="720" alt="4 커맨드실행" src="https://github.com/user-attachments/assets/1ddcb8f5-c9e2-40ab-8504-ffebc6ef4bbc" />

파일브라우저
<img width="960" height="720" alt="5 파일탐색기" src="https://github.com/user-attachments/assets/f7ddd56e-248d-462a-9b07-45f180a6e124" />

스케쥴 관리
<img width="960" height="720" alt="6 스케쥴 관리" src="https://github.com/user-attachments/assets/6dd10c1f-b5a5-4f0a-ac31-e50d96c52441" />


