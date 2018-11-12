# Azure_Sphere_Sample_Smart_Fan
MT3620, Azure sphere, Smart fan, Azure IoT Hub 

# Devolopemet Tools
- Visual Studio 2017 Community/Enterprise/Professional (Open AzureSphereDemo2.sln)
- Arduino IDE (Open Arduino_code/Arduino_code.ino)
- Using [DeviceExplorer](https://github.com/Azure/azure-iot-sdks/releases) to manage Device twin and message transmission.

# IoT Technology 2018デモ

## セットアップ

- Arduino_code/Arduino_code.inoを、Arduino Unoへ書き込む。
- MT3620_code/AzureSphereDemo2.slnを、MT3620 Dev Boardへ書き込む。
- デモセットに電源供給する。（MT3620 Dev BoardのマイクロUSBで給電。外部からArduino Unoへの電源供給は不要。）

## 機能

- 環境温度を測定して、4桁ディスプレイに表示。
- `上限温度`を越えると(Arduino Unoの電源がONして)ファンが稼働。
- `下限温度`を下回ると(Arduino Unoの電源がOFFして)ファンが停止。
- スライダーでファンの回転速度を変更。(Arduino Unoの制御)
- MT3620 Dev BoardのボタンAを押すと、そのときの環境温度-1を`上限温度`と設定
- MT3620 Dev BoardのボタンBを押すと、そのときの環境温度+1を`下限温度`と設定
