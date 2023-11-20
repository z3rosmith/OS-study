## 1주차 문제

---

- Q. I/O를 걸때 인터럽트가 몇 가지 걸리는지 설명하고, 각각의 인터럽트의 특징을 설명하시오.

<br><br>

- Q. cache, main memory, magneitic disk, register, optical disk를 저장장치 계층 순으로 나열하고,
휘발성, 속도, 가격측면에서 어떤 계층이 높은지 설명하시오.

<br><br>

- Q. 소프트웨어 인터럽트에서 시스템 콜 말고 어떤 인터럽트가 있는가?

<br><br>

- Q. 가상메모리는 어디에 위치하는가?

<br><br>

Q. 다음은 Interrupt-driven I/O Cycle의 과정이다. 박스 안에 정답을 채워 넣으시오.

   ![week1_problem_1.jpg](https://github.com/gashe-soo/OS-7week-KOCW/blob/main/asset/week1_problem_1.jpg?raw=true)

   - a.  interrupt handler process data, returns from interrupt
   - b. initiates I/O
   - c. CPU receiving interrupt, transfers control to interrupt handler
   - d. CPU resumes processing of interrupted task
   - e. input ready, output complete, or error generates interrupt signal
   - f. device driver initiates I/O

<br><br>

Q. 다음 중 옳은 것을 모두 고르시오.
   - ㄱ. 운영체제는 사용의 용이성을 위해 설계되었고 자원의 이용에는 신경쓰지 않는다.
   - ㄴ. CPU는 하나의 명령어의 실행을 완료할 때마다 인터럽트 라인을 감지한다.
   - ㄷ. Mode bit이 1이 되면서 커널 모드에 진입한다.
   - ㄹ. 메인 메모리는 비휘발성 저장장치이다.
   - ㅁ. DMA는 CPU의 개입 없이 메모리와 버퍼 장치 간의 데이터를 바이트 단위로 전송한다.
   - ㅂ. Swap area는 메모리에 속한다.
   - ㅅ. Memory Mapped I/O는 메모리와 I/O가 하나의 연속된 address 영역에 할당된다.

<br><br>

Q. DMA 컨트롤러가 하는일이 무엇인지?

<br><br>

Q. 커널 주소 공간 메모리의 code, stack, data 가 하는 일에 대해 설명해보기

<br><br>

Q. Multiprocess와 Multiprocessor의 의미 차이?

<br><br>

Q. 운영체제의 자원 관리시에 효율성 말고도 신경써야 하는 특성은?

<br><br>

Q. Mode bit는 2가지 모드의 operation을 지원한다. 2가지는?

<br><br>

Q. DMA가 인터럽트를 발생시키는 단위는?
