# HRT
HRTTotK is a tools to track visited locations in a 100% run of TotK. It works by monitoring the streamed game frames from a camera / video and detecting if the frames contain location names.

This repo was branched from [HRT for BotW](https://github.com/minghaob/HRT). It is currently still in work-in-progress state.

## How to Build
1. Install [Visual Studio 2022](https://visualstudio.microsoft.com/vs/).
2. Install [vcpkg](https://github.com/microsoft/vcpkg).
3. Open command line in vcpkg folder and run the following commands to build OpenCV and Tesseract, and integrate vcpkg into Visual Studio.
```
vcpkg install opencv4[world]:x64-windows-static
vcpkg install tesseract:x64-windows-static
vcpkg integrate install
```
4. Download the latest ffmpeg build [here](https://github.com/BtbN/FFmpeg-Builds/releases). (Get **ffmpeg-master-latest-win64-lgpl-shared.zip**, you might need to click "Show all 50 assets" to find it.) Extract its contents to the root folder of this repository.
5. Open "HRT.sln" and build. Find the artifacts in the "bin" folder.

## Acknowledgements
HRT uses the following libraries:

### Tesseract
https://github.com/tesseract-ocr/tesseract

### OpenCV
https://github.com/opencv/opencv

### FFmpeg
https://github.com/FFmpeg/FFmpeg

### Simple-Web-Server and Simple-WebSocket-Server
https://gitlab.com/eidheim/Simple-Web-Server

https://gitlab.com/eidheim/Simple-WebSocket-Server
