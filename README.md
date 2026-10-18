# 박희철

Cloud Infrastructure Engineer

**[포트폴리오](https://cloud-infra-portfolio.vercel.app/)** · [포트폴리오 소스](https://github.com/wkfkeha784-pixel/cloud-infra-portfolio) · [이메일](mailto:wkfkeha784@gmail.com)

## 인프라 프로젝트

### Durian · Kafka/KEDA 구성과 장애 분석

- **개인 담당:** **Kafka/KEDA 구성·관측, 모니터링 인수·재구성**.
- Terraform 구성 변경·Drift 분석과 worker-03 재가입 검증에 참여했습니다.

팀 결과: 8/10 부하 시험에서 Consumer 1→4→1, HTTP 300/300 응답. HTTP 응답은 비동기 요청 수락 기준이며, worker-03 복구는 단일 VM 팀 시험입니다.

[문제 해결·담당 역할 →](https://cloud-infra-portfolio.vercel.app/projects/durian)

### Bluebell · AWS Web–WAS 구축과 통합 검증

- **개인 담당:** 팀장으로 **AWS Web–WAS와 LB를 연결**하고 서비스·Target Group·API 응답을 통합 검증했습니다.

팀 결과: EventBridge 규칙을 비활성화한 통제 복구 시험에서 인스턴스 교체 후 서비스·Target Group·HTTP 응답을 확인했습니다.

[서비스 구성·복구 기록 →](https://cloud-infra-portfolio.vercel.app/projects/bluebell)

## 서비스 구현

### OneReport · Backend 공동 구현

**개인 담당:** Backend 2명 중 한 명으로 도메인·DB·Timeline API/SSE와 규칙 기반 분석·라우팅을 공동 구현했습니다.  
**팀 결과:** 2026-08-21 AWS PoC 환경에서 배포 정상화 후 Smoke Test PASS.

[구현 기능·API 계약 →](https://cloud-infra-portfolio.vercel.app/projects/onereport)

### Labbit · Frontend 세션·파일 충돌 처리

**개인 담당:** Frontend/Design. 세션 종료 후 재연결, 파일 동시 수정 충돌, LabSpec 권한·오류·빈 상태와 Mapping 선택 UI를 구현했습니다.  
**2026-10-16 기준:** 본인 PR 병합. Frontend 코드·API 계약·PR 검사와 실제 Auth/Class Backend 연동 기록입니다.

[구현 과정 →](https://cloud-infra-portfolio.vercel.app/projects/labbit) · [팀 저장소](https://github.com/ktcloud4-SL/labbit-app)  
개인 PR: [#62 세션·파일](https://github.com/ktcloud4-SL/labbit-app/pull/62) · [#93 권한·오류](https://github.com/ktcloud4-SL/labbit-app/pull/93) · [#98 빈 상태](https://github.com/ktcloud4-SL/labbit-app/pull/98) · [#97 Mapping](https://github.com/ktcloud4-SL/labbit-app/pull/97)

## 사용 기술

- **인프라·구성:** AWS, OpenStack, Linux, Nginx, Kubernetes, Terraform
- **메시징·관측:** Kafka, Redis, KEDA, Prometheus, Grafana
- **서비스 연동:** Backend 도메인·API, Frontend HTTP·WebSocket 소비자와 오류 처리

## 경력·교육

- 육군 정보통신 장교: 통신 운용계획·장비 점검·인원과 현장 조율
- KT Cloud Infrastructure Bootcamp · 2026.05.12–2026.12.03
- AWS SAA-C03 준비
