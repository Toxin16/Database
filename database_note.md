## 데이터베이스
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

제어어 (DCL) : 
