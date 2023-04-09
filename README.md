### TCP/IP Network
![image](https://user-images.githubusercontent.com/108508922/228227771-5bc58c1a-32ac-40e7-a163-0a2e649c9e4c.png)
- 커널의 구성요소를 어플리케이션을 추상화할때 File요소로 추상화 하는데 이때 네트워크에 관련된 File을 Socket이라 부른다.
- Socket이란? TCP/IP 소켓이라 했을때 user mode application process가 접근할 수 있도록 파일형식으로 추상화한 interface를 Socket이라 한다.
- 식별자: MAC (Hardware 수준), IP주소(Network수준), Port번호(Transport 수준)

### MAC주소, IP주소, Port 번호가 식별하는것
![image](https://user-images.githubusercontent.com/108508922/228231689-04068427-4d31-4f06-b31b-e268058c3871.png)

- MAC주소: NIC(NetworkInterfaceCard, LAN 카드)에 대한 식별자. MAC주소는 변경가능한가? : Yes
- IP주소: Host에 대한 식별자. Host: 인터넷에 연결된 컴퓨터. IP주소는 몇개나 있을까? :N개, NIC 한개에 여러개 바인딩 가능하다.
- Port번호: 프로세스 식별자, 서비스 식별자, 인터페이스 식별자 와 같이 업무관점에 따라 다르게 불려온다.

### Host, Switch, Network
![image](https://user-images.githubusercontent.com/108508922/228235475-2a8756f6-10be-4aed-b130-c9fe186f0873.png)
- Host : Computer + Network  
- End-Point : 인터넷에 연결된 컴퓨터가 Host인데 이때 컴퓨터가 Netwokr 이용 주체이면 End-Point라 한다. ex) Peer, Server, Client
- Switch : 인터넷에 연결된 컴퓨터가 Host인데 이때 컴퓨터가 Netwokr 자체를 이루면 Switch라 한다. ex) Router, FW, IPS.  
- MAC 주소를 Swithching 하면 L2 Swithch, IP주소를 Swithching 하면 L3 Swithch, Port번호를 Swithching 하면 L4 Swithch, Http를 Swithching 하면 L7 Swithch.
- Network : Internet이란? Router + DNS

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### 자료구조란 무엇인가?
- 자료구조란? :  현실의 체계를 컴퓨터 체게에 효율적 데이터 관리하는법.
- 자료구조의 목적: 큰 데이터를 효율적으로 관리하는 것.
### 자료구조 - Array(배열)
- 배열이란?: 여러 데이터를 하나의 이름으로 그룹핑해서 관리하기 위한 자료구조.
- 배열에 자료를 넣으면 index라는 색인을 가지게 되며 index는 데이터를 식별하는 역할을 해준다.
![image](https://user-images.githubusercontent.com/108508922/229144495-90c71ab9-1551-4bc0-8110-f7234bea1b1f.png)
- 값=value, 값의 식별자= index, 값+식별자 = element
- 배열의 생성 ex) int[] numbers1 = new int[4]
![image](https://user-images.githubusercontent.com/108508922/229145695-c9b59b89-f8e8-49e9-8da0-8ff2b4ba8d55.png)
- 생성된 배열
![image](https://user-images.githubusercontent.com/108508922/229146040-22327090-10d0-4bbf-9169-2d5ed525fcba.png)
- 배열의 넣을 값을 미리 알고있다면 다음과 같이 작성하면 쉽다.
![image](https://user-images.githubusercontent.com/108508922/229146505-011fb013-3ae9-4946-b2bd-c64b83db7ec7.png)
- 배열에 설정하지 않은 값을 출력하면 0이 나온다.
![image](https://user-images.githubusercontent.com/108508922/229147522-3991b81e-62c4-4d60-badb-e89e8d14d15a.png)
## 배열의 크기
![image](https://user-images.githubusercontent.com/108508922/229147846-8921be50-d41f-4db4-9e84-c91b449b8326.png)
- element의 개수를 카운트 하기때문에 length 값=4가 된다. 단, 값을 설정하지 않은 값도 length 에 포함된다.
![image](https://user-images.githubusercontent.com/108508922/229148383-9de79a58-30cc-4bca-a904-105eb6ce160f.png)
## Iteration(반복)
- while문
![image](https://user-images.githubusercontent.com/108508922/229148820-ee86b4d7-3bfb-48de-801b-184e86a04b16.png)
- while 문의 단점은 반복을 i=0, numbers.length, i++ 구문이 떨어져있어 중간에 다른 코드가 들어가면 헷갈릴 수 있다. 
- for문
![image](https://user-images.githubusercontent.com/108508922/229149125-9c1519a2-e741-4449-ba1b-b5fe0b32bd3d.png)
- while문보다 보기가 편하다, 반복횟수를 알고있을때 좋다.
## 배열의 장,단점
- 배열의 단점
1. 크기가 정해져있다.
2. 기능이 없다.
- 배열의 장점
1. 작고 가볍다. (크기가 정해져있기 때문에 메모리를 적게 사용할수 있는 조건이 된다.)
2. 단순하다.

### 자료구조 - List
- List의 가장큰 특징 2가지
1. 순서가 정해져있다. (Array보다 순서를 좀더 중요시한다)
2. 중복해서 저장 할 수 있다. 
(Array 또한 순서가 있고 중복이 가능하지만 List의 기능이 많다)
## List 자료 추가
![image](https://user-images.githubusercontent.com/108508922/229151492-6a04b3b9-849b-46e8-b7a5-82bf5e7145d3.png)
- Array에서는 기존 값을 제거하고 새로운 값(50)을 넣는다.
- List에서는 기존 값을 뒤로 보내고 새로운값을 해당 번호에 삽입한다.
## List 자료 삭제
![image](https://user-images.githubusercontent.com/108508922/229152018-8bf11b29-7b54-47c6-ab39-7580e27e459d.png)
- Array에서는 데이터를 삭제하고 빈공간으로 남아있다.
- List에서는 해당 데이터 삭제시 뒷 데이터가 자리를 매꾼다.
- 따라서 List는 연속적인 데이터를 이루기 때문에 데이터의 유무를 확인하지 않아도 되는 장점이 있다.
## List 기능
- 처음, 끝, 중간에 엘리먼트를 추가/삭제하는 기능
- 리스트에 데이터가 있는지를 체크하는 기능
- 리스트의 모든 데이터에 접근할 수 있는 기능
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

### JAVA의 장단점 
장점: 가상머신으로 인해 이식성이 높다. 어떤 운영체제든 적용 가능
단점: 컴파일링 과정이 필요하여 응답이 상대적으로 늦다.(서버에 적합하지 않다)

### 객체지향언어란?
JAVA, Python, C++
객체를 만들고 사용하는 언어, 유지 보수 유리
객체지향 <-> 절차지향 : 3D 프린터, 계산기 

### 자바가상머신이란?
메모리 자동 관리 해주고, 쉽게 다른 운영체제 이식 개발 환경

### 클래스란?
객체의 설계도
예) 자동차 설계도, 붕어빵 틀
객체 : 자동차, 붕어빵
필드값 : 자동차 스펙, 붕어빵 크기

### 상속이란?
코드 재사용, 상위 클래스의 필드값과 메소드를 하위 클래스가 쉽게 이용
아예 상속을 안받을 수 있어도 골라서 받는 것은 안된다.

### 생성자란?
클래스와 이름이 동일한 메소드: 필드 초기화
Human클래스
Human(String name){this.name = name;}
Human human =  new Human("김철수")
- 생성자의 특징
1) 생성자의 이름은 클래스의 이름과 같아야 한다.
2) 생성자는 리턴 값이 없다. void 또한 사용하지 않는다.
3) 생성자는 메소드와 매우 유사하다
4) 생성자는 메소드 처럼 클래스 내에 선언되고, 오버로딩이 가능하므로 하나의 클래스에 여러개의 생성자가 존재 할 수 있다.

- 기본 생성자란, 매개변수 생성자

### 오버로딩과 오버라이딩의 차이점.
오버로딩 : 짐을 쌓는 것, 생성자 변수 추가
오버라이딩: 담벼락을 건너 뛴다. 상위 클래스의 필드값/메소드를 하이 클래스가 이용

### 추상클래스와 일반 클래스의 차이점
객체화 가능 여부: 추상 클래스는 불가, 일반 클래스 가능


### JAVA Compile 과정
![image](https://user-images.githubusercontent.com/108508922/230772778-3d56b979-7974-41d5-9318-d32e2885953d.png)
1. 개발자가 .java 파일을 생성한다
2. build를 한다
3. java compiler의 javac 명령어를 통한 바이트코드(.class) 생성
4. class loader를 통해 jvm내로 로드
5. 실행엔진을 통해 컴퓨터가 읽을 수 있는 기계어로 해석되어(각 운영체제에 맞는 기계어)Runtime Data Area에 배치

### compiler vs interpreter 차이

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

### 운영체제란?
- 시스템의 자원과 동작을 관리하는 소프트웨어.
- 프로세스, 저장장치, 네트워킹, 사용자, 하드웨어를 관리한다.

### 메모리 구조
- Code, Data, Heap, Stack
- ![image](https://user-images.githubusercontent.com/108508922/230784003-9baea2e7-f0de-4941-a59e-136deb01a257.png)
- ![image](https://user-images.githubusercontent.com/108508922/230784066-84127606-05d2-47b7-ba09-a70e2b2d448f.png)
- 코드영역: 실행할 프로그램의 코드
- 데이터영역 : 전역 변수, 정적 변수
- 힙 영역: 사용자의 동적 할당 (런 타임에 크기가 결정됨)
- 스택 영역: 지역변수, 매개변수 (컴파일 타임에 크기가 결정됨)

### 프로세스 & 스레드
- 프로세스: 실행중인 프로그램
- 스레드: 프로세스 안 실행 단위
- 프로세스안에 코드, 데이터, 힙 영역은 공유되지만 스레드는 독립된 스텍을 가진다.

### CPU 스케줄러
- 준비큐에 있는 프로세스에 대해 CPU 할당하는 방법
## 비선점 스케줄링
1) FCFS(First Come First Served)
- 먼저 CPU를 요청하는 프로세스 부터 처리하는 방식
- ![image](https://user-images.githubusercontent.com/108508922/230785376-83081cb9-02a0-4ec9-b2b8-c629bdf60845.png)
 2) SJF(Shortest Job First)
 - 평균 waiting time을 최소화 하기위해 사용하는 방식
 - 버스트 시간이 짧은 프로세스부터 CPU를 할당한다.
 - ![image](https://user-images.githubusercontent.com/108508922/230786490-bec8eee2-725d-4a99-9235-4baf89ce2e15.png)
 ## 선점 스케줄링
 1) SRT(Shorted Remaining Time)
 - 최단 잔여시간을 우선으로 하는 스케줄링
 - ![image](https://user-images.githubusercontent.com/108508922/230786509-5b8700fa-4055-4a79-9809-5487042b24e3.png)
 2) RR(Round Robin)
 - Time Sharing System을 위해 설계된 스케줄링
 - 모든 프로세스가 같은 우선순위를 가지고, time slice를 기반으로 스케줄링한다.
 - Time slice burst가 일어나면 해당 프로세스는 스케줄링 큐의 끝으로 이동한다.
![image](https://user-images.githubusercontent.com/108508922/230787203-77282f04-85bc-4d30-bbee-b7d852db981c.png)

## 우선순위 스케줄링(Priority Scheduling)
- 우선 순위가 높은 프로세스에 CPU를 우선 할당하는 방식의 스케줄링
- 우선 순위는 시간 제한, 메모리 요구량, 프로세스의 중요성, 자원사용 비용 등에 따라 달라질 수 있다.
- 우선 순위가 같은 경우, FCFS와 다를게 없다.
