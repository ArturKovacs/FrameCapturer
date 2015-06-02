# FrameCapturer

FrameCapturer is a plug-in for Unity that allow you to capture frame buffer and export to image or movie files. Currently supported are gif and exr.

## Gif Capturer
features:
- Keeps last N frames on memory and write a part of it to file later (similar to ShadowPlay or PS4)
- Async & parallel encoding
- In-game previewer and simple editor
- Supports D3D9, D3D11 and OpenGL graphics APIs, x86 and x86-64 architectures. (Confirmed only on Windows)

demo video:
[![FrameCapturer: GifRecorder](http://img.youtube.com/vi/VRmVIzhxewI/0.jpg)](http://www.youtube.com/watch?v=VRmVIzhxewI)  

examples: this image is exported by this plug-in. (This scene is included in this repository)  
![example1](Screenshots/gif_example1.gif)  

### Usage
1. Import [this package](https://github.com/unity3d-jp/FrameCapturer/blob/master/Packages/GifRecoder.unitypackage?raw=true) to your project
2. Add GifCapturer component to camera that you want to record
3. Place GifCapturerHUD.prefab (uGUI object) to somewahere, and set GifCapturer (that added in 2.) to its capturer parameter

3 is not required, but GifCapturer needs GUI or scripts to turn on/off recording, write to file, etc. Modifing GifCapturerHUD.prefab is good way to make your own GUI.  


## Exr Capturer  
ExrCapturer can export G-Buffer. But currently unstable and many features are work in progess.