# 실습 진행 기록

## 2026-11-03 실습 기록



### 1. Git Bash 기본 명령어

- pwd: 현재 위치 확인

- ls -a: 숨김 파일을 포함한 목록 확인

- cd: 폴더 이동

- mkdir: 폴더 생성

- touch: 빈 파일 생성

- cp: 파일 복사

- mv: 파일 이동 및 이름 변경

- rm: 파일 삭제

- cat: 파일 내용 확인

- echo: 파일에 내용 쓰기 및 추가



### 2. Docker 및 Ubuntu 환경 확인

- Docker 버전 확인: 29.9.2

- Docker 서버 정상 실행 확인

- Ubuntu 컨테이너 실행 성공



### 3. Linux 파일 및 폴더 권한 실습

- 파일 permission.txt 권한 확인 및 변경

- 파일 권한: 644 → 755 → 644

- 폴더 permission-dir 생성 및 권한 확인

- 폴더 권한: 755 → 700



### 4. 실습 결과

- Linux의 chmod 명령어로 파일 및 폴더 권한 변경 성공

- ls -l 및 ls -ld 명령어로 변경 결과 확인

- Git Bash와 Ubuntu 컨테이너의 환경 차이 확인


### 5. 새 PC에서 Git Bash 기본 명령어 재실습 (2026-11-03)

- pwd: 현재 작업 위치 확인
- ls: 파일 및 폴더 목록 확인
- ls -a: 숨김 파일 및 폴더 확인
- cd: Desktop 및 mission-practice 폴더 이동
- mkdir: mission-practice 및 storage 폴더 생성
- touch: hello.txt 파일 생성
- echo: 파일에 내용 작성 및 추가
- cat: 파일 내용 확인
- cp: hello.txt 파일 복사
- mv: 복사한 파일 이름 변경
- rm: 이름을 변경한 파일 삭제
- 실습 결과를 practice/git-bash-practice.txt에 별도 저장

### 6. 새 PC에서 Docker 기본 실습 (2026-11-03)

- Docker 버전 29.9.2 확인
- docker run hello-world 실행 및 성공 메시지 확인
- Ubuntu 컨테이너 실행 후 pwd 명령어 확인 및 종료
- docker images로 이미지 목록 확인
- docker ps 및 docker ps -a로 컨테이너 상태 확인
- docker logs로 hello-world 실행 로그 확인
- docker stats --no-stream으로 컨테이너 자원 사용량 확인
- mission-practice-ubuntu 컨테이너 생성 및 실행 상태 확인
- docker exec로 실행 중인 컨테이너 내부 접속
- docker attach로 컨테이너 접속 후 Ctrl+P, Ctrl+Q로 분리

### 7. Dockerfile을 이용한 사용자 정의 이미지 제작 (2026-11-03)

- practice/dockerfile/Dockerfile 직접 작성
- Ubuntu latest 이미지를 기반 이미지로 지정
- CMD 명령어로 사용자 지정 메시지 출력 설정
- docker build -t mission-practice:1.0 실행하여 이미지 생성
- docker images로 생성된 이미지 확인
- docker run --rm mission-practice:1.0 실행
- "Hello from my custom Docker image!" 출력 확인
