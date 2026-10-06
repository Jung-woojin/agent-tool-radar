# AI Tool Radar 자동화 운영 — 2026-10-06

AI Tool Radar는 매일 한국시간 08:10에 최근 24~72시간의 도구 변화를 조사한다. 10~15개 후보를 검토하고 근거가 충분한 5~10개를 선정한다. 공식 repo·docs·release·코드·권한 모델·issue/PR을 교차 확인하며, 확인되지 않은 정보는 추측하지 않는다.

도구별 필수 25개 항목과 보고서 형식은 [원본 AI Tool Radar 지침](https://github.com/Jung-woojin/cv-research-radar/blob/main/docs/requirements/ai-tool-radar.md)을 따른다. 마지막에는 설치/시험 Top 3, CV 연구 workflow 적합성, 보안 주의 표, 설치를 미뤄도 되는 도구, 측정 가능한 10~30분 테스트를 포함한다. 중요한 새 변화가 없는 도구는 Top 3에 반복하지 않는다.

전체 보고서를 먼저 채팅에 전달한다. 이후 이 저장소에 `[archive] daily: AI tool radar YYYY-MM-DD` Issue를 생성하며, body 첫 줄은 `<!-- path: daily/YYYY/MM/YYYY-MM-DD.md -->`이다. 다음 줄부터 채팅과 동일한 전체 본문을 넣는다. 기존 Actions의 성공, 실제 파일 내용, commit, Issue closed를 확인해야 아카이브 완료로 기록한다.

기존 코드·workflow·settings는 변경하지 않는다. 도구 설치나 계정 권한 추가는 이 조사 자동화에 포함하지 않는다. 저장 실패 시 채팅 보고서와 로컬 초안을 보존하고 정확한 실패 원인을 알린다.

매일 09:30 통합 Health Check가 예약 활성화, 실행 기록, 누락 보고서, Actions 실패, 미처리 Issue를 점검한다. 백필은 당시 날짜까지 공개된 근거만 사용한다. 실행 기록은 로컬 `radar-runtime/runs`에 남긴다. 전체 실행 규칙과 일정은 [통합 운영 문서](https://github.com/Jung-woojin/cv-research-radar/blob/main/docs/automation-system.md)와 [작업 설정](https://github.com/Jung-woojin/cv-research-radar/blob/main/config/radar-jobs.json)을 따른다.

로컬 실행을 위해 컴퓨터와 Codex 앱이 켜져 있어야 하며, 오전 9시 완료는 목표다.
