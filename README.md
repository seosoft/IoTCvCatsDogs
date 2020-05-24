# Azure IoT Edge + Custom Vision でエッジデバイスで画像分類

[**Azure IoT Edge**](https://docs.microsoft.com/ja-jp/azure/iot-edge/) + [**Custom Vision**](https://www.customvision.ai/) を使って、エッジデバイスで画像分類するアプリケーションです。  
例として、[猫と犬との画像](https://www.kaggle.com/chetankv/dogs-cats-images) を分類します。

Raspberry PI などの物理デバイスを使用せずに、**カメラのシミュレーター**を使います。  
物理デバイスを持っていなくてもアプリケーションを開発することができ、Costom Vision と IoT Edge、Azure IoT を理解できます。

このリポジトリは以下の内容を含みます。

- [**開発手順のハンズオン**](./docs/README.md)
- [**開発完了時点のソースコード**](./source/README.md)

実際に自分でアプリケーションを開発するには、[このリポジトリのハンズオン](./docs/README.md) を参照してください。

Custom Vision や Azure IoT の概要を知りたい場合、または開発の手順を短時間で直感的に追いたい場合は、別途用意した [**セッション資料**](https://www.slideshare.net/seosoft/azure-iot-edge-custom-vision) を参照してください。

---

<img src="./docs/images/customvision_top_image.jpg" width="360px" />
<br />
<img src="./docs/images/iotedge_top_image.jpg" width="360px" />
<br />
<img src="./docs/images/08/vs_display_buildin_monitor.jpg" width="480px" />


このアプリケーションは、[**勝手に勉強会** (2020年4月19日 開催)](https://katte.connpass.com/event/173288/) の説明・デモで使用したものです。

[Azure IoT Edge の公式チュートリアル](https://docs.microsoft.com/ja-jp/azure/iot-edge/tutorial-deploy-custom-vision) を元に、

- 手順の整理
- 手順の追加
- アプリケーションのソースコードを一部改訂

しました。

---

Copyright (C) 2020 Seosoft All rights reserved.  
本コンテンツの著作権、および本コンテンツ中に出てくる商標権、団体名、ロゴ、製品、サービスなどはそれぞれ、各権利保有者に帰属します。
