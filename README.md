## <img  src="kakaotalk_logo_round.png"  width='20'  height='20'> alone_kokoaclone

카카오톡을 클론코딩하여 HTML과 CSS 학습을 진행합니다.

## HTML

1. HTML의 목적: **브라우저에게 구조를 알려준다**.
   <br/>

2. tag를 이용하여 요소를 삽입한다.
   <br/>

3. HTML 특징 - 잘못된 태그: **오류가 발생하지 않는다.** - 태그 안 attribute: 태그에 추가적인 정보를 주는 요소. 마찬가지로 **잘못된 attribute를 사용해도 오류가 발생하지 않는다**. - Self-Closing Tag: 닫는 태그가 없는 태그. **attribute가 태그의 내용이 되므로** 열고 닫는 태그 사이에 text를 넣을 필요가 없음.
   <br/>

4. < !DOCTYPE html > : 브라우저에게 해당 문서가 html code를 갖는다는 것을 알려준다.
   <br/>

5. head 는 웹페이지의 부가적인 설정을 정의한다. - meta: 사람의 눈에 보이지 않는 태그 (부가적인 정보). - 특히 < meta charset="utf-8" /> 태그는 글자의 포맷을 지정해주기 때문에 중요하다. - < Link rel="이름" href="아이콘 사진 링크" /> 를 넣으면 페이지 탭의 아이콘을 지정할 수 있다.
   <br/>

6. html 작성 시 유의하면 좋은 점들 - html tags 서치 시 mdn 붙여서 찾기 -> 외우지 말고 찾아서 확인하면 좋음! - html 문서를 작성할 때는 semantic tags (보자마자 의미를 유추할 수 있는 태그들) 를 사용하는 것이 좋다
   <br/>

7. id - id는 유일해야하고, 태그는 id를 갖지 않거나 오직 한 개만 갖는다. - body에도 id를 부여할 수 있다.
   <br/>

## CSS

1. CSS의 목적: 스타일링
   <br/>

2. CSS를 HTML에 추가하는 방법

   1. HTML과 CSS코드를 한 파일에 작성하기: HTML 코드에 <style> </style> 태그를 입력한다.
   2. HTML 코드와 CSS 파일을 분리하기: CSS 파일을 만든 뒤 `<link href="스타일.css 파일 이름" rel="stylesheet" />`를 입력한다.

3. CSS를 작성할 때

   1. style을 넣고자 하는 HTML 태그의 이름을 작성한다.
   2. 중괄호에 원하는 스타일 내용을 넣는다.

   ```css
   h1 {
     color: red;
     font-size: 20px;
   }
   ```

   3. BEM - 클래스 이름 짓는 방법

      1. class__안의정보
      2. class--modifier

4. 브라우저는 CSS 파일을 위에서부터 아래로 순서대로 읽는다. 따라서 동일한 태그를 꾸미는 CSS가 있을 경우, 제일 마지막에 있는 코드가 실행된다.

5. Blocks(box) and Inlines

   1. Blocks 특징을 갖는 태그들은 옆에 다른 요소가 올 수 없다.

   2. Inlines 특징을 갖는 태그들은 옆에 다른 요소가 올 수 있다.

   3. Block 과 Inline 스타일은 display 속성을 이용하면 바꾸기가 가능하다.

   4. Block은 높이와 너비를 가질 수 있고, Inline은 그럴 수 없다.

   5. Block(box)는 margin, padding, border 특성을 갖는다.

   6. Inline은 **margin을 좌우로만 가질 수 있고**, padding과 border 특성을 갖는다. width와 height 속성을 가질 수 없다.

6. Margins

   1. box의 border(경계선)으로부터 바깥에 있는 공간

   2. box에 아무 처리도 하지 않는다면, 브라우저에 의해 자동으로 div박스의 좌측과 위쪽에 빈 공간이 생긴다.

   3. 코드 작성법

      - margin: 20px; //상하좌우 모두 20px씩 생긴다.

      - margin: 10px 20px; // 상하는 10, 좌우는 20px 씩 생긴다.

      - margin: 10px 20px 30px 40px //상 우 하 좌 시계방향

   4. Collapsing Margin

      - 두 요소의 border line이 같다면, margin이 하나로 취급된다. 상하 방향에서만 발생하는 상황이다.

7. Padding: border 안쪽의 공간

8. Border: 아웃라인 (box와 inline 모두 Border를 갖는다)

9. CSS의 Selector 작성 법칙

   1. 일반 Tag 이름: 태그 이름 그대로

   2. Tag의 아이디: #id이름

   3. 전체를 가리킬 때: \*

   4. 여러 개의 아이디를 한꺼번에

      ```css
      #tomato,
      #tomato1,
      #tomato2 {
        background-color: yellow;
      }
      ```

   5. 비슷한 것들을 묶어 클래스로 만들기 가능: .클래스이름

      ```
      .tomato{
         background-color: yellow;
      }
      ```

      - 클래스 이름은 여러 개 가질 수 있다 `<div class="btn tomato">`

   6. div:first-child //: 앞의 태그와 뒤의 자식 번지수는 바꾸기 가능

      div 내에서 첫번째 자식을 선택해 스타일링 가능

   7. span:nth-child(2) // 괄호 안에 들어가는 것이 순서가 됨

      - span들 중 2번째 span을 선택해 스타일링 가능, odd와 even도 가능하다

      - 2n+1 과 같이 일반식으로도 작성 가능하다

   8. Combinators

      - p span {} : p안에서 span을 찾아 스타일링

      - div p span {} : div 안에서 p를 찾고, p안의 span을 찾아 스타일링

      - div > span {} : div 안에서 가장 첫번째로 나오는 자식 (바로 밑 자식)에 스타일링

      - p + span {} : p 바로 다음에 있는, 같은 레벨에 존재하는 span에 스타일링

      - p ~ span {} : 형제관계, 꼭 바로 다음에 오지 않아도 됨. p 다음에 오는 어느위치든 상관없는 span에 스타일링

   9. attribute 선택하기-> tagname:attribute

      - input:required{} -> input form에서 required인 것

      - input:[placeholder~="name"] -> input form에서 placeholder에 name이 포함된 것

