<h1>오시영</h1>
<h2>6주차 2023-04-06</h2>
<h3>1.컴포넌트 추출</h3>

    - 복잡한 컴포넌트를 쪼개서 여러개의 컴포넌트로 나눌 수 있다.
    - 큰 컴포넌트에서 일부를 추출해서 새로운 컴포넌트를 만드는 것이다.
    - 실무에서는 처음부터 1개의 컴포넌트에 하나의 기능만 사용하도록 설계하는 것이 좋다.

Comment는 댓글 표시 컴포넌트입니다.
 ```js
    function Avatar(props){
        return(
            <img className="avatar"
                src={props.user.avatarUrl}
                alt={props.user.name}
            />
        )
    }
```
가독성이 높아진다
```js
function Comment(props){
    return(
        <div className = "comment">
            <UserInfo user={props.author}>
            <div className="comment-text">
                    {props.text}
            </div>

            <div className="comment-date">
                    {formatDate(props.date)}
            </div>
        </div>
    )
}
```
<h3>생명주기에 대해 알아보기</h3>

    - 생명주기는 컴포넌트의 생성시점, 사용시점, 종료시점을 나타내는 것입니다.
    - constructor가 실행 되면서 컴포넌트가 생성됨
    - 생성 직후 componentDidMount() 함수가 호출됩니다.
    - 컴포넌트가 소멸하기 전까지 여러번 렌더링 한다.
    - 렌더링은 props, setState(), forceUpdate() 에 의해 상태가 변경되면 이루어짐.
    - 렌더링이 끝나면 componentDinUpdate() 함수가 호ㅊㄹ됩니다.
    - 마지막으로 컴포넌트가 언마운트 되면 conponentWillUnmount() 함수가 호출됨.

<h2>5주차 2023-03-30</h2>
<h3>1.엘리먼트?</h3>

    엘리먼트의 정의
        - 엘리먼트는 리액트 앱을 구성하는 요소

    자바스크립트 객체의 형태 
        - 내부의 모든 children을 포함하는 일반 JS객체
        - 불변성을 갖고 있다.

<h3>2.컴포넌트</h3>

    리액트 컴포넌트
    속성들을 입력받아 알맞은 리액트 엘리먼트를 생성하여 리턴해주는것

<h2>4주차 2023-03-23</h2>

<h3>1. 파일 백업</h3>

<h3>2. jsx</h3>

    jsx?
        -자바스크립트의 확장 문법
    jsx의 장점
        -코드 간결화
        -가독성 향상
        -해킹을 방어해 보안성 상승
    jsx의 사용법
        -모든 자바스크립트 문법 지원
        -XML,HTML 둘다 사용
<h2>3주차 2023.03.16</h2>
<h3>1. Node.js와 npm설치후 버전 확인</h3>

    node --version
<h3>2. chocolatey 활용 방법</h3>

    choco search ....
        - 초코레이트에 저장된 패키지를 검색하고 보여준다.
    choco install ....
        - 초코레이트에 저장된 패키지를 검색후 설치한다.

<h3>3. 리액트</h3>

    리액트의 정의 
        -사용자 인터페이스를 만들기 위한 자바스크립트 라이브러리

    리액트의 개념
        - 복잡한 사이트를 쉽고 빠르게 만들고 관리한기 위해 만들어진것
        - SPA를 쉽고 빠르게 만들 수 있도록 해주는 도구

    리액트의 장점
        - 빠른 업데이트와 렌더링 속도
        - 활발한 지식 공유& 커뮤니티

    리액트 단점
         - 방대한 학습량
         - 높은 상태관리 복잡도

<br>
<h2>2주차 2023-03-16</h2>

    Node.js, npm 설치
<h2>1주차 2023-03-09</h2>

    Git 연결 및 커밋 푸쉬와 풀 기본


