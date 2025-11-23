# 📦 자동 물류 분류 시스템

주소지 기반의 자동 물류 분류 기능을 갖춘 스마트 컨베이어 시스템

## ⚙️ Features
|기능|기능 상세|
|------|------------|
|물류 입고 감지 기능|새로운 물류가 들어왔음을 감지|
|주소지 인식 기능|물류 상자에 부착된 QR 코드를 스캔하여 주소지 추출|
|물류 분류 기능|주소지를 기준으로 분류기를 제어|

## 💠 Environments
### Hardware
|||
|------|------------|
|STM32F103C8T6|<img width="100" height="100" alt="Image" src="https://github.com/user-attachments/assets/2ca5771b-33b1-4507-bf6d-6352d282d017" />|
|TCRT5000 적외선 광센서|<img width="100" alt="Image" src="https://github.com/user-attachments/assets/be7bb56e-e997-4225-b133-a417bc57879a" />|
|SG90 360도 디지털 서보모터|<img width="100" height="100" alt="Image" src="https://github.com/user-attachments/assets/602fb979-9817-48b3-ad29-6fe76cc2e452" />|
|5V 스텝모터 + ULN2003 모터 드라이버 |<img width="100" alt="Image" src="https://github.com/user-attachments/assets/a2d52a8a-07ce-4158-a13c-161a236cdb2f" />|
|DC 모터|<img width="100" height="100" alt="Image" src="https://github.com/user-attachments/assets/29ef962d-4e5c-43e0-a92d-bd88d58ba140" />|
|L298 모터드라이버|<img width="100" alt="Image" src="https://github.com/user-attachments/assets/49ac122f-3a81-4237-8af5-96241a84024a" />|


### Software
- STM32Cube HAL
- FreeRTOS (CMSIS-OS v2)

## 🗺️ 시스템 구성도
<img width="773" height="543" alt="Image" src="https://github.com/user-attachments/assets/17a0169f-a7e4-41c5-b686-66bd2f1b34db" />
