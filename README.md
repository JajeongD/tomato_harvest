# tomato_harvest
YOLOv8, RealSense D405, Raspberry Pi 5, ESP32/Arduino 기반 방울토마토 자동 수확 로봇 졸업작품

# Tomato Harvest Robot
방울토마토 자동 수확 로봇 졸업작품입니다.

라인을 따라 이동하는 모바일 플랫폼 위에 XYZ 직교 로봇 팔과 그리퍼를 구성하고,
YOLOv8 기반 비전 인식, RealSense D405 Depth 카메라, Raspberry Pi 5,
ESP32, Arduino Uno를 연동하여 방울토마토를 인식하고 수확하는 시스템입니다.

## 주요 기능

- YOLOv8 기반 방울토마토 인식 및 익음 정도 판별
- RealSense D405를 이용한 Depth 기반 위치 추정
- XYZ 직교 로봇 팔 제어
- 3지 소프트 그리퍼 기반 수확 동작
- Arduino Uno 기반 라인트레이싱 주행
- Raspberry Pi 5와 ESP32/Arduino 간 UART 분산 제어

## 코드 구성

- `apps/`: 주행, 비전, 수확, 전체 실행 로직
- `lib/`: 로봇 제어, 카메라, 캘리브레이션, 통신 공통 모듈
- `firmware/`: ESP32 및 Arduino 펌웨어
- `tools/`: 포트 스캔, 캘리브레이션, 테스트 도구
- `TOGG_map/`: 하드웨어/소프트웨어 구조 문서
