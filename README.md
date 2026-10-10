# 박희철 | Cloud Infrastructure Engineer

> 구축에서 끝내지 않고, 운영 상태를 관측하고 장애 이후 정상화까지 검증합니다.

KT Cloud 교육·팀 프로젝트에서 AWS·OpenStack·Kubernetes 환경의 서비스를 구성하고, 부하와 장애 상황에서 어떻게 동작하는지 확인해 왔습니다. 구축한 환경의 상태를 관측하고, 문제가 생겼을 때 원인을 찾아 복구하는 일에 관심이 있습니다.

육군 정보통신 장교로 근무하며 장비와 인원, 운영 절차를 관리했습니다. 지금은 이 경험을 바탕으로 클라우드 인프라 엔지니어 취업을 준비하고 있습니다.

**[포트폴리오](https://cloud-infra-portfolio.vercel.app/)** · [포트폴리오 소스](https://github.com/wkfkeha784-pixel/cloud-infra-portfolio) · [이메일](mailto:wkfkeha784@gmail.com)

## 주요 경험

- **AWS 서비스 구성·복구:** Web–WAS 연결, 인스턴스 교체 후 서비스 정상화 확인
- **Kubernetes 운영:** Redis·Kafka 운영, Kafka Lag에 따른 KEDA 확장·축소
- **인프라 관리·관측:** Terraform으로 worker-03 재생성·재가입 검증, 실행 상태와 설정·모니터링 비교
- **서비스 연동:** Backend 도메인·API 구현, Frontend HTTP·WebSocket 연동과 오류 처리

## 프로젝트

### Team Durian · Kubernetes 운영과 부하 대응

수강신청 폭주에 대응하는 대기열 플랫폼에서 Kubernetes·Redis·Kafka·KEDA 운영, 모니터링 인수·재구성과 worker-03 복구 검증을 맡았습니다.

- 외부 HTTP 요청 **300/300 수락**과 Consumer **1→4→1** 확장·축소를 확인했습니다.
- Terraform으로 단일 노드 worker-03을 재생성하고 클러스터에 재가입시켰습니다. 최종 상태는 `Ready,SchedulingDisabled`입니다.
- HTTP 200은 비동기 요청을 수락했다는 뜻입니다. DB에 300건이 모두 저장됐다는 결과는 아닙니다.

`OpenStack` `Kubernetes` `Kafka` `Redis` `KEDA` `Prometheus` `Grafana`

[담당 역할과 검증 결과 →](https://cloud-infra-portfolio.vercel.app/projects/durian)

### Bluebell · AWS 서비스 통합과 복구

AWS Web/WAS와 로컬 DB를 연결한 하이브리드 3-Tier 프로젝트입니다. 팀장을 맡아 Web–WAS 구축과 AWS·복구 흐름의 통합 검증을 담당했습니다.

- ASG가 인스턴스를 교체한 뒤 서비스·Target Group·HTTP 응답이 정상화되는지 확인했습니다.
- 팀의 최종 E2E는 EventBridge 규칙 2개를 비활성화한 통제 실행입니다. EventBridge → SSM 자동 실행 설계와 구분해 기록했습니다.

`AWS` `Nginx` `Flask` `Docker Swarm` `Ansible` `Prometheus` `Grafana`

[서비스 구성과 복구 검증 →](https://cloud-infra-portfolio.vercel.app/projects/bluebell)

### OneReport · Backend 도메인과 API

복합사고에 여러 기관이 공동 대응하는 플랫폼입니다. Backend의 도메인·DB, 라우팅, API 계약과 규칙 기반 분석을 구현했습니다.

- 개인 구현·검증 근거는 PR #9/#14/#27/#30에 정리했습니다.
- 팀은 PR #30 당시 health 502 문제를 배포 정상화 후 해결했고, 최종 운영 Smoke Test에서 **PASS**를 확인했습니다.
- 팀 저장소는 비공개이며, 상세 페이지에서 공개 가능한 검증 자료를 제공합니다.

[구현 범위와 운영 검증 →](https://cloud-infra-portfolio.vercel.app/projects/onereport)

### Labbit · Frontend 연동과 Workspace

OpenStack 기반 실습 환경 플랫폼입니다. Frontend·디자인을 맡아 HTTP·WebSocket 연동, 인증·권한·오류 화면과 테스트·CI를 작업했습니다.

**진행 중 · 2026-10-10 기준**

- Terminal·파일 기능을 구현한 **PR #62**가 2026-10-07 팀 `main`에 병합됐습니다.
- 코드·CI에서 Terminal 세션과 재연결, 파일 편집 보호와 HTTP 412 충돌 처리를 검증했습니다.
- Auth/Class 흐름은 실제 Backend와 브라우저로 확인했습니다.
- 실제 OpenStack VM의 PTY/SFTP 연동은 후속 통합 검증 범위입니다. 관련 작업은 LBT-21/LBT-22입니다.

[상세 →](https://cloud-infra-portfolio.vercel.app/projects/labbit) · [팀 저장소](https://github.com/ktcloud4-SL/labbit-app) · [PR #62 — Terminal·파일 연동](https://github.com/ktcloud4-SL/labbit-app/pull/62) · [PR #59 — Workspace 진입 검증](https://github.com/ktcloud4-SL/labbit-app/pull/59)

## 학습 중

- **KT Cloud Infrastructure Bootcamp** · 2026.05.12–2026.12.03
- **AWS SAA-C03** 준비
- **GCP Cloud Operations 개인 프로젝트** · 설계·환경 준비

## 연락처

[cloud-infra-portfolio.vercel.app](https://cloud-infra-portfolio.vercel.app/) · [wkfkeha784@gmail.com](mailto:wkfkeha784@gmail.com)
