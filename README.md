docker build -t qrcode-generator:1.0 .
docker run --env-file .env -p 8080:8080 qrcode-generator:1.0
