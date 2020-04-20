# hello-world
github 공부용

1.Git for Windows 설치<br/>
 https://gitforwindows.org 에서 다운로드 설치<br/>
 Git BASH / Git GUI<br/>
 
2.Github 가입<br/>
https://github.com
New Repository 생성

3.Root Folder 연결<br/>
 Web상의 Git과 연결될 Local Folder에서 마우스 RMB <git bash here> <br/>
 $git init<br/>
 $git remote add origin <repository address><br/>
 $git remote add origin https://github.com/copaland/hello-world.git<br/>

4.Push전에 Pull<br/>
 푸시<br/>
 $git pull origin master ; 지정한 Repository에서 끌어 온다.<br/>
 
 풀<br/>
 $git status ; 현재 git과의 상태를 체크<br/>
 $git add . ; 변경된 파일들을 모두 Tracking<br/>
 $git commit -m "message" ; 인식할 수 있는 "내용" 커밋을 달아 줍니다.<br/>
 $git push origin master ; 실제로 git에 PUSH<br/>
