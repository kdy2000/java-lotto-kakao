# 로또
## 진행 방법
* 로또을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)

## 기능 요구사항
* 로또 구입 금액을 입력하면 구입 금액에 해당하는 로또를 발급해야 한다.
* 로도 1장의 가격은 1000원이다.

## 프로그래밍 요구사항
* indent(인덴트, 들여쓰기) depth를 2단계에서 1단계로 줄여라.
  * depth의 경우 if문을 사용하는 경우 1단계의 depth가 증가한다. if문 안에 while문을 사용한다면 depth가 2단계가 된다.
* else를 사용하지 마라.
* 메소드의 크기가 최대 10라인을 넘지 않도록 구현한다.
  * method가 한 가지 일만 하도록 최대한 작게 만들어라.
* **배열 대신 ArrayList를 사용한다.**
* java enum을 적용해 프로그래밍을 구현한다.
* **규칙 3: 모든 원시값과 문자열을 포장한다.**
* **규칙 5: 줄여쓰지 않는다(축약 금지).**
* **규칙 8: 일급 콜렉션을 쓴다.**


## 구현 기능 목록
- 로또 번호 6개 생성  
  - 1-1. 셔플 함수  
  - 1-2. index 0 ~ 5까지 숫자 리턴

- UI 기능  
  - 2-1. 구입 금액 입력을 위한 메시지 출력  
  - 2-2. 구입 금액 입력  
  - 2-3. 구매 갯수 출력  
  - 2-4. 구매한 로또 출력  
  - 2-5. 당첨번호 입력을 위한 메시지 출력  
  - 2-6. 당첨번호 입력  
  - 2-7. 보너스 볼 입력을 위한 메시지 출력  
  - 2-8. 보너스 볼 입력  
  - 2-9. 당첨 통계 출력  

- 당첨번호 확인 함수  
  - 3-1. 구매 로또에서 일치 여부 확인

- 스트링 스플릿 함수
  - 4-1. 공백 제거 후, (,) 기준으로 스플릿  
  - 4-2. 예외 상황 처리  
    - 4-2-1. 숫자가 아닌 문자열 스플릿  
    - 4-2-2. 공백 혹은 null  

- 수익률 계산 함수