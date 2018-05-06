# SketchRNN Service

SketchRNN as a service. Get drawing predictions from a set of strokes using an HTTP server or a WebSocket client.

## Models

This distribution doesn't come with trained models. Make sure to download at least one, for example https://storage.googleapis.com/quickdraw-models/sketchRNN/large_models/bird.gen.json, rename it to `.js` and put it in `./lib/models`

## HTTP server

Make sure all the necessary modules are installed.

```bash
npm i
```

Start the HTTP server.

```bash
node http-server.js
```

Then test the HTTP server works making a POST request from your Terminal.

```bash
make post
```

Then a GET request.

```bash
make get
```

Now you can try to do the get request on your browser.

Just visit <http://localhost:8080/simple_predict?strokes=[[-4,0,1,0,0],[-15,9,1,0,0],[-10,17,1,0,0],[-1,28,1,0,0]]>.

## WebSocket client

Start the WebSocket client.

```
node websocket-client.js
```

(The server needs to know how to handle the messages.)
