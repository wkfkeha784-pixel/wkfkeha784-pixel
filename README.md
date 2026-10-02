# 박희철 | Cloud Infrastructure Engineer

> 구축에서 끝내지 않고, 운영 상태를 관측하고 장애 이후 정상화까지 검증합니다.

AWS·OpenStack·Kubernetes 환경에서 서비스 경로를 구성하고, 부하·장애·Drift·권한/오류 상황을 실제 Evidence로 확인해 정상 상태로 수렴시키는 프로젝트 경험을 쌓고 있습니다.  
육군 정보통신 장교로 쌓은 조직·절차 기반 운영 경험을 Cloud Infrastructure 역량으로 확장하고 있습니다.

[Web Portfolio](https://cloud-infra-portfolio.vercel.app/) · [Email](mailto:wkfkeha784@gmail.com)

## Core Focus

- **Infrastructure Integration & Recovery** — AWS 3-Tier 통합 · ASG Replacement 이후 서비스 정상화 검증
- **Kubernetes Operations** — 외부 HTTP 부하 · Kafka Lag 기반 KEDA Consumer 1→4→1 검증
- **IaC · Observability · Reproducibility** — Terraform Drift 복구 · Git/Manifest/Monitoring과 Runtime 정합
- **Contract-driven Application Integration** — Backend Domain/API · Frontend HTTP/WS Contract Consumer

## Selected Projects

### Team Durian
수강신청 폭주 대응 대기열 오토스케일링 플랫폼  
**Kubernetes · Redis/Kafka/KEDA 운영 · Monitoring · Terraform**

`[MY]` 외부 HTTP 300/300 → Consumer 1→4→1 · Terraform worker-03 Drift Recovery

`OpenStack` `Kubernetes` `Kafka` `Redis` `KEDA` `Prometheus` `Grafana`  
[Case Study](https://cloud-infra-portfolio.vercel.app/projects/durian)

### Bluebell
AWS Web/WAS + Local DB 하이브리드 3-Tier 인프라  
**Team Lead · Web–WAS Traffic Flow · AWS/Recovery 통합 검증**

`[MY]` ASG Replacement E2E · `[BOUNDARY]` Recovery Design ≠ Final Trigger Test

`AWS` `Nginx` `Flask` `Docker Swarm` `Ansible` `Prometheus` `Grafana`  
[Case Study](https://cloud-infra-portfolio.vercel.app/projects/bluebell)

### OneReport
복합사고 다기관 공동대응 운영 플랫폼  
**Backend — Domain / DB / Routing / Contract / Rule Classification**

[Repository](https://github.com/ktcloud4-SL/hackathon) · [PR #9 — Core Domain/DB](https://github.com/ktcloud4-SL/hackathon/pull/9) · [PR #27 — Rule-based Analysis](https://github.com/ktcloud4-SL/hackathon/pull/27)

### Labbit
OpenStack 기반 Virtual Lab Platform — **IN PROGRESS · 2026-10-03**  
**Frontend / Design · HTTP/WS Contract Consumer · Auth/Permission/Error UX · Test/CI**

`[MY]` Auth/Class 실제 Backend Browser Flow · `[DRAFT]` Terminal/File Consumer — actual VM PTY/SFTP E2E Pending

[Repository](https://github.com/ktcloud4-SL/labbit-app) · [PR #59 — Current Frontend Baseline](https://github.com/ktcloud4-SL/labbit-app/pull/59)

## Current Focus

- **KT Cloud Infrastructure Bootcamp** · 2026.05.12–2026.12.03
- **AWS SAA-C03** 준비 중
- **GCP Cloud Operations 개인 프로젝트** · 설계·환경 준비 중

## Contact

- Web: [cloud-infra-portfolio.vercel.app](https://cloud-infra-portfolio.vercel.app/)
- Email: [wkfkeha784@gmail.com](mailto:wkfkeha784@gmail.com)

---

**Build → Observe → Troubleshoot → Recover → Verify**
