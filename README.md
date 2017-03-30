# Camera-Image-In-Background

This sample app uses AVFoundation to take a Still Image in the background as soon as the app loads.

The app is updated for Xcode 8.2 & Swift 3

Updated in iOS SDK 10 :

* [AVCapturePhotoOutput](https://developer.apple.com/reference/AVFoundation/AVCapturePhotoOutput)
* [AVCapturePhotoSettings](https://developer.apple.com/reference/avfoundation/avcapturephotosettings)

This fucntion is called by the **AVCapturePhotoOutput** with **AVCapturePhotoSettings** as settings and **AVCapturePhotoCaptureDelegate** type of class as delegate

```sh
capturePhoto(with settings: AVCapturePhotoSettings, delegate: AVCapturePhotoCaptureDelegate)
```

The delegate function on the image clicked is from which the image can be retrieved as Data
```sh
capture(_ captureOutput: AVCapturePhotoOutput, didFinishProcessingPhotoSampleBuffer photoSampleBuffer: CMSampleBuffer?, previewPhotoSampleBuffer: CMSampleBuffer?, resolvedSettings: AVCaptureResolvedPhotoSettings, bracketSettings: AVCaptureBracketedStillImageSettings?, error: Error?)
```
