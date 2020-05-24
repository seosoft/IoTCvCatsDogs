# 【開発完了時点のソースコード】Azure IoT Edge + Custom Vision を使ってエッジデバイスで画像分類するアプリケーション

Azure IoT Edge ＋ Custom Vision を使ってエッジデバイスで画像分類するアプリケーションのソースコードです。

[ハンズオン](../docs/README.md) の手順で開発完了した時点のソースコードです。  
ハンズオンの参考として利用してください。

> ソースコード利用上の注意  
>  
> ソリューションのルートフォルダーにある "**_env**" ファイルは、"**.env**" にリネームして利用してください。  
> その際には、先頭3行のコメント部分は削除してください。  
> また別途 [**Azure Container Registry**](https://azure.microsoft.com/ja-jp/services/container-registry/) を作成して、ユーザー名、パスワードで ".env" の該当部分を置換してください。
>
> ```txt
> 
> CONTAINER_REGISTRY_USERNAME_catsdogsreg=<ACRユーザー名>
> CONTAINER_REGISTRY_PASSWORD_catsdogsreg=<ACRパスワード>
>
> ```

---

Copyright (C) 2020 Seosoft All rights reserved.  
本コンテンツの著作権、および本コンテンツ中に出てくる商標権、団体名、ロゴ、製品、サービスなどはそれぞれ、各権利保有者に帰属します。
