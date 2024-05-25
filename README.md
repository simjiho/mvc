변수 
int cPage  : 현재 페이지번호를 저장하는 변수
int numPerpage : 페이지당 출력할 데이터수를 저장하는 변수
int totalData : DB에 저장되어 있는 총 row수를 저장하는 변수
int totalPage : 전체 데이터에 대한 페이지수를 저장하는 변수
// 페이지바를 구성하는 변수
int pageNo : 페이지바의 시작번호를 저장하는 변수
	-> ((cPage-1)/pageBarSize)*pageBarSize+1;
int pageEnd : 페이지바의 끝번호를 저장하는 변수
	-> pageNo+pageBarSize-1;
int pageBarSize : 페이지바에 출력된 번호의 갯수를 저장하는 변수

String pageBar : 페이지 번호별 요청태그를 작성해서 저장하는 변수

page 를 요청했을때 numPerpage=5 -> 1~5까지 

데이터의 시작 : (cPage-1)*numPerpage
데이터의 끝 : cPage*numPerPage
