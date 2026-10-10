# 박희철 | Cloud Infrastructure Engineer

> 구축에서 끝내지 않고, 운영 상태를 관측하고 장애 이후 정상화까지 검증합니다.

AWS·OpenStack·Kubernetes 환경에서 서비스 경로를 구성하고, 부하·장애·Drift·권한/오류 상황을 근거로 확인하며 정상 상태로 수렴시키는 프로젝트 경험을 쌓고 있습니다.  
육군 정보통신 장교로 쌓은 조직·절차 기반 운영 경험을 Cloud Infrastructure 역량으로 확장하고 있습니다.

**[Web Portfolio](https://cloud-infra-portfolio.vercel.app/)** · [Portfolio Repository](https://github.com/wkfkeha784-pixel/cloud-infra-portfolio) · [Email](mailto:wkfkeha784@gmail.com)

## Core Focus

- **Infrastructure Integration & Recovery** — AWS 3-Tier 서비스 통합 · 장애 이후 정상화 검증
- **Kubernetes Operations** — Kafka Lag 기반 KEDA 확장·축소 · Redis/Kafka 운영
- **IaC & Observability** — Terraform Drift 복구 · Runtime과 Manifest·Monitoring 정합
- **Contract-driven Integration** — Backend Domain/API · Frontend HTTP/WebSocket Consumer

## Selected Projects

### Team Durian · Kubernetes 운영과 부하 대응

수강신청 폭주 대응 대기열 오토스케일링 플랫폼

**담당** — Kubernetes · Redis/Kafka/KEDA 운영 · Monitoring · Terraform

- **개인 검증:** 외부 HTTP 요청 **300/300 수락** · Consumer **1→4→1** 확장·축소
- **복구 경험:** Terraform으로 worker-03 Drift 복구 · 노드 재생성·클러스터 재가입
- **검증 조건:** HTTP 200은 비동기 요청 수락 기준이며, DB 300건 전체 Commit 완료를 의미하지 않습니다.

`OpenStack` `Kubernetes` `Kafka` `Redis` `KEDA` `Prometheus` `Grafana`

[역할·운영 흐름·검증 근거 보기 →](https://cloud-infra-portfolio.vercel.app/projects/durian)

### Bluebell · AWS 서비스 통합과 복구

AWS Web/WAS + Local DB 하이브리드 3-Tier 인프라

**담당** — Team Lead · Web–WAS 구축 · AWS/Recovery 통합 검증

- **개인 검증:** ASG Replacement 이후 서비스·Target Group·HTTP 응답 정상화 확인
- **팀 검증 조건:** 최종 E2E는 EventBridge Rule 2개를 DISABLED로 유지한 통제 실행입니다. EventBridge → SSM Trigger 설계와 구분합니다.

`AWS` `Nginx` `Flask` `Docker Swarm` `Ansible` `Prometheus` `Grafana`

[서비스 경로·Replacement 복구 근거 보기 →](https://cloud-infra-portfolio.vercel.app/projects/bluebell)

### OneReport · Backend 도메인과 API 계약

복합사고 다기관 공동대응 운영 플랫폼

**담당** — Backend · Domain/DB · Routing · Contract · Rule Classification

- **개인 기여:** PR #9/#14/#27/#30 기반 Backend 구현·검증
- **팀 결과:** PR #30 시점 health 502 이후 배포 정상화 · 최종 운영 Smoke **FINAL: PASS**
- Rule-based Analysis를 구현했습니다. 비공개 팀 저장소의 Repository/PR 직접 링크는 공개하지 않습니다.

[도메인·개인 기여·운영 검증 보기 →](https://cloud-infra-portfolio.vercel.app/projects/onereport)

### Labbit · Frontend 계약 구현과 Workspace 통합

OpenStack 기반 Virtual Lab Platform · **IN PROGRESS · 2026-10-10 기준**

**담당** — Frontend/Design · HTTP/WebSocket Consumer · Auth/Permission/Error UX · Test/CI

- **개인 기여:** Terminal·File Consumer **PR #62 main 병합** · 2026-10-07
- **코드·CI 검증:** Terminal 세션·재연결 · File 412 충돌 보호·편집 보호
- **Browser 검증:** Auth/Class 실제 Backend 흐름 확인
- **후속 통합 검증:** 실제 OpenStack VM PTY/SFTP E2E · LBT-21/LBT-22

[Case Study →](https://cloud-infra-portfolio.vercel.app/projects/labbit) · [Repository](https://github.com/ktcloud4-SL/labbit-app) · [PR #62 — Terminal·File 통합](https://github.com/ktcloud4-SL/labbit-app/pull/62) · [PR #59 — Workspace 진입 회귀 검증](https://github.com/ktcloud4-SL/labbit-app/pull/59)

## Current Focus

- **KT Cloud Infrastructure Bootcamp** · 2026.05.12–2026.12.03
- **AWS SAA-C03** 준비 중
- **GCP Cloud Operations 개인 프로젝트** · 설계·환경 준비 중

## Contact

[cloud-infra-portfolio.vercel.app](https://cloud-infra-portfolio.vercel.app/) · [wkfkeha784@gmail.com](mailto:wkfkeha784@gmail.com)

---

**Build → Observe → Troubleshoot → Recover → Verify**
