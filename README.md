# FlvPlayer

[![Build Status](https://www.travis-ci.org/zhw2590582/FlvPlayer.svg?branch=master)](https://www.travis-ci.org/zhw2590582/FlvPlayer)
![version](https://badgen.net/npm/v/flvplayer)
![license](https://badgen.net/npm/license/flvplayer)
![size](https://badgen.net/bundlephobia/minzip/flvplayer)
[![npm Downloads](https://img.shields.io/npm/dt/flvplayer.svg)](https://www.npmjs.com/package/flvplayer)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![dependencies Status](https://david-dm.org/zhw2590582/flvplayer/status.svg)](https://david-dm.org/zhw2590582/flvplayer)

> FlvPlayer.js is a JavaScript player for decode flv to the canvas

## Demo
[Play online demo](https://flvplayer.js.org/)

[Play local demo](https://flvplayer.js.org/fileReader.html)

## Install

Install with `npm`

```bash
$ npm install flvplayer
```

Or install with `yarn`

```bash
$ yarn add flvplayer
```

```js
import FlvPlayer from 'flvplayer';
import 'flvplayer/dist/flvplayer.css';
```

Or umd builds are also available

```html
<link rel="stylesheet" href="path/to/flvplayer.css" />
<script src="path/to/flvplayer.js"></script>
```

Will expose the global variable to `window.FlvPlayer`.

## Usage

```html
<div class="flvplayer-app"></div>
```

```js
var flv = new FlvPlayer({
    container: '.flvplayer-app', // A div dom element
    url: 'path/to/video.flv', // Url of flv video file
    videoDecoder: './baselineProfileDecoder.js', // Path to video decoder, baselineProfileDecoder.js or allProfileDecoder.js
    poster: 'path/to/poster.png', // Url of video poster, the first frame of the video is taken as the poster by default
    debug: false, // Show debug information on developer tools
    live: false, // Whether live video
    loop: false, // Whether to automatically loop play
    hotkey: true, // Whether to use hotkeys
    controls: true, // Whether to display the controller
    hasAudio: true, // Whether to include audio
    volume: 7, // Default volume, ranging from 0 to 10
    frameRate: 30, // Video frame rate, which will be extracted from the flv file by default
    width: 400, // Video default width, which will be extracted from the flv file by default
    height: 300, // Video default height, which will be extracted from the flv file by default
});
```

## QQ Group

![QQ Group](./QQgroup.png)

## License

MIT © [Harvey Zack](https://sleepy.im/)
