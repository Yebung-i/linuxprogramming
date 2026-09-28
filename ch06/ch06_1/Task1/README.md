# find 명령어로 .bashrc 파일의 위치를 검색하라.
<img width="500" height="95" alt="image" src="https://github.com/user-attachments/assets/5f9205cf-08b0-4d6c-8319-24b3e4ea9821" />


# 다음 2가지 명령어의 차이는 무엇인가?
## find . -name ‘*.txt’
따옴표로 묶는다면, * 를 하나의 문자열 그대로 find에 전달되어, find가 패턴을 해석해 현재 디렉터리 부터 모든 하위 디렉터리까지 재귀적으로 탐색해 이름이 .txt 로 끝나는 모든 파일을 
검색한다.
## find . -name *.txt
따옴표로 묶지 않았을 경우, 셸이 * 를 경로 확장 문자로 받아들여 find가 실행되기 전, 현재 디렉터리의 .txt 파일명들로 먼저 바꿔버림. 
예를 들어 a/b.txt 가 있다면, `find . - name a.txt b.txt` 로 확장되기 때문에 이 경우 `-name` 은 인자를 하나만 받으므로 오류가 발생함

# --help 옵션을 사용하여 명령어의 사용법을 출력하는 예제를 만들어보라
<img width="770" height="517" alt="image" src="https://github.com/user-attachments/assets/78bac2aa-ce61-4b7a-b9f9-a399d2495f6c" />


# man 명령어로 명령어의 사용법을 출력하는 예제를 만들어보라
<img width="338" height="22" alt="image" src="https://github.com/user-attachments/assets/b2e6dc5b-d507-43e7-a525-fe779de30cc9" />

<img width="1091" height="617" alt="image" src="https://github.com/user-attachments/assets/59a9a820-9513-4bb1-9ae4-7bdb1e14516c" />


# cd, ls, cp, rm, ifconfig 명령어의 실행파일이 존재하는 경로를 조사하라.
<img width="448" height="118" alt="image" src="https://github.com/user-attachments/assets/cff3e975-dcdf-424c-a194-ebe2537c77d9" />
cd는 실행파일이 따로 존재하는 외부 명령어와 달리 bach 프로그램 자체에 기능이 포함되어 있기에 별도의 실행 파일이 없다.

<img width="1030" height="441" alt="image" src="https://github.com/user-attachments/assets/8ede2d5f-15bf-42a7-a83b-4ddd84e34a70" />
ifconfig는 네트워크 인터페이스의 IP 주소 등을 확인,설정하는 명령어로 net-tools 패키지 설치 후 확인한다.
