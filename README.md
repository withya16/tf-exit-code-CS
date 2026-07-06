# 🚀 Exit Code 0 - Tech Interview Track

단순히 CS 지식을 넓게 훑는 것이 아니라, **기본 개념을 이해하고**, **면접 답변으로 정리하고**, **꼬리질문에 대응할 수 있도록 깊게 학습하는 것**을 지향합니다.

---

## 1. 스터디 개요

### 장소 및 시간

- 과제 기한: 매주 일요일 자정
- 라이브 다대다 모의면접: 격주 진행 예정
- 라이브 다대다 모의면접은 가능하면 대면 진행을 원칙으로 하되, 상황에 따라 Discord로 대체 가능

### 참여자
<table>
  <tr>
    <td align="center">
      <a href="https://github.com/minsubyun1">
        <img src="https://avatars.githubusercontent.com/u/75060858?v=4" width="100px;" alt="윤민섭"/>
        <br />
        <sub><b>윤민섭</b></sub>
      </a>
      <br />
      <sub>TF장</sub>
    </td>
  </tr>
</table>
---

## 2. 주차별 커리큘럼

기본 운영 기간은 약 8~9주이며, 진행 상황에 따라 추가 운영할 수 있습니다. (시즌 1 한달 간 CS, 시즌 2는 직무에 맞춘 세부 질문으로 진행)

| 주차 | 시즌 | 주제 | 질문 범위 | 진행 내용 |
| --- | --- | --- | --- | --- |
| Week 01 | Season 1 - 공통 CS 압축 | Computer Architecture + OS Runtime | COMMON-001 ~ COMMON-040 | 컴퓨터가 코드를 실행하는 흐름, CPU, 레지스터, 명령어 사이클, 컴파일/인터프리터, 프로세스, 스레드, 컨텍스트 스위칭 |
| Week 02 | Season 1 - 공통 CS 압축 | OS Memory / Concurrency + Core Data Structure | COMMON-041 ~ COMMON-080 | 메모리 구조, Stack/Heap, 가상 메모리, Page Fault, 동시성, Mutex/Semaphore, Deadlock, Hash, Tree, Heap |
| Week 03 | Season 1 - 공통 CS 압축 | Network / Web / I/O | COMMON-081 ~ COMMON-120 | 요청이 서버까지 가는 흐름, OSI/TCP-IP, TCP/UDP, HTTP/HTTPS, DNS, REST, WebSocket, Blocking/Non-blocking, I/O Multiplexing |
| Week 04 | Season 1 - 공통 CS 압축 | Database / Storage / Cache | COMMON-121 ~ COMMON-160 | 데이터 저장과 조회, Key, 정규화, Join, Index, Transaction, Isolation Level, Lock, Connection Pool, Replication, Cache |
| Week 05 | Season 1 - 공통 CS 압축 | Software Engineering / Design Pattern | COMMON-161 ~ COMMON-200 | OOP, SOLID, Design Pattern, Layered Architecture, 테스트, 좋은 코드 구조, 시스템 설계 기초 |
| Week 06 | Season 2 - 직무별 심화 | Role-Based Interview 1 | ROLE-001 ~ ROLE-040 | 희망 직무별 핵심 질문 선정 및 답변 작성. Backend, Cloud/DevOps, Frontend, Data/AI 등 각자 직무에 맞는 질문 대비 |
| Week 07 | Season 2 - 직무별 심화 | Role-Based Interview 2 | ROLE-041 ~ ROLE-080 | 직무별 상세 질문, 기술 선택 이유, 트레이드오프, 직무 적합성 중심 답변 정리 |
| Week 08 | Season 2 - 프로젝트/포트폴리오 | Project-Based Interview | PROJECT-001 ~ PROJECT-040 | 프로젝트 구조, 본인 역할, 기술적 의사결정, 트러블슈팅, 성능 개선, 장애 대응, CS 개념과 프로젝트 연결 |


진행 상황에 따라 특정 주제는 2주 이상 다룰 수 있으며, 참여자들의 필요에 따라 추가 주차를 운영할 수 있습니다.

---

## 3. 주차별 제출 방식

매주 일요일 자정까지 질문에 대한 답변을 PR로 제출합니다.

각 질문에 대해 **본인의 언어로 설명 가능한 답변**을 작성하는 것을 목표로 합니다.

### 필수 제출 항목

- 질문에 대한 개념 정리 및 본인의 답변
- 질문은 주에 주제 별로 40개씩 출제되지만, 최소 20개에 답변 작성 후 제출을 원칙으로 합니다.

### 선택 작성 항목

아래 항목은 필수가 아니며, 필요하다고 판단되는 경우에만 작성합니다.

- 참고 자료
- 꼬리 질문 및 답변
- 추가로 공부한 개념
- 프로젝트 / 과제 경험과의 연결
- 헷갈렸던 부분
- 함께 고민하고 싶은 부분

답변 예시

```jsx
# Week 01 - Computer Architecture + OS Runtime

## 담당자

- 이름:

---

## [OS-001] 시스템 콜이 무엇인지 설명해 주세요.

시스템 콜은 사용자 프로그램이 운영체제 커널의 기능을 사용하기 위해 요청하는 인터페이스입니다.  
일반 애플리케이션은 파일 입출력, 프로세스 생성, 네트워크 통신처럼 하드웨어나 커널 자원에 직접 접근할 수 없기 때문에, 시스템 콜을 통해 커널 모드로 전환한 뒤 OS가 대신 작업을 수행합니다.

대표적인 예시로는 `read`, `write`, `open`, `fork`, `exec` 등이 있습니다.

참고 자료:
- 

---

## [OS-002] 우리가 사용하는 시스템 콜의 예시를 들어주세요.

파일을 읽을 때 사용하는 `read`, 파일을 열 때 사용하는 `open`, 프로세스를 생성할 때 사용하는 `fork`, 새로운 프로그램을 실행할 때 사용하는 `exec` 등이 시스템 콜의 예시입니다.

개발자가 직접 시스템 콜을 호출하지 않더라도, Java의 파일 입출력 API나 Python의 `open()` 같은 고수준 API 내부에서 운영체제의 시스템 콜이 호출될 수 있습니다.

참고 자료:
- 
```
