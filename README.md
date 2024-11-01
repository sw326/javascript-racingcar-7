# 자동차 경주 게임

## 프로젝트 소개

이 프로젝트는 간단한 자동차 경주 게임을 구현한 것입니다. 사용자가 자동차 이름과 시도 횟수를 입력하면, 무작위로 자동차들이 전진하거나 멈추는 경주를 시뮬레이션합니다.

## 기능 목록

- 자동차 이름 입력 및 검증
  - 쉼표(,)로 구분된 이름 입력
  - 이름 길이 1-5자 제한
  - 중복 이름 검증
  - 빈 입력 검증
- 시도 횟수 입력 및 검증
  - 양의 정수만 허용
  - 소수점 입력 방지
- 자동차 전진 로직
  - 0-9 사이 무작위 값 생성
  - 4 이상일 때 전진
- 경주 결과 출력
  - 각 라운드별 진행 상황
  - 최종 우승자 결정

## 프로젝트 구조

```
src/
├── App.js         # 메인 애플리케이션 로직
├── App.test.js    # 테스트 코드
└── index.js       # 진입점
```

### 주요 컴포넌트

- **상수 관리**
  - GAME_CONSTANTS: 게임 관련 상수
  - ERROR_MESSAGES: 에러 메시지 상수
- **클래스 구조**
  - App: 메인 게임 로직 클래스
  - Car: 자동차 객체 타입 정의

## 테스트

Jest를 사용한 단위 테스트 구현:

- 입력 검증 테스트
  - 빈 입력 처리
  - 중복 이름 검증
  - 이름 길이 제한
- 게임 진행 테스트
  - 자동차 전진 로직
- 우승자 결정 테스트
  - 단독 우승
  - 공동 우승

## 예외 처리

- 입력값 검증
  - 자동차 이름 형식
  - 시도 횟수 유효성
- 에러 메시지 표준화
- try-catch를 통한 안정적인 에러 처리

## 실행 방법

```bash
# 패키지 설치
npm install

# 게임 실행
npm run start

# 테스트 실행
npm run test
```

## 코드 컨벤션

- JavaScript Style Guide 준수
- JSDoc을 통한 타입 힌트 제공
- 상수 분리로 매직 넘버 제거
- 단일 책임 원칙 준수

## 개선된 기능

- 강화된 입력 검증
- 체계적인 에러 처리
- 명확한 타입 정의
- 구조화된 테스트

이 프로젝트는 우아한테크코스 프리코스 과제로 진행되었습니다.
