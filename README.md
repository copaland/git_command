# hello-world
github 공부용

1.GitBash 설치
 https://gitforwindows.org
 다운로드 설치
 
2.Github 가입
https://github.com
New Repository 생성

3.Root Folder 연결
 Web상의 Git과 연결될 Local Folder에서 마우스 RMB <git bash here>
 $git init
 $git remote add origin <repository address>
 $git remote add origin https://github.com/copaland/hello-world.git

4.Push전에 Pull
 $git pull origin master ; 지정한 Repository에서 끌어 온다.
 
 <push>
 $git status ; 현재 git과의 상태를 체크
 $git add . ; 변경된 파일들을 모두 Tracking
 $git commit -m "message" ; 인식할 수 있는 "내용" 커밋을 달아 줍니다.
 $git push origin master ; 실제로 git에 PUSH
