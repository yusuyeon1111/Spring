# Spring

### Spring Framework의 특징
1. POJO 방식의 프레임워크이다.
2. 경량 컨테이너로서 자바 객체를 직접 관리함
3. IoC, DI, AOP 를 지원함
4. 확장성, 생산성이 높음

### annotation
1. @Controller → class 파일을 FC 가 일을 시킬 수 있는 POJO임을 나타냄
2. @RequestMapping(”/”) - 요청 url을 메소드와 연결시킬 수 있는 주석 --> 전송방식을 구분하지 않는다.
3. @Autonwired - Spring container 안쪽에 있는 객체를 가져와서 자동으로 주입시키는 주석
4. @GetMapping() - Get 전송박식 요청 url을 메소드와 연결시킬 수 있는 주석
5. @ PostMapping() -Post 전송박식 요청 url을 메소드와 연결시킬 수 있는 주석
6. @Select/@Delete/ @Insert / @Update ("sql 구문") - 비교적 간단한 sql구문일 때는, 굳이 xml파일로 가지 않고, annotation 활용해서 처리할 수 있음.
7. PathVariable("name값") - QueryString 형식이 아닌, 경로 자체에 데이터를 포함시켰을 때 해당하는 데이터를 수집하는 방법
![image](https://github.com/yusuyeon1111/Spring/assets/142488306/c776a28f-5b95-4912-92bf-cafa3bca3deb)
![image](https://github.com/yusuyeon1111/Spring/assets/142488306/76a3e07b-fa63-4a31-8c30-a5291e43cfb2)

![image](https://github.com/yusuyeon1111/Spring/assets/142488306/190eaa47-74cf-42af-93d0-e8534b94c271)
- FC Pattern
- HttpServletRequest 경량화된 버전 -> Model model
- model.addAttribute("name값", value);

### XML -> Extensible markup language
- pom -> servlet -> root -> web
    1. web.xml : 웹에 대한 전반적인 설정파일
    2. roor_context.xml : Sptring 환경설정 파일, 그 중에서도 DB와 관련된 설정 파일
    3. servlet - context.xml " : Spring 환경설정 파일
    4. pom.xml : Maven project 설정 파일

### DBCP (DataBase Connection Pool)
: 데이터 베이스를 연결하는 java기술 (데이터 베이스 성능 향상을 위해 사용하는 기술)
1. DBCP기술을 사용할 라이브러리 : HikariCP
2. sql 구문과 java 파일을 분리하고 자동으로 연결시켜주는 라이브러리 : mybatis
3. DB 드라이버 파일을 가져올 라이브러리 : my sql-connector-java
4. spring f/w와 mybatis f/w 연결해주는 라이브러리 : mybatis-spring
5. spring f/w jdbc 연결해주는 라이브러리 : spring-jdbc
![image](https://github.com/yusuyeon1111/Spring/assets/142488306/52799ed7-e3cb-45c7-a380-9a4e00b76258)
![image](https://github.com/yusuyeon1111/Spring/assets/142488306/b215673d-f7c1-44ea-92dd-7344484952bc)

 ### contextPath를 동적으로 가져오는 방법
 ```
<c:set var="cpath" value="${pageContext.request.contextPath }"/>
"/${cpath }”
```
