## 2주차 문제

---

- Q. Program Counter, code section, register set, data section, OS resources, stack space 중<br>
Thread와 공유하는 부분과 공유하지 않는 부분을 나눠 주세요.

<br><br>

- Q. Multi thread의 장점 중 한가지를 예시로 들어 설명해주세요. ex) 웹 브라우저

<br><br>

- Q. 아래 코드는 process를 생성하고 수행하는 코드이다.<br>
아래 코드를 실행했을 때의 출력과정을 설명해 주세요.<br>
![image](https://user-images.githubusercontent.com/37397737/96326477-f1404c00-106b-11eb-8ccc-4a5786913a73.png)<br>
사진 출처: https://blog.naver.com/PostView.nhn?blogId=scy7351&logNo=221522253222&parentCategoryNo=&categoryNo=21&viewDate=&isShowPopularPosts=true&from=search<br>

<br><br>

- Q. 다음 코드에서 출력되는 값과 그 이유를 설명하시오.<br/>
```c
#include <sys/types.h>
#include <sys/wait.h>
#include <stdio.h>
#include <unistd.h>

int value = 5;
int main()
{
    pid_t pid;
    pid = fork();
    
    if(pid == 0){
        value += 15;
        return 0;
    }
    else if(pid > 0){
        wait(NULL);
        printf("Parent: value = %d\n",value);
        return 0;
    }
}
```
출처 : 운영체제(Operating System Concepts) 10th edition<br/>
<br/>

- Q. O/X를 고르시오.<br/>
    - 같은 프로세스에 있는 각각의 쓰레드는 각각 가상 메모리 mapping을 가진다. (O/X)<br/>
    - 쓰레드는 프로세스보다 문맥 교환(context switch) 비용이 적다.(O/X)<br/>
    - 한 프로세스 내의 스레드들은 Code, Data, Heap 영역을 공유한다.(O/X)<br/>
    
<br/><br/>

#### Q.1. Blocked와 Suspended의 차이 ?

#### Q.2.  PCB가 갖고 있는 정보가 아닌 것은?

<br><br>

- Q. 프로세스와 스레드의 협력 방식의 차이점에 대해 설명하시오

<br><br>

- Q. 한 프로세스가 long term scheduler에 의해 메모리에 올라간 후 대기하다 cpu를 점유한 후

i/o request가 들어와 device controller에 관리되어진 후  i/o가 끝나 다시 memory로 돌아가는 과정을

job queue, ready queue, device queue의 관점에서 서술하시오


######### Q1 ###########

프로세스와 스레드의 협력 방식의 차이점에 대해 설명하시오

########################
######### Q2 ###########

한 프로세스가 long term scheduler에 의해 메모리에 올라간 후 대기하다 cpu를 점유한 후

i/o request가 들어와 device controller에 관리되어진 후  i/o가 끝나 다시 memory로 돌아가는 과정을

job queue, ready queue, device queue의 관점에서 서술하시오

########################
