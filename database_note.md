## 데이터베이스
cls 터미널 지우기
C:\laragon\bin\mysql\mysql-5.7.33-winx64\bin>
mysql -u root -p (enter), root password 없음
show databases; //데이터베이스 목록출력, show tables; //테이블 출력, desc fruit; //fruit table 목록출력
use goods;  //데이터베이스의 목록의 goods 사용
insert into fruit values ('Apple', 10, 'Red', 'Korea');

ctrl + c : 작업취소
용어
원소 하나 : data / 원소의 모임 : 필드 / 서로 연관성이 있는 필드의 묶음 : record / 전체 : table
데이터베이스에는 여러 테이블이 있을 수 있음. 

### php db 연동
$conn = mysqli_connect('localhost', 'root', '', 'goods'); 

221109
정의어(DDL) : 데이터베이스에 들어 있는 데이터를 조회하거나 검색하기 위한 명령어를 말하는 것. CREATE TABLE //생성, ALTER TABLE //변경, DROP //삭제

조작어(DML) : 테이블과 같은 데이터 구조를 정의하는데 사용되는 명령어들로 (생성, 변경, 삭제, 이름변경) 데이터 구조와 관련된 명령어들을 말함. select(검색), update(수정), insert(삽입), 삭제(delete)

relation : 2차원의 테이블(스프레드 시트와 유사)
record : 릴레이션의 각 행
tuple : 레코드를 공식적으로 부르는 용어
attribute : 릴레이션에서 이름을 가진 하나의 열

대체 키 : 기본키로 선정되지 않은 후보 키
외래 키 : 어떤 다른 릴레이션의 기본키를 참조하는 애트리뷰트, 릴레이션들간 관계를 나타내기 위해 사용. 릴레이션의 기본키와 동일한 도메인을 가져야함. 자신이 속한 릴레이션의 기본키의 구성요소가 되거나 되지 않을수 있음.

laragon, xampp, wampp, autoset
데이터베이스 쿼리를 php에서도 그대로 적용가능
