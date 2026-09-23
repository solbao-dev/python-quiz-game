# Python Quiz Game

> **Console quiz application built with Python, OOP, JSON, and Git**  
> Python 기초 문법부터 객체지향·파일 저장·Git 협업 흐름까지 연결해 구현한 콘솔 퀴즈 게임

`Python` `OOP` `JSON` `Git` `CLI`

---

## Overview | 프로젝트 소개

A console-based quiz application created during the CODYSSEY Foundation Program. The project combines Python fundamentals with object-oriented design, persistent JSON data, defensive input handling, and practical Git workflows.

CODYSSEY 입학연수 과정에서 Python의 기본 문법을 실제 프로그램으로 연결하기 위해 만든 콘솔 기반 퀴즈 게임입니다. `Quiz`와 `QuizGame` 클래스로 역할을 나누고, `state.json`을 통해 퀴즈와 최고 점수를 저장하며 Git의 기본 협업 흐름까지 함께 실습했습니다.

## Key Features | 주요 기능

- Play quizzes and calculate scores | 퀴즈 풀이 및 점수 계산
- Add and list custom quizzes | 사용자 퀴즈 추가·목록 조회
- Persist data with JSON | JSON 기반 데이터 저장
- Track best score | 최고 점수 기록
- Defensive input handling | 잘못된 입력 및 종료 예외 처리

## Design | 설계

- `Quiz` — question, choices, and answer data | 문제·보기·정답 데이터
- `QuizGame` — application flow and state management | 게임 흐름·상태 관리
- `state.json` — quizzes and best-score persistence | 퀴즈·최고점수 영속 저장

## Run | 실행

```bash
git clone https://github.com/solbao-dev/python-quiz-game.git
cd python-quiz-game
python main.py
```

## What I Learned | 핵심 학습

이 프로젝트에서는 단순히 Python 문법을 사용하는 데서 그치지 않고 **데이터와 동작을 클래스로 나누는 이유**, 파일에 상태를 저장하는 방법, 예외 상황에서 프로그램을 안전하게 유지하는 방법을 익혔습니다.

또한 Git과 GitHub가 서로 다른 역할을 가진다는 점부터 clone, push, pull, branch, merge까지 직접 시행착오를 겪으며 버전 관리의 기본 흐름을 학습했습니다.

## Learning Log | 상세 학습 기록

초기 학습 당시의 Git 오류, Python 들여쓰기 문제, 작업 디렉토리 혼동, clone/pull 실습과 평가 준비 내용은 별도 로그에 보존했습니다.

➡️ **[View Detailed Learning Log](./docs/LEARNING_LOG.md)**

---

**CODYSSEY AI All-in-One · Foundation Program**