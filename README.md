# Errores comunes

Tip: La mayoría de veces los errores se pueden solucionar leyendo los logs de los contenedores con detenimiento.
Por favor, siempre seguir el siguiente formato:
- Título del Error encontrado
- Descripción (Si es necesaria)
- Causa del error
- Solución
Si el error se podía haber evitado leyendo documentación que no existia comunicarlo a los superiores y **crear la documentación** pertinente en los repositorios de documentación ([enlaces en este documento](https://github.com/governify/seville-devops-docs#readme))
## Listado
[Error-001](#error-001) Contenedor de mongo se resetea continuamente, no hay conexión con el servidor desde internet





a

a

a
a

a
a

a



a

a

a

a

a

a

a

a

a

---
### Error-001 
**Contenedor de mongo se resetea continuamente, no hay conexión con el servidor desde internet**
- **Causa:**
  Se ha hecho un pull y un up de docker compose y la version de mongo no es compatible (En el log del contenedor lo dice en un mensaje)
![image](https://github.com/governify/seville-devops-docs/assets/91433995/4db74905-ae9a-427d-aea0-8687fe8cdb0b)

- **Solución:**
  En /home/ubuntu/governify/bluejay-infrastructure/docker-bluejay/docker-compose.yaml cambiar la version de mongo a una compatible hacer up del contenedor y resetear el nginx-streamer:
![image](https://github.com/governify/seville-devops-docs/assets/91433995/c3ba0b38-9254-40a1-ac2b-15c3d15a5935)


  
