# Spring

Spring Framework의 특징

1. POJO 방식의 프레임워크이다.
2. 경량 컨테이너로서 자바 객체를 직접 관리함
3. IoC, DI, AOP 를 지원함
4. 확장성, 생산성이 높음

annotation
1. @Controller → class 파일을 FC 가 일을 시킬 수 있는 POJO임을 나타냄
2. @RequestMapping(”/”) - 요청 url을 메소드와 연결시킬 수 있는 주석 --> 전송방식을 구분하지 않는다.
3. @Autonwired - Spring container 안쪽에 있는 객체를 가져와서 자동으로 주입시키는 주석
4. @GetMapping() - Get 전송박식 요청 url을 메소드와 연결시킬 수 있는 주석
5. @ PostMapping() -Post 전송박식 요청 url을 메소드와 연결시킬 수 있는 주석
6. @Select("sql 구문") - 비교적 간단한 sql구문일 때는, 굳이 xml파일로 가지 않고, annotation 활용해서 처리할 수 있음.
![image](https://github.com/yusuyeon1111/Spring/assets/142488306/c776a28f-5b95-4912-92bf-cafa3bca3deb)
![image](https://github.com/yusuyeon1111/Spring/assets/142488306/76a3e07b-fa63-4a31-8c30-a5291e43cfb2)

![image](https://github.com/yusuyeon1111/Spring/assets/142488306/190eaa47-74cf-42af-93d0-e8534b94c271)
- FC Pattern
- HttpServletRequest 경량화된 버전 -> Model model
- model.addAttribute("name값", value);

  - pom -> servlet -> root -> web
  - XML -> Extensible markup language
    1. web.xml : 웹에 대한 전반적인 설정파일
   
