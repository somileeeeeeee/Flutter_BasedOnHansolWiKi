1. Mysql 홈페이지에서 다운로드 -> 로그인 없이 받기
 https://dev.mysql.com/downloads/file/?id=510039

2. Developer Default는 용량 차지가 많아 Custom으로 일단 설치

![image](https://user-images.githubusercontent.com/30613069/163695257-d593f76f-2092-4e91-9ee7-8eaa1a275f3b.png)


![image](https://user-images.githubusercontent.com/30613069/163695275-8c570653-2f32-4538-9cca-1aac5a120026.png)

![image](https://user-images.githubusercontent.com/30613069/163695287-29d26e6b-c57e-4fc7-9162-4b9889fff722.png)

3. TCP/IP 포트 넘버 기억하기!
![image](https://user-images.githubusercontent.com/30613069/163695375-3a35e71f-dbfc-4d98-8731-5a4fb4b29a95.png)


4. Account and Roles
![image](https://user-images.githubusercontent.com/30613069/163695380-158e09bc-728b-49a3-b8a4-6a815c9ba84c.png)

4-1. Root Password - 관리자 패스워드 설정
![image](https://user-images.githubusercontent.com/30613069/163695396-a7c7e417-6804-49d8-8d83-1dfad57eb866.png)

5. Windows Service
- mysql 0.8 버전이다 해서 80 붙지만 내 local pc에선 하나만 쓰일 것이므로 일단 80 삭제
![image](https://user-images.githubusercontent.com/30613069/163695422-0ea06db1-b369-4d0d-8740-f11d3014140f.png)


6. Apply Configuration
![image](https://user-images.githubusercontent.com/30613069/163695448-b959e28b-4f25-4fac-95cd-2cdbccfe320f.png)

7. 설치 후 Connection
![image](https://user-images.githubusercontent.com/30613069/163695464-9df639ca-c7e8-493c-a302-d39ff1be936b.png)
![image](https://user-images.githubusercontent.com/30613069/163695468-1259267a-1b24-46ae-b8f5-980a8eea4329.png)

8. Apply configuration - execute 계속 누르기
![image](https://user-images.githubusercontent.com/30613069/163695480-5fa5c60a-1e44-47c6-933b-5ff7dd990473.pn

9. 로컬 PC 확인

![image](https://user-images.githubusercontent.com/30613069/163695492-49b55100-c248-492f-91c2-4eeaa095413b.png)

10. MySQL > EDIT > Preference

![image](https://user-images.githubusercontent.com/30613069/163695528-a3ba555c-6ce0-49a7-bbdd-c2aba39bd551.png)

11. SAFE UPDATES 체크 해제

![image](https://user-images.githubusercontent.com/30613069/163695543-386cf804-794a-4afa-a237-86100018610b.png)

12. 대문자만 나오게 설정

![image](https://user-images.githubusercontent.com/30613069/163695551-a83581ef-ed8c-4255-bf0d-fef445a7d848.png)

13. 샘플 db 가져오기
13-1. 명령프롬포트 관리자 권한으로 실행

13-2. PATH 설정
C:\Windows\system32>SETX PATH "%PATH%:C:\Program Files\MySQL\MySQL Server 8.0\bin
![image](https://user-images.githubusercontent.com/30613069/163695818-c621d783-66a9-4b1d-b932-03c4d70c4d37.png)

13-3. 재부팅해야 먹힘

13-4. employees 예제 파일 옮기기
C:\Program Files\MySQL\employees
![image](https://user-images.githubusercontent.com/30613069/163696045-0dbc023d-ce5a-4bbd-b01f-71195cde1a4d.png)
![image](https://user-images.githubusercontent.com/30613069/163696063-1b62daff-ad6a-41c1-96cf-a1cccf470bf2.png)

13-5. dir
![image](https://user-images.githubusercontent.com/30613069/163696075-6ee15fd5-4f58-454e-b267-3a492ee180ef.png)

13-6. 내 pc > 우클릭 > 속성 > 고급 > 환경 변수 > Path 확인
아래의 경로가 Path에 있어야만 cmd 창이 먹힘
C:\Program Files\MySQL\MySQL Server 8.0\bin
![image](https://user-images.githubusercontent.com/30613069/163696134-a94b93c6-a2ac-4c82-bc04-819417b2913b.png)

13-7. mysql 로 로그인
C:\Windows\system32>cd C:\Program Files\MySQL\employees

C:\Program Files\MySQL\employees>mysql -u root -p
![image](https://user-images.githubusercontent.com/30613069/163700197-f96383b6-a117-4cf9-aecd-c1f4529aa968.png)

13-8. 이관
mysql> source employees.sql;

![image](https://user-images.githubusercontent.com/30613069/163700379-19643d05-87fc-406f-a27e-9e33408d2c7d.png)


