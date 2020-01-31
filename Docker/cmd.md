docker build -t flaskapp:latest .
docker run -v /"path"/:/app -p 8080:5000  flaskapp:latest
