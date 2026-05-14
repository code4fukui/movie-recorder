# movie-recorder

MediaRecorder API を使用して構築された、ブラウザ上で動作するオープンソースの動画録画アプリケーションです。カメラとマイクから直接クライアントサイドで動画と音声を録画できます。

## デモ

[https://code4fukui.github.io/movie-recorder/](https://code4fukui.github.io/movie-recorder/)

![movie-recorderのユーザーインターフェースのスクリーンショット。大きな動画プレビュー領域が表示されています。その上部には、カメラの選択ドロップダウン、"反転"（Flip）のチェックボックス、動画形式（例: video/mp4）の選択ドロップダウン、および"録画開始"（Start Recording）、"録画停止"（Stop Recording）、"ダウンロード"（Download）の3つのボタンが含まれたコントロールバーが配置されています。](https://user-images.githubusercontent.com/1552733/235272189-7013f990-250a-426c-829d-536f01538f97.png)

## 機能

- **クライアントサイドでの録画**: 動画の録画および処理はすべてブラウザ内で行われます。サーバーにデータは送信されません。
- **カメラ選択**: 使用可能なすべての動画入力デバイスを一覧表示し、選択できます。
- **音声と動画**: カメラからの動画とマイクからの音声を同時にキャプチャします。
- **動画のミラーリング**: 自撮りスタイルの録画に最適な「反転」オプション（デフォルトで有効）で、動画プレビューをミラー表示します。
- **形式選択**: ブラウザがサポートする動画形式（例: `video/mp4`、`video/webm`）を自動検出し、選択できます。
- **即時ダウンロード**: 録画を停止するとすぐに、録画データを動画ファイルとしてダウンロードできます。

## 使い方

1. プロンプトが表示されたら、ブラウザがカメラとマイクへアクセスすることを許可します。
2. 最初のドロップダウンメニューから使用するカメラを選択します。
3. （オプション）**反転**（Flip）チェックボックスのチェックを外して、動画のミラーリングを無効にします。
4. **Type** ドロップダウンから希望する動画形式（例: `video/mp4`）を選択します。
5. **録画開始**（Start Recording）ボタンをクリックして録画を開始します。
6. 終了したら、**録画停止**（Stop Recording）ボタンをクリックします。
7. **ダウンロード**（Download）ボタンをクリックして、動画ファイルをコンピュータに保存します。

## 使用技術

- HTML5 & Vanilla JavaScript
- [MediaDevices API](https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices) (`getUserMedia`, `enumerateDevices`)
- [MediaStream Recording API](https://developer.mozilla.org/en-US/docs/Web/API/MediaRecorder_API) (`MediaRecorder`)

## ライセンス

MIT License — 詳細は [LICENSE](LICENSE) を参照してください。
