# 📚 학습 정리 노트 (Sourcetree, CSS3 & GitHub 협업)

이 레포지토리는 버전 관리 툴인 **Sourcetree**의 기본 개념과 설치 과정, **명품 웹 프로그래밍 - CSS3 고급 활용**, 그리고 **GitHub를 활용한 팀 프로젝트 협업 가이드** 내용을 통합하여 요약한 공간입니다.

---

## 📑 목차 (Table of Contents)
- [🌳 1. Sourcetree 개요 및 사용법](#-1-sourcetree-개요-및-사용법)
  - [🔹 주요 특징](#-주요-특징)
  - [🛠 설치 과정](#️-설치-과정)
- [🎨 2. (명품 웹 프로그래밍) CSS3 고급 활용 요약](#-2-명품-웹-프로그래밍-css3-고급-활용-요약)
  - [📦 태그 배치와 박스 모델 (Positioning & Layout)](#-태그-배치와-박스-모델-positioning--layout)
  - [🧭 리스트 및 네비게이션 메뉴 꾸미기](#-리스트-및-네비게이션-메뉴-꾸미기)
  - [📊 표 (Table) 스타일링](#-표-table-스타일링)
- [🤝 3. GitHub로 협업하기 (Git & GitHub 워크플로우)](#-3-github로-협업하기-git--github-워크플로우)
  - [⚖️ Git vs GitHub 개념 비교](#️-git-vs-github-개념-비교)
  - [📖 핵심 용어 정리](#-핵심-용어-정리)
  - [🛠️ 팀장 & 팀원 세팅 가이드](#️-팀장--팀원-세팅-가이드)
  - [🔌 외부 협업 툴 연동 (Slack, Jira)](#-외부-협업-툴-연동-slack-jira)

---

## 🌳 1. Sourcetree 개요 및 사용법

### 🔹 주요 특징
* **직관적인 버전 관리**: 커밋(Commit) 이력, 브랜치(Branch) 병합 과정, 코드 변경 차이(Diff)를 시각적인 그래프로 한눈에 확인 가능합니다.
* **복잡한 CLI 명령어 대체**: 마우스 클릭만으로 `Commit`, `Push`, `Pull`, `Merge`, `Rebase`, `Stash` 등 Git의 핵심 기능을 수행할 수 있습니다.
* **원격 저장소 연동**: GitHub, Bitbucket, GitLab 등 주요 Git 호스팅 서비스와 쉽게 연동됩니다.
* **무료 제공**: Windows 및 macOS 환경에서 무료로 사용 가능합니다.

---

### 🛠️ 설치 과정
1. **다운로드 및 약관 동의**: 공식 웹사이트에서 설치 파일 다운로드 및 라이선스 동의.
2. **계정 연동 설정**: Bitbucket 연동 단계에서 필요 시 건너뛰기 선택 가능.
3. **Mercurial 옵션 해제**: Git 사용이 목적이므로 불필요한 Mercurial 옵션은 체크 해제.
4. **사용자 정보 입력**: 이름 및 이메일 주소 설정.
5. **SSH 키 설정**: 기존 SSH 키 보유 여부에 따라 선택 후 설치 완료.
6. **화면 구성**: 로컬 디렉토리를 열면 Git 상태 및 이력을 시각적으로 분석하여 출력합니다.

---

## 🎨 2. (명품 웹 프로그래밍) CSS3 고급 활용 요약

### 📦 태그 배치와 박스 모델 (Positioning & Layout)
* **디스플레이 (`display`)**
  * `block`: 새 줄에서 시작하여 너비를 전체 차지합니다.
  * `inline`: 콘텐츠 크기만큼만 차지하며 한 줄에 이어 배치됩니다.
  * `inline-block`: 인라인처럼 한 줄에 배치되면서 블록 크기 지정이 가능합니다.
* **위치 지정 (`position`)**
  * `static`: Normal Flow에 따른 기본 배치입니다.
  * `relative`: 기본 위치를 기준으로 상대적 이동 (`top`, `bottom`, `left`, `right`)을 합니다.
  * `absolute`: 가장 가까운 상위 위치 지정 조상 요소를 기준으로 절대 배치됩니다.
  * `fixed`: 뷰포트(브라우저 화면)를 기준으로 고정 배치됩니다 (스크롤해도 이동하지 않음).
* **유동 배치 및 중첩 (`float` & `z-index`)**
  * `float: left/right`: 텍스트나 요소가 이미지 주변을 감싸도록 유동 배치합니다.
  * `z-index`: 요소들이 겹칠 때 앞뒤 수직 레이어 순서를 지정합니다 (숫자가 클수록 위에 표시).
* **표시 제어 (`visibility` & `overflow`)**
  * `visibility: hidden`: 요소가 영역은 차지하되 눈에 보이지 않게 처리합니다.
  * `overflow`: 콘텐츠가 박스 영역을 벗어날 때의 처리 방식을 정의합니다 (`visible`, `hidden`, `scroll`).

---

### 🧭 리스트 및 네비게이션 메뉴 꾸미기
* **리스트 스타일**: `list-style-type`, `list-style-image`, `list-style-position` 등으로 불릿 및 마커 모양을 제어합니다.
* **내비게이션 바(GNB) 구현**: `<ul>`, `<li>` 태그에 `display: inline-block`과 `list-style-type: none`을 조합하여 상단 메뉴바를 구성합니다.

---

### 📊 표 (Table) 스타일링
* **테두리 설정**: `border` 프로퍼티로 테두리 두께 및 모양을 지정합니다.
* **테두리 병합**: `border-collapse: collapse;`를 사용하여 셀 간 중복되는 테두리를 깔끔하게 하나로 합칩니다.
* **셀 크기 및 효과**: `width`, `height`, `padding` 지정 및 마우스 오버(`tr:hover`) 효과를 추가할 수 있습니다.

---

## 🤝 3. GitHub로 협업하기 (Git & GitHub 워크플로우)

### ⚖️ Git vs GitHub 개념 비교
* **Git**: 개별 컴퓨터에서 작동하는 버전 관리 프로그램으로, 로컬 환경에서 코드 변경 이력을 기록합니다.
* **GitHub**: 인터넷 클라우드 기반 웹 서비스로, Git으로 기록된 프로젝트를 업로드하여 팀원들과 공유하고 협업할 수 있는 공간입니다.

---

### 📖 핵심 용어 정리
* **Issue (이슈)**: 버그 수정, 새로운 기능 개발 등 앞으로 해야 할 일이나 작업 목록을 적어두는 게시판.
* **Repository (저장소)**: 프로젝트 파일과 전체 변경 이력이 보관되는 클라우드상의 메인 폴더.
* **Branch (브랜치)**: 원본 코드(`main`)에 영향을 주지 않고 안전하게 작업할 수 있도록 만든 독립된 복사본 작업 공간.
* **Pull Request (PR)**: 내 브랜치에서 완료된 작업을 원본(`main`) 브랜치에 합쳐달라고 요청하는 공식 제출서.
* **Code Review (코드 리뷰)**: 팀원들이 제출된 PR의 코드를 점검하고 피드백을 남기는 과정.
* **Merge (머지)**: 코드 리뷰를 거친 이상 없는 작업물을 최종적으로 메인 원본 코드에 통합하는 단계.

---

### 🛠️ 팀장 & 팀원 세팅 가이드

#### **팀장 세팅 가이드**
1. **새 저장소 생성**: GitHub에서 `New repository`를 생성하고 프로젝트 이름과 설명을 작성.
2. **기본 파일 추가**: `README.md` 및 개발 환경에 맞는 `.gitignore` 파일 설정.
3. **팀원 초대**: `Settings > Collaborators` 메뉴에서 팀원들의 계정을 검색하여 초대.
4. **브랜치 보호 규칙 설정(권장)**: `Settings > Branches`에서 `main` 브랜치에 직접 푸시를 막고, 반드시 PR 제출 후 리뷰를 거치도록 설정 (`Require a pull request before merging`).

#### **팀원 세팅 가이드**
1. **초대 수락 및 클론(Clone)**: 초대를 수락한 뒤 저장소 URL을 복사하여 내 컴퓨터에 다운로드.
   ```bash
   git clone [저장소 URL]
   ```
2. **작업용 브랜치 생성 및 이동**:
   ```bash
   git checkout -b feature/내기능이름
   ```
3. **코드 작성 및 커밋(Commit)**:
   ```bash
   git add .
   git commit -m "작업 내용 설명"
   ```
4. **원격 저장소에 푸시(Push)**:
   ```bash
   git push origin feature/내기능이름
   ```
5. **Pull Request (PR) 작성**: GitHub 웹 페이지에서 `Compare & pull request` 버튼을 눌러 PR 생성.

---

### 🔌 외부 협업 툴 연동 (Slack, Jira)

#### **슬랙(Slack) 연동**
* **앱 설치 및 채널 연결**: Slack에 GitHub 앱을 설치하고, 원하는 채널에서 아래 명령어로 알림 구독.
  ```bash
  /github subscribe [조직명/레포지토리이름]
  ```
* **알림 설정**: `/github settings` 명령어를 통해 PR, 이슈, 커밋 등 수신할 알림 항목 제어 가능.

#### **지라(Jira) 연동**
* **앱 연결**: Jira의 `Apps` 메뉴에서 `GitHub for Jira`를 설치하고 레포지토리를 연결.
* **이슈 키 연동**: 커밋 메시지 작성 시 지라 이슈 번호(예: `PROJ-123`)를 포함하면 지라 보드에 작업 현황이 자동 연동됨.
  ```bash
  git commit -m "PROJ-123: 메인 페이지 HTML 레이아웃 작성"
  ```
