# 開発環境の構築

最初に開発に必要な環境を構築します。

Azure IoT Edge + Custom Vision アプリケーションを開発するには、以下のツールのインストールが必要です。

[0. 開発用 PC の条件](#%e9%96%8b%e7%99%ba%e7%94%a8-pc-%e3%81%ae%e6%9d%a1%e4%bb%b6)  
[1. Visual Studio Code](#visual-studio-code)  
[2. Azure IoT Tools](#azure-iot-tools)  
[3. Docker Desktop](#docker-desktop)  
[4. (オプション) Anaconda](#anaconda)

<br />

> ここでは Windows 環境のみ記載しています。  
> Windows 以外の OS での動作確認は行っていません。

<br />

---

## 開発用 PC の条件

IoT Edge 開発では [**Docker Desktop**](https://www.docker.com/products/docker-desktop) が動作する必要があります。

Windows 10 の場合は

- Hyper-V または [**WSL2**](https://docs.microsoft.com/ja-jp/windows/wsl/install-win10) が動作する PC
- メモリ 16GB 程度以上

が必要です。

開発時には Visual Studio Code および Docker Desktop (+ IoT Edge Simulator) が同時に起動している必要があるため、マシンスペックによっても開発が困難または不可能なことがあります。
Windows 以外の場合でも Visual Studio Code + Docker Desktop が必要です。こちらも十分なスペックのマシンが必要です。

<br />

> Windows 10 で Docker Desktop を実行するために必要な条件は [**docker docs**](https://docs.docker.com/desktop/windows/install/) に書いてあります。  

<br />

> ローカル PC で実行できない場合は、**Azure 上に仮想マシンを作成** してハンズオンを進めることができます。
>
> 仮想マシンで Hyper-V を有効にするには [**Dv3 または Ev3 の仮想マシン**](https://docs.microsoft.com/ja-jp/azure/virtual-machines/windows/nested-virtualization) が必要です。  
> "Standard D4s_v3" などの Windows 10 仮想マシンを作成して、Visual Studio Code のインストールから実施してください。
>
> なお 2020年4月時点では Dv3 または Ev3 の仮想マシンを作成した後に、以下の Hyper-V の有効化コマンドの実行は不要なようです。
>
> ```powershell
> # Windows Server の場合
> Install-WindowsFeature -Name Hyper-V -IncludeManagementTools -Restart
> ```
>
> または
>
> ```powershell
> # Windows 10 の場合
> Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All -Restart
> ```
>
> もし Docker Desktop の起動時にエラーメッセージが表示されるようであれば、一度 Docker Desktop をアンインストールしてから上記の Hyper-V 有効化コマンドを実行してください。

<br />

---

## Visual Studio Code

[Visual Studio Code](https://code.visualstudio.com/) で Visual Studio Code のインストーラーをダウンロードします。

<br />

<img src="./images/01/vscode_download.jpg" width="560px" />

<br />

---

## Azure IoT Tools

[Azure IoT Tools](https://marketplace.visualstudio.com/items?itemName=vsciot-vscode.azure-iot-tools) をインストールします。  
VSCode の [**拡張機能**] を開き、"**azure iot tools**" などで検索してインストールします。

Azure IoT Tools は Visual Studio Code の拡張機能で、Azure IoT (IoT Hub, IoT Edge) 開発に必要なツールです。

<br />

<img src="./images/01/vscode_install_iottools.jpg" width="560px" />

<br />

インストールが完了しすると "**AZURE IOT HUB**" メニューが表示されます。
<br />

<img src="./images/01/iottools_installed.jpg" width="560px" />

<br />

---

## Docker Desktop

IoT Edge モジュールを開発するには、開発用 PC に Docker Desktop が必要です。

[Docker Desktop のダウンロード ページ](https://www.docker.com/products/docker-desktop) からダウンロードして、インストールします。

<br />

<img src="./images/01/docker_download.jpg" width="560px" />
<img src="./images/01/docker_installing.jpg" width="480px" />
<img src="./images/01/docker_installed.jpg" width="480px" />

<br />

OS の再起動後に Docker Desktop が起動すればインストール完了です。

<br />

<img src="./images/01/docker_running.jpg" width="480px" />

<br />

---

## Anaconda

Anaconda または Python は、このハンズオンでは不要です。  

ただし同様のアプリケーションを開発する場合は、Python のコードを編集したりデバッグしたりする必要が出てきます。  
このタイミングで Anaconda または Python をインストールすることをお勧めします。

Anaconda は [Anaconda のダウンロードページ](https://www.anaconda.com/distribution/#download-section) からダウンロードできます。  
Python は Windows ストアで "Python" で検索するか、[Python.org のダウンロードページ](https://www.python.org/downloads/) からダウンロードしてください。

---

以上で、アプリケーション開発に必要な環境が構築できました。

次は Custom Vision で画像分類器を作成します。

[次に進む](./02_custom_vision.md)  
[目次に戻る](./README.md)