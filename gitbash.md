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



### 파일 지우고 싶을 때

------

```
git rm 폴더이름/파일이름
```
