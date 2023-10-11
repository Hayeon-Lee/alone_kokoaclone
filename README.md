## <img  src="kakaotalk_logo_round.png"  width='20'  height='20'> alone_kokoaclone

카카오톡을 클론코딩하여 HTML과 CSS 학습을 진행합니다.

## HTML

1. HTML의 목적: **브라우저에게 구조를 알려준다**.

2. tag를 이용하여 요소를 삽입한다.

3. HTML 특징

- 잘못된 태그: **오류가 발생하지 않는다.**

- 태그 안 attribute: 태그에 추가적인 정보를 주는 요소. 마찬가지로 **잘못된 attribute를 사용해도 오류가 발생하지 않는다**.
- Self-Closing Tag: 닫는 태그가 없는 태그. **attribute가 태그의 내용이 되므로** 열고 닫는 태그 사이에 text를 넣을 필요가 없음.

4. < !DOCTYPE html > : 브라우저에게 해당 문서가 html code를 갖는다는 것을 알려준다.
 
5. head: 웹 페이지의 설정을 정의한다.
- meta: 사람의 눈에 보이지 않는 태그 (부가적인 정보). 
- 특히 < meta charset="utf-8" /> 태그는 글자의 포맷을 지정해주기 때문에 중요하다.
- < Link rel="이름" href="아이콘 사진 링크" /> 를 넣으면 페이지 탭의 아이콘을 지정할 수 있다.

6. body: 웹페이지의 내용을 넣는다.

7. html tags 서치 시 mdn 붙여서 찾기 -> 외우지 말고 찾아서 확인하면 좋음!

8. id
- id는 유일해야하고, 태그는 id를 갖지 않거나 오직 한 개만 갖는다.
- body에도 id를 부여할 수 있다.

9. semantic vs nonsemantic tags
- 태그 자체에 의미가 부여되는 태그와 그렇지 않은 태그이다.
- div는 nonsemantic tags인데, 단순히 구분을 짓는 것이고 header(semantic 태그 중 한 개)는 보자마자 이 코드가 헤더의 역할을 한다는 것을 알 수 있다.
- 코딩을 할 때는 직관적이면서 이해하기 쉬운 코드를 작성할 수 있는 semantic tags 사용을 권장한다.

