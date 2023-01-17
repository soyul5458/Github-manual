## git bash 사용법

### 초기 설정

------

1. **git bash 다운로드**

 https://gitforwindows.org/ 



2. **change directory** 

```
ls
dir
cd Documents
pwd
```



3. **git 최초 설정 (git config)**

```
git config --global user.name "username"
git config --global user.email "email"
```



4. **git clone**

   이렇게 하면 Dpcuments 파일 안에 CAU_ET라는 폴더 생긴다.

```
git clone "https://github.com/ikwak2/CAU_ET"

ls
```



### Github에 파일 올리기 

------

1. 먼저 올릴 파일을 Documents-CAU_ET 파일에 옮겨 놓는다.

   

2. git bash

```
## change directory
cd Documents/CAU_ET

## 깃허브 변경내역 내 컴퓨터로 불러오기
git pull

## 파일 올리기 
git add 폴더이름/파일이름.형식
ex)git add yr19/Readme.md >> yr19라는 폴더에 Readme.md 라는 파일을 올리겠다.

## 변경 내역에 관한 기록
git commit -m "message"
ex) git commit -m "update"

## 깃허브에 올리기
git push

## 깃허브가서 올라갔는지 확인해보기
```

ex) git commit -m "Update R_setup.txt"<img src="C:\Users\dd\AppData\Roaming\Typora\typora-user-images\image-20200110235230754.png" alt="image-20200110235230754" style="zoom:80%;" />

### git push/pull 에러 

------
1. Github 로그인
2. 우측 상단 프로필 이미지 클릭 > Settings 클릭
3. 좌측 하단 Demeloper settings 클릭
4. Personal access tokens > Generate new token 클릭
5. New personal access token (classic) 클릭 > **'select scopes'** 에서 'repo' 체크
6. 생성된 토큰 안전한 곳에 저장해두기 (나갔다 들어오면 확인 불가능)
7. pull/ push할 때 복사한 토큰 비밀번호 부분에 붙여넣기     
[참고](https://velog.io/@mgk8609/remote-Password-authentication-is-temporarily-disabled-as-part-of-a-brownout.-Please-use-a-personal-access-token-instead.-%ED%95%B4%EA%B2%B0%ED%95%98%EA%B8%B0)



### 파일 지우고 싶을 때

------

```
git rm 폴더이름/파일이름
```
