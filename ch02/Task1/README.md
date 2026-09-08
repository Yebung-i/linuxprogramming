## 리눅스 명령어가 무엇인지 설명하시오. 또, 실제 명령어의 정체는 무엇인가?
명령어란, 운영체제에 작업을 지시하는 단어로, 실제로는 실행파일의 이름을 뜻한다.
따라서 리눅스 명령어란, 사용자가 리눅스 운영 체제에 특정 작업을 수행하도록 지시하는 명령이며, 실제로는 해당 작업을 수행하는 실행파일을 가리키는 이름이다.

## 리눅스에서 가장 많이 사용되는 명령어 10개를 조사하고 설명하시오. 또 셸에서 실행하고 결과를 첨부하시오.
- ls : 현재 위치의 파일과 폴더 목록을 보여줌
<img width="403" height="87" alt="image" src="https://github.com/user-attachments/assets/a1283cfe-dd21-43f2-9086-1cfed17d88d1" />


- pwd : 현재 작업 중인 폴더의 전체 경로를 보여준다 
<img width="305" height="78" alt="image" src="https://github.com/user-attachments/assets/b0e0a8bb-b378-4b85-a65c-d3f3031557c6" />


- cd : 다른 폴더로 이동한다.
<img width="460" height="70" alt="image" src="https://github.com/user-attachments/assets/282ab845-9f58-4d33-b9c6-3e3c5378bb88" />


- mkdir : 새 폴더를 생성한다. 
<img width="587" height="132" alt="image" src="https://github.com/user-attachments/assets/6880f51e-f9cb-4d45-ad05-9a514e69bd10" />


- mv : 파일이나 폴더를 이동하거나 이름을 바꾼다.
<img width="602" height="227" alt="image" src="https://github.com/user-attachments/assets/7bd08f6d-aa0b-47b1-b50f-f122b59e5e1b" />


- cp : 파일이나 폴더를 복사한다.
<img width="732" height="142" alt="image" src="https://github.com/user-attachments/assets/1abe866c-1a8d-45aa-bfd3-03b9e661441b" />


- rm : 파일이나 폴더를 삭제한다.
<img width="712" height="112" alt="image" src="https://github.com/user-attachments/assets/171d9e35-f537-47ef-b4cd-d6eceb1a0c48" />

- touch : 내용이 없는 빈 파일을 생성하거나, 이미 존재하는 파일의 최종 수정 시간을 현재 시각으로 갱신한다.
<img width="728" height="125" alt="image" src="https://github.com/user-attachments/assets/9294c7c0-d30e-4b01-8154-9b8125e196ef" />


- ln : 파일에 대한 링크를 생성
<img width="707" height="102" alt="image" src="https://github.com/user-attachments/assets/2e9f95d9-4451-4940-83ea-04db860ef973" />


- clear : 터미널 화면에 출력된 내용을 지우고 깨끗하게 정리한다.
<img width="735" height="127" alt="image" src="https://github.com/user-attachments/assets/b0b0595e-064e-4801-afd4-900ce39f5bbd" />
사용 후
<img width="1158" height="257" alt="image" src="https://github.com/user-attachments/assets/69ace6d9-0c25-4211-a50b-204a8bee3201" />



## 셸과 커널을 구분하여 자세히 설명하시오.
- 커널은 운영체제의 핵심으로서, 하드웨어와 소프트웨어 사이에서 직접 자원을 관리하는 부분이다. 하드웨어와 직접 상호작용하며 프로세스, 메모리, 파일시스템 관리 등을 한다.
커널은 사용자가 직접 접근 및 조작할 수 없으며 사용자가 이를 이용할 수 있도록 인터페이스 (셸) 을 제공한다.

- 셸이란 사용자가 커널에 접근할 수 있도록 제공되는 사용자 인터페이스로, 시스템 콜을 통하여 커널과 상호작용하며 간접적으로 이용할 수 있도록 해준다.
이렇게 간접적으로 상호 작용하는 이유는, 커널이 손상되면 시스템 전체가 부팅되지 않거나 심각한 오류가 발생하기에 커널을 셸로 감싸 정해진 규칙을 통해 간접적으로 접근하게 함으로서 커널을 보호하기 위함이다.

## 프롬프트 문자열에서 문자 ~의 의미를 조사하라.
현재 사용자의 홈 디렉토리를 의미한다. 예를 들어, `~/Downloads` 라면, `home/사용자이름/Downloads` 를 의미한다. 

## sh, bash, zsh 셸의 차이를 자세히 조사하시오.
- sh : 1977년 스티븐 본이 개발한 유닉스 최초의 표준 셸로서, 히스토리 기능 및 자동완성 등의 편의성 기능 없이 스크립트 실행을 위한 최소한의 기능만 제공한다. 


- bash : 1989년 브라이언 폭스가 GNU 프로젝트의 일환으로 개발한, sh를 계승하면서 기능을 확장한 셸이다. 명령어 히스토리, 자동완성, 별칭(alias) 등의 작업 제어 등
편의성 기능들이 대거 추가되었다.


- zsh : 1990년 폴 포크맨이 프린스턴 대학교 재학 중 개발한, bash의 기능을 포함하면서 더 강력한 편의성을 더한 셸로서, 오타 교정 제안, 대소문자 무관 자동완성, 재귀적 파일 탐색 같은 확장 글로빙, 여러 터미널 간
히스토리 공유 등을 지원한다.  `Oh My Zsh` 프레임워크를 통해 테마와 플러그인을 손쉽게 적용 가능해 개발자들 사이에서 인기가 높다.

## 셸 스크립트에 대하여 자세히 조사하시오.
셸 스크립트는 리눅스/유닉스 셀 등에서 실행 가능한 명령어들을 순서대로 나열하여 저장한 텍스트 파일이다. 반복적인 작업을 자동화하기 위함이나 여러 명령어를 한 번에 실행하기 위해 작성된다. 

## Windows에서 사용하는 CLI방식의 셸의 종류를 조사하라.
- 명령 프롬프트 (cmd) : MS-DOS 시절부터 이어져 온 Windows의 가장 오래된 CLI 셸이다. <br>
  -> DOS 명령 체계를 기반으로 함 (dir, copy, del, cd 등) <br>
  -> 배치 파일 (.bat, .cmd) 작성 및 실행 가능
    
