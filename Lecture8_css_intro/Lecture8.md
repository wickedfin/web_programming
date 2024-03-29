# Lecture 8

## CSS란?
- Cascading Style Sheets의 줄임말로 웹페이지에서 HTML를 꾸며주는 역할을 한다
- CSS의 기본구조는 선택자와 명령문으로 이루어진다
    - 선택자: CSS를 적용할 영역 선택
    - CSS 명령문: CSS 속성과 값을 입력하는 부분

## CSS를 삽입하는 방법들
1. Inline style: HTML 문서 안에서 줄에서 간단하게 입력하는 방법
    - 권장하지 않음
2. 내부 스타일 시트 style: CSS 코드를 HTML 문서의 style 태그 안에 써주는 방식
    - 하나의 HTML에서만 작동한다
3. 외부 스타일 시트 style: CSS 파일을 별도로 분리한 뒤, HTML에서 링크로 참조하는 방식
    - 권장하는 방식

## 기본 선택자
- 전체 선택자 `*`: HTMl 태그에 있는 모든 요소를 선택
    > 주로 글씨체나 글자 크기를 위해 사용
- 태그 선택자 `태그명`: HTML 내부의 특정태그를 선택
- 아이디 선택자 `#아이디`: 특정 id 속성에 있는 태그 선택
    > HTML 내부에 id 값은 중복되면 안된다 
- 클래스 선택자 `.클래스명`: 특정 클래스가 있는 태그들을 선택
- 다중 선택을 할 때는 `쉼표`로 이어준다

## 속성 선택자
- 선택자에 해당하는 속성 값을 필터링하여 선택해낸다
~~~css
input[type]{color: blue;}
input[type="password"]{color: red; font-size:23px;}
~~~

## 하위레벨 선택자
- `선택자A 선택자B`: 후손 선택자로 직속이 아니어도 됨
- `선택자A > 선택자B`: 자손 선택자로 직속만 선택 가능
- 참고로 테이블 태그에서는 이러한 하위레벨 선택자를 잘 사용하지 않는다

## 반응 & 상태 선택자
- `:active`: 사용자가 마우스로 클릭한 태그
- `:hover`: 사용자가 마우스 커버를 올린 태그
- `:checked`: 체크가 되어있는 상태의 input 태그
- `:focus`: focus 되어있는 input 태그
- `:enabled`, `:disabled`: 사용 가능/불가능 input 태그
    > disabled="disabled" 라는 속성을 추가해서 사용할 수 있다

## 구조 선택자
- 형제 관계에서의 선택을 할 수 있다
- `:first-child`: 첫번째 태그
- `:last-child`: 마지막 태그
- `:nth-child(수열)` & `:nth-last-child(수열)`: 형제 관계에서 수열로 선택 가능


> CSS 강의 시작, 11강의 내용임