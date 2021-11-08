# error
resolve error
---

#### npm 설치오류 메세지

#### Error: Invalid hook call. Hooks can only be called inside of the body of a function component. This could happen for one of the following reasons:
1. You might have mismatching versions of React and the renderer (such as React DOM)
2. You might be breaking the Rules of Hooks
3. You might have more than one copy of React in the same app
* react와 react-Dom의 버전차이일 수 있다. update 후 작동됨. 
* npm update --force, 브라우저 쿠키삭제

---

#### ??? is not defined
* import나 선언 실수

---

#### 오타없는데 안됨
* 일단 서버 재시작

---

#### mysql
* mysql이 예기치 않게 종료되었습니다 -> 버전 8.0.22로 
* MySQL PID 파일 생성 에러 -> MySQL 데이터 디렉토리의 소유권 변경 sudo chown -R mysql:mysql /usr/local/var/mysql -> sudo chmod -R 777 /usr/local/var/mysql -> sudo mysql.server start 해결
* mysql localhost 실행시 로딩화면에서 진전없음 -> 삭제 후 localhost실행, config.json파일 비밀번호 재설정 후 해결
* Unknown database '????' -> '????'라는 데이터베이스가 존재하지 않아서 발생되는 오류 -> npx sequelize db:create 해결
* 

---

#### nestJS
* Error: Nest can't resolve dependencies of the RecordImageService (?). Please make sure that the argument RecordRepository at index [0] is available in the RecordImageModule context. -> index[0] 위치의 Clsex--Repository가 Module 에서 사용가능한지 확인한다. -> constructor 내부에 첫번째로 주입된 Repository 를 가리킨다. 해당 레포지토리를 module 에서 사용하려면 module 내부에서도 레포지토리를 주입해야 한다.
