# 오늘은 자바 1일차

> Write once, run anywhere

#### 자바란?
자바(Java)란 썬 마이크로시스템즈에서 1995년에 개발한 객체 지향 프로그래밍 언어이다.
    Java는 크게 다음과 같은 3가지 에디션으로 나뉜다.
* Java SE(Java Standard Edition / J2SE)
    대부분의 사람들이 가장 많이 접하는 표준 에디션. Java의 핵심 API와 기능들을 제공한다. JDK 항목도 참고.
* Jakarta EE, 구 Java EE(Java Enterprise Edition / J2EE)
    기업에서 운영하는 서버 페이지에 특화된 에디션이다. JSP와 서블릿을 비롯한 웹 애플리케이션 서버에 관련된 기술들이 포함되어 있다.
* Java ME(Java Micro Edition / J2ME)
    피처폰, PDA, 셋톱박스, 센서 등의 임베디드 시스템 환경에 특화된 경량 에디션이다.

> 자바는 주로 Intellij 같은 IDE로 코딩한다.

예시 코드

```java
public class Main {
    public static void main(String[] args) {
        //TIP Press <shortcut actionId="ShowIntentionActions"/> with your caret at the highlighted text
        // to see how IntelliJ IDEA suggests fixing it.
        System.out.printf("Hello and welcome!");

        for (int i = 1; i <= 5; i++) {
            //TIP Press <shortcut actionId="Debug"/> to start debugging your code. We have set one <icon src="AllIcons.Debugger.Db_set_breakpoint"/> breakpoint
            // for you, but you can always add more by pressing <shortcut actionId="ToggleLineBreakpoint"/>.
            System.out.println("i = " + i); // 코멘트 테스트
        }
    }
}
```
위의 코드는 Intellij Community Edition에 있는 예시 코드이다.

> 몇가지 Intellij Java 명령어
* psvm
```java
    public static void main(String[] args) 
    {
        System.out.printf("Hello, world!");
    }
```
참고로 자바는 자바스크립트처럼 코드 마지막에 ;(세미콜론)을 붙여줘야 한다.

* sout
```java
    System.out.printf("Hello, Intellij!");
```

> 자바의 변수
```java
public class Var7 {
    public static void main(String[] args) {
        int a = 100; //정수
        double b = 10.5; //실수
        boolean c = true; // true / false
        char d = 'A'; // 문자 하나
        String e = "Hello Java"; // 문자열
        byte b = 127; // -127 ~ 128
        short s = 32767; // -32, 768 ~ 32,767
        int i = 2147483647; // -2,147,483,648 ~ 2,147,483,647

        // -9,223,372,036,854,775,808 ~ 9,223,972,036,854,775,807
        long l = 9223372036854775807L;

        // 실수
        float f = 10.0f;
        double d = 10.0;

        System.out.println(a);
        System.out.println(b);
        System.out.println(c);
        System.out.println(d);
        System.out.println(e);
    }
}
```
이처럼 자바에는 ~~쓸데없이~~ 많은 변수 형식이 잇다.