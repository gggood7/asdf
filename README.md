# 리눅스 명령어

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

**ps 명령어와 top 명령어의 차이점**

ps는 ps한 시점에서 proc에서 검색한 CPU 검색량
top는 proc에서 일정 주기로 합산해 cpu 사용율 출력

---

3) ___jobs 명령어___

백그라운드로 실행되는 작업의 상태를 표시하는 명령어

`[작업 명령어] &`로 실행

백그라운드로 실행되는 작업의 상태를 표시하는 명령어

`jobs [option][%작업번호]` 형태로 사용

 

* jobs 명령어 옵션

`-l` : 프로세스 그룹 ID를 state필드 앞에 출력

`-n` : 프로세스 그룹 중에 대표 프로세스 ID를 출력

`-p` : 각 프로세스 ID에 대해 한 행씩 출력

`Command` : 지정한 명령어를 실행

`kill %[작업번호]` : 종료

 

<img width="697" alt="jobs 명령어 실행" src="https://user-images.githubusercontent.com/103065628/172044549-3097d665-1c93-456a-b66d-62da9741a908.png">

_(실제 명령어를 입력했을 때의 터미널)_

---

4) ___kill 명령어___

프로세스에 시그널을 보내는 명령어

`kill [option][PID]` 형태로 사용

 

* kill 명령어 옵션

`-l` : 사용 가능한 시그널 목록을 출력

`-1` : 재실행

`-9` : 강제 종료

`-15` : 정상 종료

 

<img width="697" alt="kill 명령어 사용" src="https://user-images.githubusercontent.com/103065628/172044742-69f67a15-0075-4a31-bd12-e38ec7117510.png">

_(실제 명령어를 입력했을 때의 터미널)_

---

# VIM 에디터에서의 매크로 사용

___매크로___

매크로는 같은 동작을 반복하게 하는 것

 
 
* 실행 방법

1. `q[name]`을 눌러 기록을 시작

2. 매크로 반복 동작을 입력하고 입력이 끝나면

3. 다시 `q`를 눌러 기록 종료

(이제 [name]이라는 매크로가 생성됨)

4. @[name]을 누르면 자동으로 매크로가 실행됨

 

_`[숫자]@[name]` : 숫자만큼 매크로가 실행됨_

_`@@` : 방금 실행한 매크로 실행_

