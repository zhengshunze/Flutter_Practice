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


- 未安裝 Android Studio
```
[X] Android toolchain - develop for Android devices
    X Unable to locate Android SDK.
      Install Android Studio from: https://developer.android.com/studio/index.html
      On first launch it will assist you in installing the Android SDK components.
      (or visit https://flutter.dev/docs/get-started/install/windows#android-setup
      for detailed instructions).
      If the Android SDK has been installed to a custom location, please use
      `flutter config --android-sdk` to update to that location.
```
★ ***解決方法*** 

進入developer.android.com/studio?hl=zh-tw 官網下載Android Studio，安裝項目如下:

<img width="747" alt="image" src="https://github.com/zhengshunze/Flutter_Practice/assets/77151276/33509451-9707-4b6f-ba94-4be6c3483472">



- 未安裝Visual Studio 之 MSVC
```
[!] Visual Studio - develop Windows apps (Visual Studio Community 2022 17.9.5)
    X Visual Studio is missing necessary components. Please re-run the Visual Studio
      installer for the "Desktop development with C++" workload, and include these
      components:
        MSVC v142 - VS 2019 C++ x64/x86 build tools
         - If there are multiple build tool versions available, install the latest
        C++ CMake tools for Windows
        Windows 10 SDK
```
★ ***解決方法*** 
進入Visual Studio Installer 修改 安裝內容 將 Desktop development with C++ 打勾後按下修改。


- 未安裝cmdline-tool
```cmdline-tools component is missing
      Run `path/to/sdkmanager --install "cmdline-tools;latest"`
      See https://developer.android.com/studio/command-line for more details.
```

★ ***解決方法*** \
安裝Android Studio後打開並安裝SDK後，至點選左側的 Customize ，找到右邊底下的 All settings... 並進入 Appearance & Behavior | System Settings | Android SDK ，切換到SDK Tools 頁籤中，將 Android SDK Command-line Tools (latest) 選項打勾後按Apply即完成安裝。

<hr>

- 尚未同意Android license
```
Some Android licenses not accepted.  To resolve this, run: flutter doctor --android-licenses 
```

★ ***解決方法*** \
在cmd 打 'flutter doctor --android-licenses' 並一直輸入'y'即可。

若報錯，請將 ' C:\src\flutter\bin ' 加入系統/使用者 Path環境變數 即可。
![image](https://user-images.githubusercontent.com/77151276/163722754-be03edcc-47f9-4ffb-8926-2e2a700aaa2c.png)
