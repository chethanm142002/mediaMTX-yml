# mediaMTX-yml
# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.







//run mediaMTX
<!-- E:
dir
folder path cd E:\mediamtx_v1.17.0_windows_amd64
run :  .\mediamtx.exe -->

//mediamtx
<!-- add camera path, source
exmple: Camera IP + username + Password 
this 3 we get a URL for live video -->

//VLC play
<!-- media -> open network stream -> add URL 
ex url  rtsp://admin:G%40nd66v%40N@192.168.103.203:554/stream1 
web url http://localhost:8888/cam2/index.m3u8 -->

video compresser
runOnRecordSegmentComplete: ffmpeg -i $MTX_SEGMENT_PATH -vcodec libx264 -crf 28 -preset veryfast ${MTX_SEGMENT_PATH%.mp4}_small.mp4




| Recording        |  Enabled    |
| Format           |  MP4 (fMP4) |
| Segment duration |  20 minutes |
| Files per hour   |  ~3 files   |
| Files per day    |  ~72 files  |
| Auto delete      |  3 days     |
| Compression      |  FFmpeg     |
