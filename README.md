# git 명령어

github 공부용

1. Git for Windows 설치<br/>
 https://gitforwindows.org 에서 다운로드 설치<br/>
 Git BASH / Git GUI<br/>
 
2. Github 가입<br/>
https://github.com
New Repository 생성

3. Root Folder 연결<br/>
 Web상의 Git과 연결될 Local Folder에서 마우스 RMB <git bash here> <br/>
 ```
 $git init<br/>
 $git remote add origin <repository address><br/>
 $git remote add origin https://github.com/copaland/hello-world.git<br/>
```
 > init ; 현재 폴더를 로컬 저장소로 지정
 > remote add ; 로컬 저장소와 원격 저장소를 연결시킨ek.
 > abc.git ; Github 저장소 주소  
 > origin ; 별칭 
 
4. Push전에 Pull<br/>
 ```
 **푸시**<br/>
 $git pull origin master ; 지정한 저장소 내용을 로컬에 끌어 온다.<br/>
 
 **풀**<br/>
 $git status ; 현재 git과의 상태를 체크<br/>
 $git add . ; 변경된 파일들을 모두 Tracking<br/>
 $git commit -m "메세지" ; 인식할 수 있는 "메세지" 커밋을 달아 줍니다.<br/>
 $git push origin master ; 실제로 git 저장소에 올린다<br/>
```
 > add ; 작업 공간의 파일들을 준비 영역에 추가
 > commit ; 로컬 저장소에 최종 저장하는 단계
 > $git push origin https://github.com/copaland/hello-world.git
 
5. 기타<br/>
 
별칭 내역을 확인   
origin의 별칭으로 등록된 원격 저장소를 확인할 수 있다.  
```
git remote -v  
```
만약 pull을 해줬음에도 불구하고 에러가 발생할 경우 강제로 push하는 명령어는  
```
git push origin +master  
```

commit 간에 파일의 바뀐 내용을 보여줌  
```
 git log -p
```

로그 읽는법  
+: 추가 또는 바뀐 내용,  
-: 이전 내용  

commit 간의 소스코드 차이를 보여줌   
git diff 커밋ID1..커밋ID2  
```
 diff --git a/test.txt b/test.txt
```
 ;a는 이전 버전이라는 의미하고 b는 현재 버전을 의미
 
