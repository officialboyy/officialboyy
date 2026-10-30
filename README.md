# 박준호 · Junho Park

**Embedded Software / Firmware**

저는 STM32 기반 센서·모터 제어 프로젝트와 차량 통신 시스템 설계를 경험했습니다.
현재 HINT 프로젝트의 리더로 FreeRTOS 기반 CAN–LIN 시스템의 ECU 간 통신 펌웨어를 구현하고 있습니다.
차량 전장 SW를 중심으로 임베디드 SW·펌웨어 분야에서 일하고 싶으며, 임베디드 AI도 교육 실습을 통해 공부했습니다.

[Email](mailto:pjh0063@gmail.com) · [GitHub](https://github.com/officialboyy)

## Current Project

### FreeRTOS CAN–LIN Gateway

HINT 교육에서 시작한 차량 네트워크 프로젝트입니다.
저는 팀 리더로 시스템 아키텍처와 통신 명세, 고장 대응 정책 정리를 주도했고, 현재 ECU 간 통신을 구현하고 있습니다.

- **개발 환경:** STM32, FreeRTOS, CAN, LIN
- **통신 설계:** CAN DBC, LIN LDF, 통신·메시지 정의서
- **처리 구조:** ISR → Queue → Task
- **설계 내용:** CAN·LIN 간 신호 전달, 주기 차이를 처리하는 신호 캐시, 통신 이상 감지와 Fault/Failsafe 상태 전이
- **진행 상태:** 펌웨어 개발 및 ECU 간 통신 구현 중

HINT 교육은 2026년 10월 22일에 수료했으며, 프로젝트는 이후에도 진행하고 있습니다.

## Repositories

### [STM32F411 Firmware](https://github.com/officialboyy/stm32f411_fw)

STM32F411 기반 펌웨어 학습 저장소입니다.

- Application / BSP / Hardware 계층을 구분한 코드 구성
- GPIO 기반 LED 드라이버
- USB CDC 전송 호출
- STM32 HAL 기반 주변장치 제어

### [STM32 Practice](https://github.com/officialboyy/stm32_prac)

STM32CubeIDE / STM32CubeMX 기반 펌웨어 실습 저장소입니다.

- STM32 프로젝트 구성
- MCU 초기화 및 주변장치 제어 학습
- 시작 코드와 링커 스크립트를 포함한 개발 환경

### [HARMAN Semiconductor Academy](https://github.com/officialboyy/Harman)

하만 세미콘 아카데미에서 진행한 임베디드 시스템·디지털 회로·SoC 관련 학습과 프로젝트 자료입니다.

- ARM 기반 MCU 프로그래밍
- 센서·모터 제어 및 통신 연동
- Verilog / VHDL
- SoC Peripheral 설계

## Education Projects

### STM32 커넥티드 자율이동체

초음파 센서로 장애물을 감지하고 Bluetooth로 수동 조작하는 이동체 제작 프로젝트에 참여했습니다.

- **기간:** 2024.05.08–2024.05.30
- **구성:** STM32F411RE, HC-SR04, HC-06, 모터 드라이버
- **기능:** 장애물 감지, 모터 제어, 자동·수동 주행
- **개발 환경:** C/C++, STM32CubeIDE

### Smart Farm

환경 센서와 제어 장치, 모바일 앱을 연결하는 스마트팜 제작 프로젝트에 참여했습니다.

- **기간:** 2024.07.15–2024.08.13
- **구성:** 온습도·토양 수분·조도 센서, 팬·모터, Bluetooth 통신
- **기능:** 환경 상태 확인, 장치 제어, 모바일 앱 연동
- **개발 환경:** C/C++, STM32CubeIDE, Android

두 프로젝트는 하만 세미콘 아카데미 교육에서 진행했습니다.

## Technical Experience

| 기술 | 사용한 맥락 |
| --- | --- |
| C / C++, STM32CubeIDE | STM32 펌웨어 실습, 센서·모터 제어 프로젝트 |
| PWM, UART | 자율이동체 모터 제어와 Bluetooth 통신 |
| FreeRTOS | HINT 프로젝트의 ISR·Queue·Task 처리 구조 설계 및 구현 |
| CAN, LIN | 차량 네트워크 통신 명세와 ECU 간 통신 구현 |
| DBC, LDF | CAN 메시지와 LIN 프레임·스케줄 정의 |
| Python, OpenCV | 카메라 입력과 움직임 감지 교육 실습 |
| MobileNetV2, TensorFlow Lite / LiteRT | 분류 모델 학습·변환·추론 교육 실습 |
| Verilog, Vivado / Vitis | 디지털 회로와 SoC Peripheral 교육 실습 |

## Education & Certification

- **울산대학교 전기전자공학** — 졸업, 2022.02
- **하만 세미콘 아카데미 부산 3기** — 수료, 2024.08
- **HINT Embedded AI(SW) 1기** — 수료, 2026.10.22
- **전기기사** — 취득, 2022.11

## Contact

- Email: [pjh0063@gmail.com](mailto:pjh0063@gmail.com)
- GitHub: [officialboyy](https://github.com/officialboyy)
