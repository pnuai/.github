# PNU Slate: 온라인 브로슈어 CMS


[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Docusaurus](https://img.shields.io/badge/Docusaurus-3.10.1-green.svg)](https://docusaurus.io/)
[![React](https://img.shields.io/badge/React-19.0.0-blue.svg)](https://react.dev/)

> **서비스 링크: [https://pnuai.github.io](https://pnuai.github.io)**
>
> 📖 **[사용자 가이드 (운영 매뉴얼) 바로가기](./USER_GUIDE.md)**

PNU Slate는 부산대학교 AI융합교육원의 다양한 교육 프로그램을 체계적으로 관리하고 배포하기 위한 통합 디지털 브로슈어 플랫폼입니다. Docusaurus 기반의 정적 사이트 생성(SSG) 기술과 Git 기반의 무설치형 Web CMS를 결합하여 개발 생산성과 운영 편의성을 동시에 제공합니다.

---

## 핵심 기능

### PNU AI Hub 
PNU AI Hub는 전체 시스템의 메인 게이트웨이 역할을 수행합니다.

통합 접근 지점: 별도의 리포지토리로 관리되는 개별 교육 과정(부트캠프, 대학원, 교원 연수 등) 브로슈어를 한곳에서 탐색하고 접근할 수 있는 인덱스 기능을 제공합니다.

중앙 집중형 라우팅: 각 프로그램의 상세 페이지와 Slate 엔진 기반의 프로젝트들을 유기적으로 연결하여 사용자 경험의 일관성을 유지합니다.

### Web CMS 
/admin 경로를 통해 제공되는 관리자 인터페이스는 기술적 지식이 부족한 운영자도 고성능 콘텐츠를 관리할 수 있도록 설계되었습니다.

문서 라이프사이클 제어: 신규 MDX 문서 생성, 기존 문서의 실시간 수정 및 삭제를 지원합니다.

순서 및 구조 관리: 드래그 앤 드롭 또는 파일명 프리픽스 제어를 통해 사이드바 및 챕터 노출 순서를 GUI 상에서 즉시 변경할 수 있습니다.

실시간 위지윅(WYSIWYG) 편집: 커스텀 React 컴포넌트(Callout, StepList, Columns 등)가 적용된 결과물을 미리보며 편집할 수 있습니다.

자동화된 배포 연동: 저장 시 GitHub API를 호출하여 소스 코드를 업데이트하며, 이는 곧바로 CI/CD 빌드로 이어집니다.

협업 안정성 (Soft Lock): 동일 문서에 대한 다중 사용자의 동시 수정을 방지하기 위해 경량 잠금 시스템을 제공합니다.

책임 추적 (Audit Trail): 누가 어떤 문서를 생성/수정/삭제했는지 GitHub 커밋 히스토리에 명확하게 기록하여 운영의 투명성을 확보합니다.


---

## 부가기능

- **프리미엄 MDX 컴포넌트**: 안내 박스(Callout), 추진 절차(StepList), 아코디언(Details), 다단 레이아웃(Columns), 단계별 블록(Phase Blocks) 등 공공기관 브로슈어에 특화된 커스텀 React 컴포넌트 제공.
- **다양한 레이아웃 규격**: 리플렛(B5), 브로슈어(A4), 포스터(A3), 시네마(Wide) 등 실제 판촉물 규격에 맞춘 5단계 레이아웃 프리셋 제공.
- **지능형 폰트 시스템**: 지마켓 산스, 프리텐다드, 나눔고딕 등 공공기관 및 홍보물에 최적화된 서체를 기본 탑재하여 별도 설정 없이 즉시 사용 가능.
- **제로-설정 CMS**: 별도의 로컬 환경 없이 `/admin` 경로를 통해 즉시 접속 가능한 관리자 포탈. 실제 디자인과 100% 일치하는 실시간 미리보기 지원.
- **자동 CI/CD 파이프라인**: GitHub Actions와의 연동을 통해 저장 버튼 클릭 한 번으로 자동 빌드 및 배포.
- **고성능 SSG**: Docusaurus 3 기반의 정적 사이트 생성으로 압도적인 페이지 로딩 속도와 SEO 최적화.
- **지능형 UX**: 스크롤 추적 목차(Scroll-Spy TOC), 부드러운 전환 효과, 마케팅에 최적화된 반응형 레이아웃.

---

