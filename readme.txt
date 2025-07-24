git 사용법을 위한 첫 번째 예제
1. git에 추가할 폴더에서 마우스 오른쪽 버튼을 눌러 "Open Git Bash here" 선택(없으면 맨 아래에 추가옵션 표시 선택하면 나타남)
2. Bash창이 뜨면 $ 커서에서 git init 입력(git 폴더 초기화 .git 폴더가 만들어짐)
3. git add 파일명 (파일을 git에 추가하여 첫 번째 버전을 만든다.)
4. git commit -m "추가할 설명을 여기에 적음" (해당 파일의 첫 커밋으로 설명을 추가함)
5. git add 파일명 (파일에 내용을 추가하고 다시 add를 하면 두 번째 버전이 저장됨)
6. git commit -m "새로운 설명 추가" (두번째 버전에 설명을 추가함)

git 사용법 2단계(원격저장소로 올리기)
1. gitHub에 원격저장소(레포지토리:repository)를 만든다.
2. 원격저장소의 주소를 복사
3. Bash 창에서 원격저장소를 지정
   $ git remote add origin 원격저장소주소 (마우스 오른쪽 버튼을 눌러서 paste 선택. ctrl-v 아님)
4. 브랜치(branch) 생성
   $ git branch -M main
5. 로컬의 커밋들을 원격저장소로 올림
   $ git push origin main
6. 브라우저에서 gitHub 로그인 과정을 거치면 로컬 내용이 원격저장소로 복사됨

git 사용법 3단계(원격저장소 내려받기)
1. 로컬에 새로운 폴더 생성하고 해당 폴더에서 Bash 실행(마우스 오른쪽 버튼)
2. gitHub의 원격저장소로 가서 Code 탭에서 주소를 복사
3. 원격저장소 내용을 내려받음
   $ git clone 원격저장소주소
4. 파일을 열어서 내용 추가
5. git 버전 추가
   $ git add 파일명
6. 추가된 내용에 대해서 커밋 추가
   $ git commit -m "추가된 내용 설명"
7. 원격저장소에 푸시
   $ git push origin main
