# OMX 모터 ID 설정 방법

## 1. 서브모터 ID 변경

서브모터 1~6의 ID를 아래와 같이 변경한다.

| 기존 ID | 변경 ID |
|---|---|
| 1 | 11 |
| 2 | 12 |
| 3 | 13 |
| 4 | 14 |
| 5 | 15 |
| 6 | 16 |

---

## 2. ID 변경 방법

1. 보드와 모터를 연결한다.
2. Dynamixel Wizard 2.0 실행
3. `설정` 탭에 들어간다.
4. `검색` 버튼을 누른다.
5. 설정에서 아래와 같이 체크한다.
   - `Protocol 2.0` : 체크
   - `표준 Bluetooth에서 직렬 링크` : 체크 해제
6. 연결된 모터를 선택한다.
7. `ID` 탭에 들어간다.
8. 원하는 ID를 선택한다.
9. `저장(Save)` 버튼을 누른다.
<img width="2252" height="4000" alt="KakaoTalk_20260508_142119967" src="https://github.com/user-attachments/assets/6fcc97cb-69b9-4a34-a2fe-a47d9c26b6ce" />
오류화면
<img width="591" height="463" alt="스크린샷 2026-05-08 130805" src="https://github.com/user-attachments/assets/024657e0-7c8c-4227-9021-e1c402f9a5c8" />


---

## 3. 저장 확인 방법

1. 연결을 끊는다.
2. 다시 연결한다.
3. 검색 후 변경된 ID가 정상적으로 표시되는지 확인한다.

예시:
- 기존 ID 1 → 변경 후 ID 11로 표시되면 정상적으로 저장된 것이다.
