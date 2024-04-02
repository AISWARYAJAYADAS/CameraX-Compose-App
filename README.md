# CameraXComposeApp

## Overview

This Android app leverages Jetpack Compose and CameraX library to provide camera functionality for
capturing photos and recording videos.

## Features

- Switch between front and back cameras.
- Capture photos with rotation correction.
- Record videos with audio.
- Display captured photos in a staggered grid layout.

## Usage

1. Ensure necessary permissions (camera and audio recording) are granted.
2. Use the camera switch icon to toggle between front and back cameras.
3. Click the "Take Photo" icon to capture a photo with rotation correction.
4. Click the "Record Video" icon to start/stop recording videos with audio.
5. Captured photos are displayed in a staggered grid layout below the camera preview.

## Components

- **MainActivity**: Controls the app flow and sets up the camera preview and UI.
- **MainViewModel**: Manages the state of captured photos using a ViewModel.
- **CameraPreview**: Displays the camera preview using a Compose composable.
- **PhotoBottomSheetContent**: Displays the captured photos in a staggered grid layout using a
  Compose composable.

## Dependencies

- **Jetpack Compose**: Used for building the UI declaratively.
- **CameraX**: Provides camera functionality abstraction.
    - `androidx.camera.core`: Core library using the camera2 implementation.
    - `androidx.camera.camera2`: CameraX Camera2 library.
    - `androidx.camera.lifecycle`: CameraX Lifecycle library.
    - `androidx.camera.video`: CameraX VideoCapture library.
    - `androidx.camera.view`: CameraX View class.
    - `androidx.camera.mlkit.vision`: CameraX ML Kit Vision Integration.
- **AndroidX Material Icons Extended**: Provides extended Material icons support.
- **AndroidX Lifecycle ViewModel Compose**: ViewModel integration for Jetpack Compose.

## Permissions

Ensure the following permissions are added to your app's manifest file:

```xml
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>

## Requirements
- Android device running Android 5.0 (API level 21) or higher.
- Permissions for camera and audio recording.
