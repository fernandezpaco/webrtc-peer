# webrtc-peer
webrtc peer using peerjs

You can use it to call or to receive calls.

Caller:
```html
<video-camera id="mywebcam" stream="{{stream}}"></video-camera>
<video-camera id="peerstream" waitforinput="true" stream="[[peerstream]]"></video-camera>
<webrtc-peer peerjskey="your key" peerid_tocall="[[peer id to call]" stream="[[stream]]" peerstream="{{peerstream}}">
</webrtc-peer>
```
Receiver:
```html
<video-camera id="mywebcam" stream="{{stream}}"></video-camera>
<video-camera id="peerstream" waitforinput="true" stream="[[peerstream]]"></video-camera>
<webrtc-peer peerjskey="your key" stream="[[stream]]" peerstream="{{peerstream}}">
</webrtc-peer>
```
