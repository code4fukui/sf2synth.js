sf2synth.js
===========

sf2synth.js は [WebMidiLink](http://www.g200kg.com/en/docs/webmidilink/) 対応の SoundFont シンセサイザです。


## 使い方

```js
import { SoundFont } from "https://code4fukui.github.io/sf2synth.js/SoundFont.js";

const wml = new SoundFont.WebMidiLink();

btn.onclick = () => {
  const url = "https://imaya.github.io/demo/sf2.js/soundfont/A320U.sf2";
  wml.setLoadCallback(function(arraybuffer) {
    // loaded
  });
  wml.setup(url);
};
```


## 対応ブラウザ

最新の Web Audio API 実装を必要とします。

- Google Chrome 25+
- Google Chrome for Android 28+


## WebMidiLink 対応

sf2synth.js は WebMidiLink の Link Level 1 に対応しています。
現在、シンセサイザ固有の情報はありません。


## ライセンス

Copyright &copy; 2013 imaya / GREE Inc.
Licensed under the MIT License.
