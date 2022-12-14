### 1. 테이블
<img width="395" alt="스크린샷 2023-01-02 오전 1 28 35" src="https://user-images.githubusercontent.com/90540377/210177933-616c9686-7c37-44e8-b301-6ff9f3864944.png">

### 2. 클래스 다이어그램
![classDiagram](https://user-images.githubusercontent.com/90540377/210321782-6c18f9f8-e786-4d9f-884a-e5b1df692724.png)

### 3. 초기 관리자 화면
![스크린샷 2023-01-03 오후 5 24 00](https://user-images.githubusercontent.com/90540377/210321642-eba3a038-fe5d-42f7-a6af-e9e4f4c508f9.png)

### 4. 초기 사용자 화면
<img width="337" alt="스크린샷 2022-12-30 오후 4 15 07" src="https://user-images.githubusercontent.com/90540377/210044457-fbe76cfd-993f-4de1-bef0-ef70e90e03fc.png">

---

# 3차 미니 프로젝트
1. 1차시 미니 프로젝트와 동일한 주제    
2. 추가 요구 사항
    - JDBC를 이용하여 오라클DB와 연동 할 것
    - 처리 결과 메시지를 확실시 할 것
    - 싱글톤 패턴을 적용하여 DAO를 Service와 Template 세분화 할 것

## 1차 피드백
- [x] 테이블을 구성할때 JOIN을 안써도 구현이 가능함
    - 학생테이블에 과목테이블의 과목 코드를 외래키로 설정해두고 접근
    
# 2차 미니 프로젝트
1. 1차시 미니 프로젝트와 동일한 주제    
2. 추가 요구 사항
    - 기존 배열이 아닌 컬렉션 프레임워크를 적용 할 것
    - MVC 디자인 패턴에 맞게 작성 할 것
3. 추가 개선 사항
    - 관리자를 따로 생성, 과목도 추가 삭제가 가능하도록 함
    - 불필요한 필드를 최대한 정리

## 1차 피드백
- [x] 하나의 객체를 사용하는것은 맞지만, static 변수까지 적용하면서 싱글톤 패턴을 사용 할 필요 없음
    - StackOverflowError 가능성 존재
    - Run 클래스에서만 객체를 생성하고 인스턴스 변수로 수정
    
# 1차 미니 프로젝트
1. 주제 - 간단한 수강 신청 프로그램
2. 요구사항
    - 개설 과목 확인시 신청 인원을 보여줄것
    - 수강 신청시 과목명 말고 과목코드를 통해 입력 받도록 할 것
3. 동작화면
    - 개설 과목 조회
    - 수강 신청
    - 수강 내역 조회
    - 프로그램 종료

## 1차 피드백
- [x] RegisterFunction의 addSubject()의 중복 코드들을 메서드로 만들어서 간결하게 할 것
    - findUpdate() : 일치하는 정보가 존재하는 경우 기존 객체를 변경
    - notFindUpdate() : 일치하는 정보가 없는 경우 새로운 객체 생성

## 2차 피드백
- [x] RegisterFunction의 addSubject() 불필요한 switch-case문 제거 할 것

## 3차 피드백
- [x] RegisterFunction의 불필요한 static 제거 할 것
