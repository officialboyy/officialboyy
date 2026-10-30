<div align="center">

# Junho Park

### 박준호 · Embedded Software / Firmware

차량 전장 SW · STM32 펌웨어 · CAN–LIN 네트워크

[![Email](https://img.shields.io/badge/Email-pjh0063%40gmail.com-176047?style=flat-square)](mailto:pjh0063@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-officialboyy-202020?style=flat-square&logo=github&logoColor=white)](https://github.com/officialboyy)

[Projects](#projects) &nbsp; · &nbsp; [Technical Experience](#technical-experience) &nbsp; · &nbsp; [Education](#education)

</div>

---

## About

저는 STM32 기반 센서·모터 제어 프로젝트와 차량 통신 시스템 설계를 경험했습니다. 현재 HINT 프로젝트의 리더로 FreeRTOS 기반 CAN–LIN 시스템의 ECU 간 통신 펌웨어를 구현하고 있습니다. 차량 전장 SW와 임베디드 펌웨어 개발을 중심으로 일하고 싶으며, 임베디드 AI도 교육 실습을 통해 공부했습니다.

## Projects

### 01 / FreeRTOS CAN–LIN Gateway

**차량 CAN 네트워크와 LIN Body 네트워크를 연결하는 분산 ECU 시스템**

![STM32](https://img.shields.io/badge/MCU-STM32-202020?style=flat-square)
![FreeRTOS](https://img.shields.io/badge/RTOS-FreeRTOS-202020?style=flat-square)
![CAN](https://img.shields.io/badge/CAN-500_kbps-176047?style=flat-square)
![LIN](https://img.shields.io/badge/LIN-19.2_kbps-176047?style=flat-square)

> **역할** &nbsp; Project Leader<br>
> **상태** &nbsp; 펌웨어 개발 · ECU 간 통신 구현 중

저는 시스템 아키텍처와 통신 명세, 고장 대응 정책 정리를 주도했습니다. CAN 측 VCU·Motor·Cluster와 LIN 측 Door·Light를 Gateway로 연결하는 구조를 설계하고 통신을 구현하고 있습니다.

- **수신 처리:** ISR → Queue → Task 구조
- **데이터 전달:** CAN·LIN의 주기 차이를 처리하는 신호 캐시와 라우팅
- **고장 대응:** 통신 이상 감지·전파와 각 ECU의 Local Fail-safe 책임 구분
- **통신 명세:** CAN DBC, LIN LDF, 통신·메시지 정의서

**[Repository →](https://github.com/HINT-CAN-LIN/freertos-can-lin-gateway)**

<sub>HINT 교육은 2026.10.22에 수료했으며, 프로젝트는 계속 진행하고 있습니다. 통합 시험 결과와 성능 측정값은 추후 정리할 예정입니다.</sub>

---

### 02 / STM32 커넥티드 자율이동체

**초음파 장애물 감지와 Bluetooth 수동 조작을 결합한 이동체**

`STM32F411RE` · `HC-SR04` · `HC-06` · `PWM` · `UART`

> **교육** &nbsp; 하만 세미콘 아카데미<br>
> **기간** &nbsp; 2024.05.08–05.30

저는 초음파 센서와 모터 제어를 사용하는 자동·수동 주행 이동체 제작 프로젝트에 참여했습니다. 개발 기록에는 코너 대응을 위해 전방 센서 3개에 측면 센서 2개를 추가한 과정이 있습니다.

**[교육·프로젝트 자료 →](https://github.com/officialboyy/Harman)**

---

### 03 / Smart Farm

**환경 센서·제어 장치·모바일 앱을 연결한 스마트팜**

`C/C++` · `STM32CubeIDE` · `DHT11` · `Bluetooth` · `Android`

> **교육** &nbsp; 하만 세미콘 아카데미<br>
> **기간** &nbsp; 2024.07.15–08.13

저는 온습도·토양 수분·조도 센서와 팬·모터, 모바일 앱을 연동하는 스마트팜 제작 프로젝트에 참여했습니다. 환경 상태 확인과 장치 제어를 구성하는 임베디드 프로젝트를 경험했습니다.

**[교육·프로젝트 자료 →](https://github.com/officialboyy/Harman)**

## Firmware Practice

| 저장소 | 코드에서 확인할 수 있는 내용 |
| :--- | :--- |
| **[stm32f411_fw](https://github.com/officialboyy/stm32f411_fw)** | `ap` / `bsp` / `hw` 계층 구성, HAL 기반 LED 드라이버, USB CDC 전송 호출 |
| **[stm32_prac](https://github.com/officialboyy/stm32_prac)** | STM32CubeIDE / CubeMX 기반 실습, 시작 코드와 링커 스크립트를 포함한 프로젝트 구성 |
| **[Harman](https://github.com/officialboyy/Harman)** | ARM·임베디드 제어·Verilog·SoC Peripheral 교육 및 프로젝트 자료 |

## Technical Experience

| 분야 | 기술 | 사용 맥락 |
| :--- | :--- | :--- |
| **Firmware** | C / C++, STM32, STM32CubeIDE | 센서·모터 제어 프로젝트와 MCU 펌웨어 실습 |
| **Interface** | PWM, UART | 자율이동체 모터 제어와 Bluetooth 통신 |
| **Vehicle Network** | FreeRTOS, CAN, LIN, DBC / LDF | HINT 통신 구조 설계와 ECU 통신 구현 |
| **Embedded AI** | Python, OpenCV, MobileNetV2, TensorFlow Lite / LiteRT | 카메라 입력, 분류 모델 학습·변환·추론 교육 실습 |
| **Digital / SoC** | Verilog, Vivado / Vitis | 디지털 회로·SoC Peripheral 교육 실습 |

## Education

| 과정 | 이수 |
| :--- | :--- |
| **HINT Embedded AI(SW) 1기** | 2026.10.22 수료 |
| **하만 세미콘 아카데미 부산 3기** | 2024.08 수료 |
| **울산대학교 전기전자공학** | 2022.02 졸업 |

---

<div align="center">

**Junho Park** &nbsp; / &nbsp; Embedded Software · Firmware<br>
[pjh0063@gmail.com](mailto:pjh0063@gmail.com)

</div>

<!-- 프로젝트 진행 상태 확인 기준: 2026-10-30 -->
