# movie-recorder

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

An open-source, browser-based video recorder application built with the MediaRecorder API. It allows you to record video and audio from your camera and microphone directly on the client-side.

## Demo

[https://code4fukui.github.io/movie-recorder/](https://code4fukui.github.io/movie-recorder/)


![A screenshot of the movie-recorder user interface. It shows a large video preview area. Above it, a control bar contains a dropdown to select a camera, a checkbox labeled "反転" (Flip)
, a dropdown to select the video type (e.g., video/mp4), and three buttons: "録画開始" (Start Recording), "録画停止" (Stop Recording), and "ダウンロード" (Download).](https://user-images.githubusercontent.com/1552733/235272189-7013f990-250a-426c-829d-536f01538f97.png)

## Features

-   **Client-Side Recording**: Records and processes video entirely in your browser. No data is sent to a server.
-   **Camera Selection**: Lists and allows you to choose from all available video input devices.
-   **Audio & Video**: Captures both video from your camera and audio from your microphone.
-   **Video Mirroring**: Includes a "Flip" option (enabled by default) to mirror the video preview, ideal for selfie-style recording.
-   **Format Selection**: Automatically detects and lets you choose from browser-supported video formats (e.g., `video/mp4`, `video/webm`).
-   **Instant Download**: Download your recording as a video file as soon as you stop.

## Usage

1.  Allow the browser to access your camera and microphone when prompted.
2.  Select your desired camera from the first dropdown menu.
3.  (Optional) Uncheck the **反転** (Flip) checkbox to disable video mirroring.
4.  Choose the desired video format (e.g., `video/mp4`) from the **Type** dropdown.
5.  Click the **録画開始** (Start Recording) button to begin.
6.  When finished, click the **録画停止** (Stop Recording) button.
7.  Click the **ダウンロード** (Download) button to save the video file to your computer.

## Built With

-   HTML5 & Vanilla JavaScript
-   [MediaDevices API](https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices) (`getUserMedia`, `enumerateDevices`)
-   [MediaStream Recording API](https://developer.mozilla.org/en-US/docs/Web/API/MediaRecorder_API) (`MediaRecorder`)

## License

MIT License — see [LICENSE](LICENSE).