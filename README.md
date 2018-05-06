# robosketch-rnn

Let a robot continue your drawings using SketchRNN.

## How it works

Three main pieces enable us to (1) draw, (2) predict the continuation of our sketch, and (3) tell the robot to draw them physically.

These three pieces are:

- Machina Bridge · an app that connects to a robot and creates a WebSocket server to give the robot instructions
- SketchRNN · a neural network that predicts how to continue a sketch from an input drawing, server as an HTTP service
- p5js · a drawing application that requests predictions from the SketchRNN services and tells the robot to draw them on paper

## Usage

- Connect to the robot with [Machina Bridge](Machina-Bridge_v0.1.0)
	- Execute `Machina-Bridge_v0.1.0/MachinaBridge.exe`.
	- Choose the make of your robot (e.g., UR).
	- Write the local IP of your robot (e.g., 192.168.0.172).
	- Click `Connect`.
	- (The Machina Bridge app should be now connected to the robot.)
- Start [SketchRNN](sketch-rnn) as an HTTP service
	- Go to the sketch-rnn folder.
	- Run `npm install`.
	- Run `node http-server.js`.
- Open the p5js drawing app's [index.html](p5js-sketch-rnn-draw-http/index.html)

## p5js drawing app commands

Here are the keystrokes you can use to control the p5js drawing app.

- `p` · request a prediction to SketchRNN
- `s` · toggle prediction visibility
- `h` · send robot *home*
- `r` · tell the robot to *draw* the latest doodle
- `c` · clean existing drawing

## Troubleshooting

- `node-gyp` only works with Python 2.7, make sure this is the version you have installed and the one referenced by npm.
- Install Visual C++ redistributable tools?
