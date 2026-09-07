python -m venv .venv


source .venv/bin/activate
Create requirements.txt with list of libraries
pip install -r requirements.txt
save the model into a pickle file using joblib

created API server as main.python
load model and create HTTP endpoint
create dockerfile
uvicorn main:app --reload --host 127.0.0.1 --port 8080

curl -X POST "http://localhost:8080/predict" -H "Content-Type: application/json" -d @testInput.json