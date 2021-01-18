# SQL 이란?
**S** TRUCTURED <br>
**Q** UERY <br>
**L** ANGUAGE <br>
관계형 데이터베이스 관리 시스템의 데이터를 관리하기 위해 설계된 특수 목적의 프로그래밍 언어 <br>

## MySQL Syntax
* 데이터 베이스 생성 <br>
```CREATE DATABASE [database name] CHARACTER SET [character set];``` <br><br>
* 데이터 베이스 선택 <br>
```USE [database name];```
<br><br>
* 데이터 베이스 삭제 <br>
```DROP DATABASE [database name];```
<br><br>
* 테이블 생성 <br>
```CREATE TABLE [table name] ([column1 name][datatype], …);``` <br>
``` sql
예시)
CREATE TABLE TOPIC2(
ID INT(11) NOT NULL AUTO_INCREMENT, //  AUTO_INCREMENT : id의 값을 자동으로 +1 시켜줌 
TITLE VARCHAR(100) NOT NULL,
DESCRIPTION TEXT NULL, 
CREATED datetime not null, 
AUTHOR VARCHAR(30) NULL, 
PROFILE VARCHAR(100) NULL, 
PRIMARY KEY(ID) // primary key : 기본키 
);
```
* 테이블 보기 <br>
```SELECT * FROM [table];``` 
<br><br>
* 테이블 삭제 <br>
```DROP TABLE [table name];``` 
<br><br>
* 테이블에 레코드(행) 추가 <br>
``` INSERT INTO [table name] VALUES (value1, value2, value3…); ``` <br><br>
* 테이블의 레코드(행) 내용 수정 <br>
```UPDATE [table] SET [column]=[value] WHERE [condition];``` 
<br><br>
* 테이블의 레코드(행) 삭제 <br>
```DELETE FROM [table] WHERE [condition];``` 
<br><br>