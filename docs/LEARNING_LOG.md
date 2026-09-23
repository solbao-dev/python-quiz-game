# Python Quiz Game — Learning Log

> CODYSSEY Foundation Program에서 Python, OOP, JSON, Git을 처음 프로젝트 형태로 연결하며 남긴 학습·트러블슈팅 기록입니다.

## Learning Scope | 학습 범위

- Python 기본 문법과 클래스
- 객체지향 구조화
- JSON 기반 상태 저장
- 예외 처리
- Git clone / commit / push / pull / branch / merge
- 터미널과 작업 디렉토리 이해

## Troubleshooting Log | 문제 해결 기록

### 1. Git author identity
첫 커밋에서 `Author identity unknown`이 발생했습니다. GitHub 로그인과 로컬 Git 사용자 설정은 별개라는 점을 확인하고 `git config --global user.name`, `user.email`을 설정해 해결했습니다.

### 2. Python `IndentationError`
코드 수정·복사 과정에서 불필요한 공백/탭으로 `unexpected indent`가 발생했습니다. Python에서는 들여쓰기가 코드 블록 자체를 정의한다는 점을 확인하고 정렬을 수정했습니다.

### 3. `git clone [URL]` 입력 오류
가이드의 대괄호를 실제 입력 문자로 오해해 zsh 패턴 매칭 오류가 발생했습니다. placeholder 표기와 실제 명령어 입력값의 차이를 익혔습니다.

### 4. Working directory mismatch
터미널은 clone 실습 폴더에 있었지만 실제 수정 파일은 원본 프로젝트 폴더에 있어 Git이 변경을 감지하지 못했습니다. `pwd`, `cd`, `git status`를 통해 현재 작업 위치를 먼저 확인하는 습관을 익혔습니다.

### 5. macOS terminal Korean input issue
터미널 한글 입력 중 버퍼/렌더링 문제가 발생했을 때 `Ctrl+U`, `Ctrl+C`와 재실행으로 복구했습니다.

## Git Collaboration Practice | Git 협업 실습

- 저장소를 별도 디렉토리에 clone
- clone된 작업공간에서 README 수정 후 push
- 원본 작업공간에서 pull하여 원격 변경사항 동기화
- branch를 분리해 작업하고 merge하는 기본 흐름 학습

## Deep Dive | 평가 준비 기록

### Why classes? | 클래스를 사용한 이유
`Quiz`는 질문·보기·정답 데이터를, `QuizGame`은 게임 흐름과 상태 관리를 담당하도록 책임을 분리했습니다. 데이터와 동작을 객체로 묶어 전역 상태 의존을 줄이고 유지보수성을 높이는 목적입니다.

### Why JSON? | JSON을 사용한 이유
Python의 `dict`, `list`와 자연스럽게 매핑되고 사람이 읽을 수 있는 텍스트 포맷이라 작은 프로젝트의 상태 저장과 직렬화 학습에 적합했습니다.

### Why `try/except`? | 예외 처리를 사용한 이유
잘못된 사용자 입력, 파일 부재, `KeyboardInterrupt` 등 예상 가능한 실패 상황에서 프로그램이 비정상 종료되지 않도록 방어적으로 처리했습니다.

### Branch & Merge
기능 작업을 독립된 branch에서 진행한 뒤 검증된 변경을 main에 merge하는 흐름을 통해 버전 관리와 협업의 기본 개념을 학습했습니다.

---

> 초기 프로젝트에서 겪은 시행착오를 지우지 않고, 현재의 프로젝트 README와 분리하여 성장 기록으로 보존합니다.