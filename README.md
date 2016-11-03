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

You can see it working at: https://fernandezpaco.github.io/webrtc-peer/index.html

If you need a turn/stun server you can pass the configuration to the iceconfig propertie, something like this:

 yourcomponent.iceconfig= {"iceServers" : [ {
        "url" : "turn:yourturnip:3478",
        "username" : "youruser",
        "credential" : "yourpwd"
    } ]}
