# ASSIGNMENT2_Mobile_and_Joystick

시작: 2023-09-13 </br>
완료: 2023-10-06 </br>

<details>
<summary>과제 요구사항 접기/ 펼치기</summary>

============ Assignment2_Mobile_and_Joystick 과제 내용 ============

플랫폼: 모바일(안드로이드)</br>
시점: TPS 백뷰

1.
모바일 TPS에서의 캐릭터 조작을 위한 조이스틱 (외부 파키지 쓰지 말고 직접 구현) </br>
터치를 통한 시점 이동(회전) </br>
UI에 배치될 버튼(점프 및 미개발 버튼)을 구현 </br>

2. 
점프 구현할 때 함수 안에 직접 기능을 넣지 않고 이벤트/action을 이용한 Delegate 패턴으로 구현할 것 </br>
Action Func Delegate </br>
UnityAction UnityEvent(사실상 현재 유니티UI에서 사용되는 것들) </br>
를 사용한 스크립트 작성. </br>

기타 정해지지 않았거나 모호한 부분은 HexaWorld어플 조작 참고 </br>

=================================================
</details>

## 이슈 메모

1. (해결) 레버가 드래그될 때만 이동됨. 레버 입력을 유지중일 때 이동이 계속되도록 수정 필요
2. (해결) 카메라가 보는 방향으로 캐릭터가 이동해야 함
3. (해결) CharacterController.isGrounded의 불안정성 문제 해결
4. (해결) Input이랑 EventSystem 동시에 사용 못하는 문제. 

## 완료한 작업
1. UI 구현
- 조이스틱 조작
    - 이미지가 입력 따라 움직이게 만들기
    - 이미지 이동범위 제한
- 시점 이동 영역
- 점프 버튼
2. 캐릭터 조작
- 이동
    - 조이스틱에 값 반환 구현
    - 캐릭터 이동과 연계
- 점프
3. 카메라 이동
