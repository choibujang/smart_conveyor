# 📦 자동 물류 분류 시스템

주소지 기반의 자동 물류 분류 기능을 갖춘 스마트 컨베이어 시스템

## ⚙️ Features
|기능|기능 상세|
|------|------------|
|입고||
|분류||
|||

## 💠 Environments
### Hardware
|||
|------|------------|
|STM32F103C8T6|<img width="100" height="100" alt="Image" src="https://github.com/user-attachments/assets/2ca5771b-33b1-4507-bf6d-6352d282d017" />|
|TCRT5000 적외선 광센서|<img width="100" alt="Image" src="https://github.com/user-attachments/assets/be7bb56e-e997-4225-b133-a417bc57879a" />|
|SG90 360도 디지털 서보모터|<img width="100" height="100" alt="Image" src="https://github.com/user-attachments/assets/602fb979-9817-48b3-ad29-6fe76cc2e452" />|
|5V 스텝모터 + ULN2003 모터 드라이버 |<img width="100" alt="Image" src="https://github.com/user-attachments/assets/a2d52a8a-07ce-4158-a13c-161a236cdb2f" />|
|DC 모터||
### Software
- STM32Cube HAL
- FreeRTOS (CMSIS-OS v2)

## 💬 통신 프로토콜

시스템은 UART 통신을 통해 QR 리더기(시뮬레이터)와 통신합니다.

*   **MCU -> QR 리더기**: QR 코드 인식을 요청합니다.
    *   형식: `<QR_REQUEST,parcel_id>`
    *   예시: `<QR_REQUEST,1>`

*   **QR 리더기 -> MCU**: QR 코드 인식 결과를 응답합니다.
    *   형식: `<QR_OK:parcel_id,destination_id>`
    *   예시: `<QR_OK:1,2>` (1번 물류의 목적지는 2번입니다)
