
# Fake mute/deafen

1. Join voice channel
2. mute and deafen youself
3. execute the script
4. unmute and speak!

```js
var text = new TextDecoder("utf-8");

WebSocket.prototype.original = WebSocket.prototype.send;
WebSocket.prototype.send = function(data) {
    if (Object.prototype.toString.call(data) === "[object ArrayBuffer]") {
        if (text.decode(data).includes("self_deaf")) data = data.replace('"self_mute":false', 'NashyLove');
    }
    WebSocket.prototype.original.apply(this, [data]);
}
```