10. inline-block

    - div를 양 옆으로 붙일 수 있게 만들어준다.

    - 반응형을 지원하지 않아 모니터 해상도에 따라 화면 구성이 달라보인다. -> 비추천

    - 위와 같은 이유로 flexbox를 사용한다.

11. Flexbox

    - 자식 요소에는 아무것도 적지 않고, 부모 요소에만 적어야 한다

    - main axis / cross axis: flexbox의 주축은 main(justify-content), 교차축은 cross axis(align-items)이다

    - 위의 요소를 쓰고 싶다면, 부모 요소에 반드시 display: flex를 적어야 한다.

    - 주축을 바꾸고 싶다면 flex-direction요소를 사용하면 된다.

    ```css
    flex-direction: row //가로가 주축
    flex-direction: column //세로가 주축
    ```

    - wrap은 화면이 줄어들어서 flexbox의 요소가 겹쳐지는 현상 등을 말하는데, flex-wrap 요소로 제어할 수 있다.

12. position

    - fixed: 를 설정하면 어느 자리에 있든 고정된다. top, bottom, left, right 요소를 수정하면 다른 요소를 무시하고 제일 위에 올라온다.

    - relative: 를 설정하면 기준값이 엘리멘트가 처음 위치한 곳이 되고 top, bottom, left, right 요소를 수정할 수 있다.

    - absolute: 를 설정하면 부모 박스로부터 벗어나 (탈출됨) top/bottom/left/right를 설정할 시 가장 가까이에 있는 relative 부모를 기준으로 맨오른쪽, 왼쪽, 위, 아래로 이동하게 됨. 이런 효과를 막고싶으면 바로 위 부모 요소를 relative로 만든다.

13. States

    - 버튼을 눌렀을 때 색을 지정하는 것 등도 가능하다

    ```css
     {
      /*마우스 클릭할 때*/
    }
    button:active {
      background-color: tomato;
    }
     {
      /*마우스를 올려둘 때*/
    }
    button:hover {
      background-color: tomato;
    }
    ```

    - 사이트에 방문한 기록이 있을 때 색이 변하는 것도 다른 색으로 설정이 가능하다.

    ```css
    a:visited {
      color: tomato;
    }
    ```

    - focus-within은 자식 요소를 클릭했을 때 부모요소에 변화가 생김. 아래의 코드는 form내부의 요소가 클릭되면 form의 테두리가 tomato색이 됨

    ```css
    form:focus-within {
      border-color: tomato;
    }
    ```

    - 이 경우 form에 마우스를 올릴 경우 input의 색이 바뀜

    ```css
    form:hover input {
      background-color: tomatoe;
    }
    ```

14. color

    - colorcode: "#000000"

    - rgb: rgb(252, 206, 0)

    - rgba: rgba(252, 206, 0, 20) //알파값

    - 색깔 이름으로 적기

15. 변수 (custome property)

    ```html
    <style>
      :root {
        --main-color: #fcce00;
        --default-border: 1px solid var(--main-color);
      }

      a {
        color: var(--main-color);
        border: var(--default-border);
      }
    </style>
    ```

## CSS Advanced

1.  Transitions

    - transition은 state가 없는 요소에만 붙이기 가능

    - 마우스 올리면 hover에 정의된대로 바뀌는데, 이때 transition에 적은 속성대로 됨.

    - 따라서! **변화하게 만드는 특징은 state가 있는 부분에, transition은 state가 없는 부분에!!!!** 적어야 한다.

    ```css
    a {
      color: wheat;
      background-color: tomato;
      text-decoration: none;
      transition: background-color 10s ease-in-out;

      /*transition: all 하면 모든 것에 다 바뀜*/
    }

    a:hover {
      color: tomato;
      background-color: wheat;
    }
    ```

2.  Transform

    - 변형시키는 것

    - 다른 요소까지 변화시키지는 않는다.

    ```css
    img{
       border: 10px solid black;
       border-radius: 50%
       transform: rotateY(30deg);
       transform: scale(2,2); //x, y 쪽으로 확대
       transform: tranlateX(-1000px) ;//가로축 -1000px 이동
    }
    ```

    - state와 같이 쓸 수 있다. hover을 하면 transition과 transform이 동시에 적용한다. transition은 root에, transform은 state에 사용가능하다.

    ```css
    img {
      transition: ...;
    }

    img:hover {
      transform: rotateY(90deg);
    }
    ```

3.  Animations

    - 마우스를 올리거나 별다른 이벤트가 없어도 자동으로 애니메이팅이 일어난다.

    ```css
    @keyframes flip {
      from {
        transform: rotateX(0);
      }
      to {
        transform: rotateX(360deg);
      }
    }

    img {
      animation: flip 5s ease-in-out;
    }
    ```
