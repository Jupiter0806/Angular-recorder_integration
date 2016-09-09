**Angular-recorder Integration**

Integrate js plugin named Angular-recorder at https://logbon72.github.io/angular-recorder/

This plugin will choose to use cordova media plugin, or HTML5 navigator.*getUserMedia() and RecorderJS, or falls back to FlashWaveRecorder.

**Installation**
```cmd
bower install angularAudioRecorder
```

import in index.html
```javascript
<!-- library of angularAudioRecorder -->
<script src="lib/angularAudioRecorder/dist/angular-audio-recorder.js"></script>
<!--angularAudioRecorder dependency -->
<script src="lib/wavesurfer.js/dist/wavesurfer.min.js"></script>
```

add dependency to project
```javascript
angular.module('yourAppName', [
    //include other dependencies
    'angularAudioRecorder'
]);
```

add cordova media plugin
```cmd
cordova plugin add cordova plugin add cordova-plugin-media
```

**Test**
Tested on chrome, everything is good
Tested on ios, not good, it always say there is not cordova-media-plugin, even I tried to replace the modified one with the original one


May need to modified it to allow it using cordova-media-plugin