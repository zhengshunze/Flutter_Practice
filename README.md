# Flutter_Practice
**0. 簡介與安裝**

☞ 安裝以下 \
[Android Studio](https://developer.android.com/studio) \
[Git](https://git-scm.com/downloads) \
[Flutter](https://docs.flutter.dev/get-started/install)

並將Flutter SDK 至所需安裝位置（例如，C:\src\flutter），並進入路徑打開CMD，輸入以下指令。
```
git clone https://github.com/flutter/flutter.git -b stable
```
⚡**警告**
- 不要將 Flutter 安裝到包含特殊字符或空格的路徑。
- 不要將 Flutter 安裝在 C:\Program Files\需要提升權限的目錄中。 

☞ 進入C:\src\flutter，雙擊執行flutter_console.bat，並輸入已下指令，來檢查是否完成必要的環境安裝項目。
```
flutter doctor
```
務必確認 Flutter、Android toolchain、Android Studio 這三個一定要有綠色打勾
![image](https://user-images.githubusercontent.com/77151276/163722113-4784ce28-6203-4895-997b-b7b30adf9f81.png)

⚡**問題與排解**
- 未安裝cmdline-tool
```cmdline-tools component is missing
      Run `path/to/sdkmanager --install "cmdline-tools;latest"`
      See https://developer.android.com/studio/command-line for more details.
```
★ 安裝Android Studio後打開並安裝SDK後，至點選左側的 Customize ，找到右邊底下的 All settings... 並進入 Appearance & Behavior | System Settings | Android SDK ，切換到SDK Tools 頁籤中，將 Android SDK Command-line Tools (latest) 選項打勾後按Apply即完成安裝。
- 尚未同意Android license
```
Some Android licenses not accepted.  To resolve this, run: flutter doctor --android-licenses 
```

