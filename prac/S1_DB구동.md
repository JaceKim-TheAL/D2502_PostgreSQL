# PostgreSQL 기본구동

1. <b>DB구동 및 종료                 </b>
2. [DB접속 및 데이터베이스와 사용자 생성](./S2_사용자생성성.md) 
3. [사용자계정 접속으로 Table 생성     ](./S3_테이블생성.md)
4. [Data CRUD 명령                  ](./S4_데이터CRUD.md)
5. [DB 백업 및 복구                  ](./S5_백업및복구.md)

---

1. DB구동 및 종료
```
Run run 'pg_ctl start' or 'pg_ctl stop' to start and stop the database or
register it as a service by running 'pg_ctl register -N PostgreSQL' from an elevated shell.
Default superuser login: postgres, password: <blank>
```

- 구동 : `pg_ctl start`
- 중지 : `pg_ctl stop`
- 등록 : `pg_ctl register -N PostgreSQL`
- 관리자 : pgAdmin4 실행 <br/> 
  `윈도우 돋보기에서 pgAdmin4 검색 후 클릭`
- Tip. 설치후 바로 구동하면 안되는 경우, 새로운 Command 창을 띄우고 실행하면 된다.
<br/>
<br/>
