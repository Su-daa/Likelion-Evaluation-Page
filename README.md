# LikeLionHomework 7/13

## 개요

서버에서 받아온 데이터들을 Redux를 이용하여 관리하는 상황을 가정했습니다. src 폴더의 store.js에 데이터들을 저장했습니다. 그냥 연습 겸 한 번 써봤습니다. 지금 저장해 놓은 데이터는 저희가 썼던 명세서와 하단에 백엔드에서 첨부한 사진을 바탕으로 임의로 작성해 보았습니다. 추후에는 직접 받아와서 사용하게 되겠지요.<br>

Home컴포넌트의 이름이 Lecture가 더 어울릴 것 같아 임의로 변경해 보았습니다.

## \<Lecture>

서버로부터 강의고유id, 강의명, 교수명, 과목번호 를 받아온 것으로 내용을 구성합니다. 별점은 지금은 사용하지 않는 것으로 얘기가 나왔지만 일단 적어는 놓았습니다.<br>

마이페이지에는 로그인 시 제공받는 자신의 강의가 담긴 배열에, 메인페이지에는 추천강의가 담긴 배열에 map함수를 사용하여 구현했습니다.<br>

상세보기 버튼에는 해당 강의의 고유 id를 url 파라미터로 넘겨 상세페이지로 라우팅합니다.

## 상세페이지 (\<Evaluation>)

url 파라미터를 뭘로 해야할까 고민하다가 해당 강의의 고유id를 사용하면 어떨까 생각해 보았습니다.
useParams로 파라미터로 사용했던 해당 강의의 고유id를 받아옵니다.<br>

내 강의, 추천 강의, 검색한 강의들 중에서 고유id가 매칭되는 강의를 찾아서 해당 내용으로 페이지를 구성했습니다.<br>


## 마이페이지

노션에 첨부된 사진에서는 로그인시 제공되는 lecture 항목이 빠져있는데 아마 추후에 만들어주지 않을까요? 아무튼 로그인 시 받아오기로 했던 정보들을 userInfo에 넣어보았습니다.<br>

백엔드에서 첨부해주신 사진에 나온 유저정보로 구성했습니다. 심리학과래요.<br>

그러고 나서 같은 방식으로 state를 참조해서 구성하였습니다.



