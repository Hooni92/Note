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

#### 자료구조 - 비전공자 version
### 
