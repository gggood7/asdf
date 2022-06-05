## 리눅스 명령어

1) ___top 명령어___

top 명령어는 실시간으로 현재 os의 상태를 나타내주는 CLI 어플리케이션

(CPU의 사용율 체크 / CPU, Memory, Process)

옵션 없이 실행하면 interval 간격(3초)로 갱신하여 정보를 보여줌

`top [option]` 형태로 사용

* top 명령어 옵션

`-b` : batch 모드(순간 정보)

`-n` : 실행 주기 설정

`shift + p` : CPU 사용률 내림차순

`shift + m` : Memory 사용률 내림차순

`shift + t` : 프로세스가 돌아가고 있는 시간 순  등...

Page up/down을 통해 페이지 이동이 가능

<img width="795" alt="top 명령어 사용" src="https://user-images.githubusercontent.com/103065628/172044049-5993e9d3-a8c0-42b4-97e0-a1a9d10c06e4.png">

_(실제 명령어를 입력했을 때의 터미널)_

---

2) ___ps 명령어___

process status의 약자로 
현재 실행 중인 프로세스 목록과 상태를 보여줌

`ps [option]` 형태로 사용

* ps 명령어 옵션

`-e` : 실행 중인 모든 프로세스의 정보를 출력

`-f` : 프로세스에 대한 자세한 정보를 출력(PPID 확인 가능)

`-u[사용자 이름]` : 특정 사용자에 대한 모든 프로세스의 정보를 출력

`-p PID` : PID로 지정한 프로세스의 정보를 출력  등...

<img width="697" alt="ps 명령어 사용" src="https://user-images.githubusercontent.com/103065628/172044420-9865dbb3-c110-4755-ac50-36bf7f829bcb.png">

_(실제 명령어를 입력했을 때의 터미널)_

---

3) ___jobs 명령어___

백그라운드로 실행되는 작업의 상태를 표시하는 명령어

`jobs [option][%작업번호]` 형태로 사용

* jobs 명령어 옵션

`-l` : 프로세스 그룹 ID를 state필드 앞에 출력

`-n` : 프로세스 그룹 중에 
