PARA EXECUTAR
- gerar o container
docker build -t qrcode-generator:1.0 .

- criar o arquivo .env e se setar 
AWS_ACCESS_KEY_ID
AWS_SECRET_ACCESS_KEY

- executar 
docker run --env-file .env -p 8080:8080 qrcode-generator:1.0

- chamar o endpoint
 http://localhost:8080/qrcode
 com o link
{
    "text":"https://www.link.com.br"
}

