Para correr el proyecto de saam usando kubernetes, sigue estos pasos:
1. **Instalar Docker**: Asegúrate de tener Docker instalado en tu máquina.
2. **Configurar .env**: Crea un archivo `.env` en la raíz del proyecto con las varables del backend
3. **Iniciar Docker**: Asegúrate de que Docker esté corriendo.
4. **Ejecutar Docker Compose**: Corre el siguiente comando en la terminal:
   ```bash
   docker compose up -d --build --remove-orphans
   docker service rm saam_saam-backend saam_saam-frontend saam_nginx
   docker stack deploy --with-registry-auth -c docker-compose.yml saam
   ```
5. **Verificar el estado**: Puedes verificar que los contenedores estén corriendo con:
   ```bash
    docker ps
    ```
6. **Acceder a la aplicación**: Entra a la ip de la maquina y nginx en el puerto 80 para ver la aplicación en funcionamiento.
7. **Detener los contenedores**: Para detener los contenedores, usa:
   ```bash
   docker-compose down
   ```