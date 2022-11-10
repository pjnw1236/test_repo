# **Java Convention**

---

# 1 Java 파일의 기본
## 1.1 파일명
파일 이름은 포함된 최상위 클래스의 대소문자 구분한 이름과 ```.java확장자```로 구성

## 1.2 파일 인코딩: UTF-8
파일은 기본적으로 UTF-8로 인코딩함

## 1.3 공백 문자
Tab은 인텔리제이 IDE Code Style을 따름 (4칸 들여쓰기)

---

# 2 Java 파일 구조
Java 파일은 다음 순서대로 구성
1. 패키지명
2. import문
3. 클래스

## 2.1 패키지명
패키지 문은 줄 바꿈되지 않음
## 2.2 import문
```*```(와일드 카드)를 이용하지 않고, 직접 지정

---

# 3 Formatting
## 3.1 선택 사항인 경우에서도 무조건 중괄호 사용
* 예시1
```java 
for (int i=0; i<3; i++) 
	System.out.println(i);
```
* 예시2
```java 
for (int i=0; i<3; i++) {
	System.out.println(i);
}
```
예시1처럼 실행하여도 실행이 되지만, 예시2처럼 중괄호 무조건 사용하기

## 3.2 한 줄에 한개의 문장씩 쓰기
단, 다음은 예외 사항 
1. 한 줄에 100자를 넘는 경우
2. 패키지 및 import문을 사용하는 경우
3. 주석인 경우

## 3.3 Enum 클래스
enum 자료형의 줄바꿈은 선택사항
* 예시1
```java 
public enum { 10, 20, 30 }
```
* 예시2
```java 
public enum {
	10,
	20, 
	30
}
```
enum type인 경우 예시1과 예시2 모두 허용

## 3.4 변수 선언
변수 초기화시 한줄에 한번씩 선언
* 예시1
```java 
int a; int b;
```
* 예시2
```java 
int a;
int b; 
```
예시1과 같이 하지말고, 예시2와 같이함

## 3.5 Array 
배열은 형식은 자유이며 다음과 같은 예시 모두 가능하다.
* 예시1
```java
public enum nums { 1, 2, 3, 4 };
```
* 예시2
```java
public enum nums {
	1, 2, 3, 4
};
```
* 예시3
```java
public enum nums {
	0,
	1,
	2,
	3,
};
```

## 3.6 Annotations 
한 줄에 하나의 Annotation 사용

## 3.7 Modifiers(접근 제한자의 순서) 
접근 제한자의 순서는 다음을 따른다.
1. public 
2. protected
3. private
4. abstract
5. default
6. static
7. final

## 3.8 Long형 숫자
long 값은 갖는 정수 리터럴은 접미사 l인 아닌 접미사 L을 사용
(l과 1 혼동 방지를 위함)
---

## 4 식별자 유형별 규칙
## 4.1 package명 
* 소문자로 구성 
## 4.2 클래스명 
* UpperCamelCase 
## 4.3 메서드명 
* lowerCamelCase 
## 4.4 상수
* 대문자로 구성
## 4.5 필드명 
* lowerCamelCase 
## 4.6 파라미터명 
* lowerCamelCase
## 4.7 지역변수명 
* lowerCamelCase


