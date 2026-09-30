# 📚 학습 정리 노트 (Sourcetree & CSS3)

이 레포지토리는 버전 관리 툴인 **Sourcetree**의 기본 개념과 설치 과정, 그리고 **명품 웹 프로그래밍 - CSS3 고급 활용** 학습 내용을 요약한 공간입니다.

## 🌳 1. Sourcetree 개요 및 사용법

### 🔹 주요 특징
* **직관적인 버전 관리**: 커밋(Commit) 이력, 브랜치(Branch) 병합 과정, 코드 변경 차이(Diff)를 시각적인 그래프로 한눈에 확인 가능합니다.
* **복잡한 CLI 명령어 대체**: 마우스 클릭만으로 `Commit`, `Push`, `Pull`, `Merge`, `Rebase`, `Stash` 등 Git의 핵심 기능을 수행할 수 있습니다.
* **원격 저장소 연동**: GitHub, Bitbucket, GitLab 등 주요 Git 호스팅 서비스와 쉽게 연동됩니다.
* **무료 제공**: Windows 및 macOS 환경에서 무료로 사용 가능합니다.

### 🛠️ 설치 과정
1. **다운로드 및 약관 동의**: 공식 웹사이트에서 설치 파일 다운로드 및 라이선스 동의.
2. **계정 연동 설정**: Bitbucket 연동 단계에서 필요 시 건너뛰기 선택 가능.
3. **Mercurial 옵션 해제**: Git 사용이 목적이므로 불필요한 Mercurial 옵션은 체크 해제.
4. **사용자 정보 입력**: 이름 및 이메일 주소 설정.
5. **SSH 키 설정**: 기존 SSH 키 보유 여부에 따라 선택 후 설치 완료.
6. **화면 구성**: 로컬 디렉토리를 열면 Git 상태 및 이력을 시각적으로 분석하여 출력합니다.

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

### 🧭 리스트 및 네비게이션 메뉴 꾸미기
* **리스트 스타일**: `list-style-type`, `list-style-image`, `list-style-position` 등으로 불릿 및 마커 모양을 제어합니다.
* **내비게이션 바(GNB) 구현**: `<ul>`, `<li>` 태그에 `display: inline-block`과 `list-style-type: none`을 조합하여 상단 메뉴바를 구성합니다.

### 📊 표 (Table) 스타일링
* **테두리 설정**: `border` 프로퍼티로 테두리 두께 및 모양을 지정합니다.
* **테두리 병합**: `border-collapse: collapse;`를 사용하여 셀 간 중복되는 테두리를 깔끔하게 하나로 합칩니다.
* **셀 크기 및 효과**: `width`, `height`, `padding` 지정 및 마우스 오버(`tr:hover`) 효과를 추가할 수 있습니다.
