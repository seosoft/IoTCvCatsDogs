# 【開発手順のハンズオン】Azure IoT Edge + Custom Vision を使ってエッジデバイスで画像分類するアプリケーション

**Azure IoT Edge ＋ Custom Vision を使ってエッジデバイスで画像分類するアプリケーション** を開発するハンズオン資料です。

開発環境の構築からアプリケーション実行方法・動作確認方法までの一連の流れを体験できます。

1. [開発環境の構築](./01_install.md)
2. [Custom Vision で画像分類器の作成](./02_custom_vision.md)
3. [IoT Edge ソリューションの作成](./03_create_edgeapp.md)
4. [予測サービスモジュールの編集](./04_edit_classfier.md)
5. [カメラモジュールの作成](./05_create_cameramodule.md)
6. [Container Registry にモジュールをアップロード](./06_upload_to_acr.md)
7. [IoT Hub / Edge デバイスの準備とソリューションのローカル実行](./07_create_iothub_edgedevice.md)
9. [IoT Edge デバイスを作成する](./08_prepare_edgedevice.md)
9. [IoT Edge デバイスでソリューションを実行する](./09_run_on_edgedevice.md)

<br />

<img src="../docs/images/customvision_top_image.jpg" width="560px" />
<br />
<img src="../docs/images/07/vs_starting_iotedge_simulator.jpg" width="560px" />
<br />
<img src="../docs/images/09/vs_display_buildin_monitor.jpg" width="560px" />

<br />

---

このハンズオンは、[Azure IoT Edge の公式チュートリアル](https://docs.microsoft.com/ja-jp/azure/iot-edge/tutorial-deploy-custom-vision) を元に、

- 手順の整理
- 手順の追加
- アプリケーションのソースコードを一部改訂

をしました。

<br />

> このハンズオンでは物理デバイスを使用せずに **カメラのシミュレーター**を使います。  
> 物理デバイスを持っていなくても全ての手順を実行することができ、アプリケーション開発の流れと、Costom Vision および IoT Edge、Azure IoT の基礎を理解できます。

<br />

---

Copyright (C) 2020-2021 Seosoft All rights reserved.  
本コンテンツの著作権、および本コンテンツ中に出てくる商標権、団体名、ロゴ、製品、サービスなどはそれぞれ、各権利保有者に帰属します。