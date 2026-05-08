# OMX Follower

## 1. 개요

OMX는 Leader와 Follower 구조로 구성되어 있다.

- Leader : 사용자가 직접 움직이는 로봇 암
- Follower(서브 모터) : Leader의 움직임을 따라 움직이는 로봇 암

Follower 모터의 ID를 Leader와 다르게 설정해야 충돌 없이 정상적으로 동작한다.

기본적으로 Leader는 ID 1~6을 사용하므로,
Follower는 ID 11에서16으로 변경하여 사용한다.

---

# 2. 준비물

- OMX 본체
- OpenRB-150 보드
- USB-C 케이블
- 외부 전원(SMPS 또는 배터리)
- Dynamixel Wizard 2.0 프로그램
- Windows 또는 Ubuntu PC

---

# 3. 보드 연결 방법

## 3-1. USB 연결

1. OpenRB-150 보드를 USB-C 케이블로 PC와 연결한다.
2. 연결 후 보드 LED가 켜지는지 확인한다.

---

## 3-2. 모터 연결

모터 케이블이 OpenRB-150의 `DXL` 포트에 연결되어 있는지 확인한다.

- USB 포트와 DXL 포트는 다르다.
- DXL 포트에 연결되어 있어야 모터 검색이 가능하다.

---

# 4. Dynamixel Wizard 2.0 실행

1. Dynamixel Wizard 2.0 실행
2. 상단의 `연결하기` 버튼 클릭

---

# 5. 포트 설정

다음과 같이 설정한다.

| 항목 | 설정값 |
|---|---|
| COM Port | COM3 또는 연결된 포트 |
| Baudrate | 1000000 bps |
| Protocol | Protocol 2.0 |

주의:
- OMX 기본 baudrate는 1000000 bps이다.
- 9600 bps로 설정하면 검색이 실패할 수 있다.

---

# 6. 검색 설정

`설정` 탭에서 아래와 같이 설정한다.

| 옵션 | 설정 |
|---|---|
| Protocol 2.0 | 체크 |
| 표준 Bluetooth에서 직렬 링크 | 체크 해제 |

설정 후 `검색(Scan)` 버튼 클릭

---

# 7. 모터 검색

검색이 성공하면 연결된 모터 목록이 표시된다.

예시:

```text
ID: 1
Model: XL330
