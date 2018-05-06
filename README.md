# robosketch-rnn

Let a robot continue your drawings using SketchRNN.

## Usage

- Open `Machina-Bridge.exe`
	- Choose the make of your robot (e.g., UR).
	- Write the local IP of your robot (e.g., 192.168.0.172).
	- Click `Connect`.
	- (The Machina Bridge app should be now connected to the robot.)
- Start SketchRNN as an HTTP service
	- Go to the sketch-rnn folder.
	- Run `npm install`.
	- Run `node http-server.js`.
- Open the p5js.
	- go to p5js folder
	- `npm install`
	- run `http-server . -o --port xxxx?`
	
	
## Troubleshooting

- `node-gyp` only works with Python 2.7, make sure this is the version you have installed and the one referenced by npm.
- Install Visual C++ redistributable tools?
