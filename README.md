# 박희철

**Cloud Infrastructure Engineer · 클라우드 인프라 엔지니어**

AWS·OpenStack·Kubernetes 기반 팀 프로젝트에서 인프라를 구성하고 서비스 요청 경로와 장애 대응·복구 과정을 검증했습니다. Linux·네트워크·자동화와 모니터링 경험을 바탕으로 클라우드 인프라 엔지니어 직무를 준비하고 있습니다.

**[웹 포트폴리오 보기](https://cloud-infra-portfolio.vercel.app/)** · [포트폴리오 소스](https://github.com/wkfkeha784-pixel/cloud-infra-portfolio) · [이메일](mailto:wkfkeha784@gmail.com)

## 대표 인프라 프로젝트

### 01 · [Durian — 수강신청 폭주 대응 대기열 서비스](https://cloud-infra-portfolio.vercel.app/projects/durian)

**OpenStack · Kubernetes · Redis/Kafka · KEDA · Prometheus/Grafana**

- 대기열·비동기 처리·자동 확장을 연결한 수강신청 서비스에서 Kafka/KEDA 운영, 모니터링 인수·재구성, 장애 분석과 Worker 복구 검증에 참여했습니다.
- Kafka 연결 문제를 NetworkPolicy → TLS 신뢰 → SCRAM 인증 → ACL 권한으로 나누어 점검했습니다. 팀 부하 시험에서 **HTTP 300/300 비동기 요청 수락, Consumer 1→4→1 확장·축소**를 확인했습니다.

**[아키텍처와 장애 분석 과정 보기](https://cloud-infra-portfolio.vercel.app/projects/durian)**

### 02 · [Bluebell — 장애 복구·모니터링 웹 API 운영환경](https://cloud-infra-portfolio.vercel.app/projects/bluebell)

**AWS · Nginx/Flask · Docker Swarm · Ansible · Prometheus/Grafana**

- **5인 팀의 팀장**으로 AWS Web/WAS와 로드밸런서를 연결하고, 요청 경로·배포 상태·복구 후 서비스 응답을 통합 검증했습니다.
- 통제된 인스턴스 교체 시험에서 **Target Group 정상 상태와 HTTP/API 응답**, 모니터링 대상 재편입을 함께 확인했습니다.

**[구축과 복구 검증 과정 보기](https://cloud-infra-portfolio.vercel.app/projects/bluebell)**

## 서비스 구현·연동 프로젝트

### [OneReport — 복합사고 다기관 공동대응 플랫폼 PoC](https://cloud-infra-portfolio.vercel.app/projects/onereport)

해커톤 팀에서 **Backend를 공동 구현**했습니다. Report/Incident 데이터 모델과 기관 배정, Timeline REST/SSE API를 연결하고 AWS PoC의 Smoke Test에 참여했습니다.

### [Labbit — 클라우드 가상 실습실 플랫폼](https://cloud-infra-portfolio.vercel.app/projects/labbit)

**Frontend/UI·UX, API/WSS 연동 및 브라우저 검증**을 담당했습니다. 인증·권한, Terminal/File/Live, 파일 충돌과 오류 상태를 점검했으며, 서울–오사카 DR의 전환·복구 절차와 중단 조건을 사전검토하고 있습니다.

[플랫폼 구현 과정](https://cloud-infra-portfolio.vercel.app/projects/labbit) · [팀 공개 저장소](https://github.com/ktcloud4-SL/labbit-app)

## 기술과 운영 경험

| 영역 | 사용·검증 경험 |
|---|---|
| 클라우드·인프라 | AWS, OpenStack, Linux, 네트워크, Nginx, Kubernetes |
| 배포·자동화 | Docker Swarm, Ansible, Terraform, GitHub Actions |
| 메시징·관측 | Redis, Kafka, KEDA, Prometheus, Grafana |
| 서비스·API 연동 | Flask API(Bluebell), FastAPI·REST/SSE(OneReport), React·TypeScript·WebSocket(Labbit) |

## 경력·교육

- **육군 정보통신 병과 장교** (2020.03–2025.09) — 통신 운용계획, 장비 점검, 현장·인원 조율, 재난 대비 업무
- **육군사관학교** — 전자공학·군사학 전공, 2020년 졸업
- **KT Cloud Infrastructure Bootcamp** (2026.05–2026.12 예정) — AWS·OpenStack·Kubernetes 기반 인프라 교육 및 팀 프로젝트
- **보유 자격·어학** — 컴퓨터활용능력 2급, G-TELP Level 2(84점)

