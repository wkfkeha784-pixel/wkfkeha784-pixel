# 개인 GitHub 공개 프로필 · 2026-11-02 종합 정리

## 작업 목표

취업용 공개 GitHub 프로필 첫 화면에서 신입 클라우드 인프라 엔지니어의 서비스 프로젝트, 역할, 검증 경험과 포트폴리오 진입 경로가 바로 보이도록 정리한다. 기존 취업·재정·학습 비공개 데이터와 협업 팀 저장소를 공개하거나 수정하지 않는다.

## 실제 접근 가능한 저장소와 공개 범위

| 사용자 소유 저장소 | 현재 GitHub visibility | 이번 작업 |
|---|---|---|
| `wkfkeha784-pixel/wkfkeha784-pixel` | public | 프로필 첫 화면 README 최신화 |
| `wkfkeha784-pixel/cloud-infra-portfolio` | public | 저장소 README의 프로젝트 설명 및 링크 정합성 최신화 |
| 개인 비공개 학습·재정·취업 기록 저장소 (합계 3개) | private | 현재 공개 범위와 원본 그대로 유지, 이번 작업에서 변경 안 함 |

두 공개 저장소 밖의 팀 공동 저장소 `ktcloud4-SL/labbit-app`은 읽기 근거·공개 링크만 사용했으며 커밋하지 않았다. 개인의 경력·지원서 PDF나 제출 원본을 공개 저장소에 올리지 않았다.

## 첫 화면 리디자인 내용

1. 기술명 나열형으로 시작하던 소개를 '인프라 구성·요청 경로·장애 대응 및 복구 검증' 중심 문장으로 정리.
2. 대표 프로젝트를 **Durian 수강신청 대기열 서비스**, **Bluebell 복구·모니터링 Web API 운영환경**으로 소개하고, 본인의 참여와 확인 가능한 팀 시험 결과를 한 단락에 자연스럽게 연결.
3. **OneReport 다기관 공동대응 PoC**는 Backend 공동 구현으로, **Labbit 가상 실습 플랫폼**은 FE·API/WSS 검증 및 DR 사전검토로 설명. Labbit의 낡은 `2026-10-16 기준` 표기 제거.
4. 웹 포트폴리오를 가장 눈에 띄는 단일 주요 진입점으로 연결하고, 프로필 코드 저장소·이메일을 옆에 배치.
5. 사용 기술·군 정보통신 장교·육군사관학교·진행 중 KT Cloud 교육 및 실제 보유 자격/어학을 간결하게 추가. AWS SAA 등 **취득하지 않은 준비 중 자격은 보유 자격으로 기재하지 않음**.
6. 타임스탬프·PR 나열·같은 단서의 반복·가독성 낮은 주석·장식용 통계 배지를 의도적으로 사용하지 않음. GitHub 기본 Markdown의 제목·볼드·짧은 문단·링크를 활용.

## 정합성 근거

- 웹 포트폴리오 4개 서비스: https://cloud-infra-portfolio.vercel.app/
- 웹 기준 코드: `wkfkeha784-pixel/cloud-infra-portfolio` PR #37 병합 이후 `main`.
- 최신 프로젝트 소개 기준: 웹 `src/data/projects.ts`와 각 프로젝트 상세 페이지, [취업 포트폴리오 작성 정책](https://github.com/wkfkeha784-pixel/cloud-infra-portfolio/blob/main/docs/PORTFOLIO_STORY_POLICY_20261023.md).
- Durian HTTP 300/300은 '비동기 요청 수락'으로 한정, Consumer 1→4→1 팀 시험을 개인 단독 성과로 쓰지 않음. worker-03는 단일 VM 복구 검증 참여.
- Bluebell 5인 팀장·Web/WAS·Target Group/HTTP 검증만 개인 담당을 강조, 팀 운영/자동화 성과는 자연스럽게 공동 결과로 연결.
- OneReport AWS PoC·Backend 공동 구현 구분, Labbit 실제 DR Failover/Failback 및 RTO/RPO 실측은 완료로 쓰지 않음.
- 군 경력은 군 정보통신 직무로 표기, 민간 클라우드 상용 운영 경력으로 치환하지 않음.

## 검증·범위 제한

- GitHub 연결 계정으로 현재 `README.md` 및 `docs/README.md` 파일과 각 저장소 visibility를 확인하고 해당 파일의 최신 SHA를 기준으로 수정·커밋. 커밋 후 파일 원문 재조회와 상대 링크·외부 주소 문자열 검사를 수행.
- GitHub 웹 사이트의 **실제 로그아웃 렌더, 고정(Pinned) 저장소 배치, 사용자 Bio·Website·저장소 About 설명 설정은 현 연결 API에서 현재값을 읽거나 변경할 수 없음**. 기존 2026-10-11 관리 기록에 당시 고정 순서는 포트폴리오 → 팀 Labbit이라고 기록돼 있으나, 이를 2026-11-02 현재 실측값으로 주장하지 않는다.
- README 콘텐츠 변경과 별개로 웹 포트폴리오 애플리케이션 구현 소스, PDF/PPTX v0.29, 배포 환경 설정은 변경하지 않음. **포트폴리오 README 문서 커밋 `157acd32919265c14404b9755e7d9c55e94e6934`로 새 Vercel Production `dpl_HreniFLJm4nL58LeAnssGUB5ZDcg`가 생성돼 READY** 및 운영 alias `cloud-infra-portfolio.vercel.app`, Git SHA 일치를 API에서 확인. README-only 커밋의 `fetch_commit_workflow_runs` 목록이 비어 있었으므로 해당 커밋에 별도 PR CI가 성공했다고 주장하지 않음. 이전 웹 기능/반응형 Playwright 72/72 PASS는 코드 변경 직전 PR #37의 검증 이력으로 유지.

## GitHub 사이트에서 수동으로 확인할 항목

- 프로필 `Edit profile`의 Bio는 '신입 클라우드 인프라 엔지니어 | AWS · OpenStack · Kubernetes · Linux · 운영·복구 검증', Website는 https://cloud-infra-portfolio.vercel.app/ 추천. 실제 UI 설정 완료 여부는 미검증.
- 프로필 `Customize your pins`에서 **개인 `cloud-infra-portfolio`를 첫 순서**, 팀 `ktcloud4-SL/labbit-app`을 보조 증빙으로 두는 구성이 적절하다. GitHub의 실제 Pinned 설정을 바꿨다고 기록하지 않는다.
- 공개 포트폴리오 저장소 About 설명은 'AWS·OpenStack·Kubernetes 팀 프로젝트의 인프라 구성·장애 분석·복구 검증 포트폴리오', Website는 운영 URL이 적합하다. 변경 전후 저장소 About 값은 별도 수동 확인 필요.

## 유지관리

앞으로는 프로젝트의 실제 신규 검증, 보유 자격·어학 갱신, 교육 상태 변경 등 **사실이 바뀔 때만** 프로필 README와 웹 상세 및 취업용 제출 파일을 각각 검토한다. 기존 채용 제출본은 사후 수정으로 자동 변경되지 않는다.
