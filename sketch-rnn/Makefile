API_KEY=;alsjfpoaisfasfjas;lfkjas;dlkfaf

post:
	@echo "Processing POST prediction request.."
	@curl \
	-H "Content-Type: application/json" \
	-d '{"i":"0","strokes":"[[-4, 0, 1, 0, 0],[-15, 9, 1, 0, 0],[-10, 17, 1, 0, 0],[-1, 28, 1, 0, 0],[14, 13, 1, 0, 0],[12, 4, 1, 0, 0],[22, 1, 1, 0, 0],[14, -11, 1, 0, 0],[5, -12, 1, 0, 0],[2, -19, 1, 0, 0],[-12, -23, 1, 0, 0],[-13, -7, 1, 0, 0],[-14, -1, 0, 1, 0]]"}' \
	-X POST http://127.0.0.1:8080/simple_predict
	@echo ""

get:
	@echo "Processing GET prediction request.."
	@curl \
	-H "Content-Type: application/x-www-form-urlencoded" \
	-X GET \
	-d strokes="[[-4, 0, 1, 0, 0],[-15, 9, 1, 0, 0],[-10, 17, 1, 0, 0],[-1, 28, 1, 0, 0],[14, 13, 1, 0, 0],[12, 4, 1, 0, 0],[22, 1, 1, 0, 0],[14, -11, 1, 0, 0],[5, -12, 1, 0, 0],[2, -19, 1, 0, 0],[-12, -23, 1, 0, 0],[-13, -7, 1, 0, 0],[-14, -1, 0, 1, 0]]" \
	http://127.0.0.1:8080/simple_predict
	@echo ""