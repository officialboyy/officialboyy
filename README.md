# 박준호 · Junho Park

Embedded Software / Firmware

저는 STM32 기반 센서·모터 제어 프로젝트와 차량 통신 시스템 설계를 경험했습니다.
현재 HINT 프로젝트의 리더로 FreeRTOS 기반 CAN–LIN 시스템의 ECU 간 통신 펌웨어를 구현하고 있습니다.
차량 전장 SW를 중심으로 임베디드 SW·펌웨어 분야에서 일하고 싶으며, 임베디드 AI도 교육 실습을 통해 공부했습니다.

[Email](mailto:pjh0063@gmail.com) · [GitHub](https://github.com/officialboyy)

## 진행 중인 프로젝트

### FreeRTOS CAN–LIN Gateway · HINT

저는 팀 리더로 시스템 아키텍처와 통신 명세, 고장 대응 정책 정리를 주도했습니다.
CAN 측 ECU와 LIN 측 노드를 Gateway로 연결하는 구조를 설계했고, 현재 각 ECU 간 통신을 구현하고 있습니다.

- **환경:** STM32, FreeRTOS, CAN, LIN
- **설계 자료:** CAN DBC, LIN LDF, 통신·메시지 정의서, Fault/Failsafe 정책
- **설계 내용:** ISR → Queue → Task 처리 구조, 통신 주기가 다른 네트워크 사이의 신호 캐시, 통신 이상 감지와 상태 전이
- **현재 상태:** 펌웨어 개발 및 ECU 통신 구현 중

HINT 교육은 2026년 10월 22일에 수료했습니다. 프로젝트는 이후에도 진행하고 있으며, 통합 시험 결과와 성능 측정값은 아직 정리하지 않았습니다.

## 공개 코드

| 저장소 | 내용 |
| --- | --- |
| [stm32f411_fw](https://github.com/officialboyy/stm32f411_fw) | STM32F411 펌웨어 학습 코드입니다. `ap`·`bsp`·`hw` 계층을 나누고, LED 드라이버와 USB CDC 전송 호출을 작성했습니다. |
| [stm32_prac](https://github.com/officialboyy/stm32_prac) | STM32CubeIDE / CubeMX 기반 펌웨어 실습 저장소입니다. |
| [Harman](https://github.com/officialboyy/Harman) | 하만 세미콘 아카데미에서 작성한 ARM·임베디드 시스템·Verilog·SoC 관련 학습 및 프로젝트 자료입니다. |

## 교육 프로젝트

### STM32 커넥티드 자율이동체

초음파 센서로 장애물을 감지하고 Bluetooth로 수동 조작하는 이동체 제작 프로젝트에 참여했습니다.
STM32F411RE, HC-SR04, HC-06을 사용해 센서 입력과 모터 제어를 구성했습니다.

### Smart Farm

온습도·토양 수분·조도 센서와 제어 장치, 모바일 앱을 연결하는 스마트팜 제작 프로젝트에 참여했습니다.
STM32CubeIDE와 C/C++을 사용한 임베디드 제어, 센서·통신 연동을 경험했습니다.

두 프로젝트는 하만 세미콘 아카데미 교육에서 진행했습니다.

## 기술 사용 맥락

| 항목 | 사용한 맥락 |
| --- | --- |
| C / C++, STM32CubeIDE | STM32 펌웨어 실습과 센서·모터 제어 프로젝트 |
| PWM, UART | 자율이동체 모터 제어와 Bluetooth 통신 |
| FreeRTOS, CAN, LIN, DBC / LDF | HINT 차량 네트워크 설계 및 통신 펌웨어 구현 |
| Python, OpenCV | 카메라 입력과 움직임 감지 교육 실습 |
| MobileNetV2, TensorFlow Lite / LiteRT | 분류 모델 학습·변환·추론 교육 실습 |
| Verilog, Vivado / Vitis | 하만 세미콘 아카데미의 디지털 회로·SoC Peripheral 교육 실습 |

## 학력·교육·자격

- 울산대학교 전기전자공학 졸업 · 2022.02
- 하만 세미콘 아카데미 부산 3기 수료 · 2024.08
- HINT Embedded AI(SW) 1기 수료 · 2026.10.22
- 전기기사 · 2022.11 취득

<!-- 진행 상태와 공개 저장소 설명의 확인 기준: 2026-10-30 -->
