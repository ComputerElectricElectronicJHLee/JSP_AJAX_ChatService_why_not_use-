# JSP_AJAX_ChatService
동빈나님의 JSP AJAX 유튜브 강의를 바탕으로 한 채팅 서비스 개발 (영상에 없는 기능 추가 및 수정)

[사용 기술]
- Java
- JSP
- AJAX
- HTML/CSS/Javascript
- MySQL
- Bootstrap

[영상에 없는 기능]
- 회원가입 시 중복되는 id일 경우 회원가입 실패 처리
- 오후 12시가 오전 12시로 표기되는 오류 수정
- 모든 페이지에 동일한 네비게이션 바 적용
- 메시지 전송 시 즉시 채팅창 갱신 기능 적용(기존 딜레이 문제 해결)
- 프로필 사진 업로드 시 사진 첨부를 하지 않고 수정 버튼 클릭 시 경고창 팝업 기능 추가

[세션 값 검증 오류 해결]
- JSP에서 encodeURIComponent를 통해 전달되는 데이터들을 고려해야함
- 회원 정보 수정 및 채팅 이용 등 기능을 인가된 사용자 본인만 이용하기 위한 세션 값 검증에서 인코딩된 전달 값과 getParameter 값을 비교하는 과정에서 오류 발생
- URLDecoder를 통해 인코딩된 값을 디코딩하여 getParameter값을 비교함으로써 문제 해결

[느낀 점]
- JSP의 정의 : HTML코드안에 JAVA 문법을 사용하여 웹 페이지를 동적으로 생성하는 방식 (역할이 분할되지 않음)
- 데이터 관리 및 뷰 렌더링 역할도 하다보니 코드가 방대해져서 유지보수가 수월하지 않음
- 이전 게시판 개발 공부 당시 스프링에서 MVC 패턴을 사용하여 이러한 문제를 개선할 수 있구나 느낌

[메인 페이지]
![image](https://user-images.githubusercontent.com/101415950/181293729-ab2f331a-a539-4e9c-9db7-84c7673e033c.png)

[로그인 페이지]
![image](https://user-images.githubusercontent.com/101415950/181293823-925c1863-aee5-4d62-8aeb-76f3372d9180.png)

[회원가입 페이지]
![image](https://user-images.githubusercontent.com/101415950/181293889-569caba2-f464-4d78-b22a-caf5431c0737.png)

[이용자 찾기 페이지]
![image](https://user-images.githubusercontent.com/101415950/181294049-66c99c11-db00-4bff-9849-1ec4963a396b.png)

[메시지 함 페이지]
![image](https://user-images.githubusercontent.com/101415950/181294106-33070e9f-705b-49e8-8344-baa2380244de.png)

[채팅창 페이지]
![image](https://user-images.githubusercontent.com/101415950/181294165-ff305e58-a875-4d98-94f5-b384d91a18e8.png)

[회원정보 수정 페이지]
![image](https://user-images.githubusercontent.com/101415950/181294255-6a43a2fb-15db-4119-9735-d5574807d2b2.png)

[프로필 사진 수정 페이지]
![image](https://user-images.githubusercontent.com/101415950/181294328-25ea00bb-bb9f-4d38-b800-e312cce1dde7.png)
