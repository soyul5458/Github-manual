## [Github 사용방법]

*push 전엔 pull을 사용해야 함*  
*한번 설정한 폴더는 1번과 2번을 다시 수행할 필요 없음*  

### 파일 올리는 방법  

1. 컴퓨터 내에 폴더를 만들기  
(C:\Users\000)


2. 폴더 선택 후 오른쪽 마우스 클릭하여 git bash here 선택  
    * git init : initialized 초기화  
    * git remote add origin "github 폴더 주소 넣기" : github와 연결하기  


3. 메모장에 파일을 생성하여 해당 폴더에 저장  
    * git status : github과 git의 상태 확인(git diff, git log = 변경된 사항이 있는지 확인)  
    (*만약 untracked files:에 빨간색 글씨가 뜬다면 아직 remote repository에 upload 되지 않았다는 뜻*)  
    * git add . : 변경된 파일을 모두 tracking  
    * git commit -m "commit할 메세지 추가하기" : history가 남으므로 간결하고 강력하게 기록할것  
    (*commit이란 파일의 수정이 끝났다는 의미로 로컬저장소에 저장하는것*)  
    * git push origin master : 폴더(local staged)에 저장된 파일을 원격 저장소 github에 올리기  
  
### 파일 다운받는 방법(github에 있는 파일 다운받기)  

1. 위와 동일  
2. 위와 동일  
3. git pull origin master : 컴퓨터 상으로 파일 다운로드됨  
  
#### 파일 내용 수정하기(수정방법 2가지)  
1. 컴퓨터상에 있는 폴더에서 데이터를 수정  
    1) 직접 데이터를 수정  
    2) 폴더 선택후 오른쪽 마우스 -> git bash here 클릭  
    - git status    
    - git adad . : 변경된 파일 tracking하기  
    - git commit -m "second commit" : "큰따옴표 안에 내용은 github에 표시되는 메세지이다."  
    - git push origin master  
    
  
2. github 웹상에서 직접 수정  
    1) 웹상에서 연필모양 클릭후 직접 수정  
    2) 그결과, 컴퓨터에 기록된 데이터와 상이. 따라서 두개를 연결시켜야 함.  
    - git pull origin master : 웹상에 수정된 데이터를 다운받으면 컴퓨터상의 데이터도 업데이트 됨.  

________________________________________________________________

## [MarkDown 사용방법]  

### MarkDown이란?
> 웹상에서 글을 쓰는 모든 사람들을 위한 글쓰기 도구(서식, 포맷, 양식) 입니다. *[참조](https://thisblogbusy.tistory.com/entry/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4Markdown-%EC%9D%B4%EB%9E%80)*  
> github, jupyter notebook 등에서 사용

자세한 사용방법은 [여기](https://heropy.blog/2017/09/30/markdown/)를 클릭하시어 참조하시길 바랍니다.

### * 그림(Images)  

![markdown](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg "markdown images")

![github][logo]

[logo]: https://medium.com/comparethemarket/three-quick-tips-to-make-your-github-repository-more-contributor-friendly-47c2db522fe6 "github logo"


### * 표(Table)  

```markdown
|값|착용|미착용|계|
|---|:---:|:---:|---:|
|남|<center>20</center>|<center>40</center>|<center>60</center>|
|여|<center>30</center>|<center>10</center>|<center>40</center>|
|계|<center>50</center>|<center>50</center>|<center>100</center>|
```

|값|착용|미착용|계|
|---|:---:|:---:|---:|
|남|<center>20</center>|<center>40</center>|<center>60</center>|
|여|<center>30</center>|<center>10</center>|<center>40</center>|
|계|<center>50</center>|<center>50</center>|<center>100</center>|

*[참조]마크다운 테이블을 만드는데 아주 유용한 사이트 : [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)*  


### * 블록(block) 코드 강조  

`를 3번 이상 입력하고 코드 종류를 작성  


``` python
print(hello world)
```


*********************

## [READ.ME 사용방법]  

### README란?  
> read.me 파일은 보고서와 같다.  
> 어떠한 목적으로 개발이 되었는지. 코드의 개요, 구조도 등을 사람들에게 노출해 해당 프로젝트에 대한 설명을 기록.  
> markdown을 사용하여 작성  

리드미 파일은 관련 내용을 필수 명시해야 한다.  
- 프로젝트명  
- 프로젝트 소개  
- 설치 방법  
- 사용 예제  
- 개발환경 설정방법
- 저작권 및 사용권 정보
- 등등
