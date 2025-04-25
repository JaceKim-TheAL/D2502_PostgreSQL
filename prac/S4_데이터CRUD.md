# PostgreSQL 기본구동

1. [DB구동 및 종료                   ](./S1_DB구동.md) 
2. [DB접속 및 데이터베이스와 사용자 생성](./S2_사용자생성성.md) 
3. [사용자계정 접속으로 Table 생성     ](./S3_테이블생성.md)
4. <b>Data CRUD 명령                 </b>                    
5. [DB 백업 및 복구                  ](./S5_백업및복구.md)
---

4. Data CRUD 명령
- 테이블 조회
```
test_db=> \d
                    릴레이션 목록
 스키마 |         이름          |  형태  |  소유주
--------+-----------------------+--------+-----------
 public | tb_admin              | 테이블 | test_user
 public | tb_admin_admin_no_seq | 시퀀스 | test_user
(2개 행)

```

- 데이터 등록
```
test_db=> INSERT INTO TB_ADMIN(LOGIN_ID, PASSWD, NICK, EMAIL)
      VALUES('hong_gd', 'hong123', '홍길동', 'hong@gmail.com');
INSERT 0 1

test_db=> INSERT INTO TB_ADMIN(LOGIN_ID, PASSWD, NICK, EMAIL)
      VALUES('jang_nr', 'jang123', '장나라', 'jang@gmail.com');
INSERT 0 1

```
- 데이터 조회
```
test_db=> SELECT * FROM tb_admin;
 admin_no | login_id | passwd  |  nick  |     email
----------+----------+---------+--------+----------------
        1 | hong_gd  | hong123 | 홍길동 | hong@gmail.com
        2 | jang_nr  | jang123 | 장나라 | jang@gmail.com
(2개 행)

```
- 데이터 수정
```
test_db=> UPDATE TB_ADMIN SET NICK='홍길똥' WHERE LOGIN_ID='hong_gd';
UPDATE 1
test_db=> UPDATE TB_ADMIN SET NICK='짱나라' WHERE LOGIN_ID='jang_nr';
UPDATE 1
test_db=> SELECT * FROM TB_ADMIN;
 admin_no | login_id | passwd  |  nick  |     email
----------+----------+---------+--------+----------------
        1 | hong_gd  | hong123 | 홍길똥 | hong@gmail.com
        2 | jang_nr  | jang123 | 짱나라 | jang@gmail.com
(2개 행)

```
- 데이터 삭제
```
test_db=> DELETE FROM TB_ADMIN WHERE LOGIN_ID='hong_gd';
DELETE 1
test_db=> SELECT * FROM TB_ADMIN;
 admin_no | login_id | passwd  |  nick  |     email
----------+----------+---------+--------+----------------
        2 | jang_nr  | jang123 | 짱나라 | jang@gmail.com
(1개 행)

```
