# Deploy con Docker

## Requisitos
- Docker Desktop.
- MongoDB.

## Docker local
1. Crea tu `.env` a partir de `.env.example` y completa valores.
2. Construye la imagen:
   `docker build -t hackaton16-chat .`
3. Ejecuta el contenedor:
   `docker run --name hackaton16-chat --env-file .env -p 9000:9000 hackaton16-chat`
4. Verifica:
   - `http://localhost:9000/health` o directamente `http://localhost:9000/`
5. Detener y eliminar (opcional):
   `docker stop hackaton16-chat`
   `docker rm hackaton16-chat`

