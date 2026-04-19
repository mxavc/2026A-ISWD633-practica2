# COMPLETAR  
Comparando sus conocimientos antes de hacer la práctica con sus conocimientos después de hacer la tarea, explicar los principales aprendizajes logrados para beneficio de su formación profesional.  

El principal aprendizaje fue comprender cómo Docker gestiona redes, contenedores y persistencia de datos, y cómo aplicar buenas prácticas para manejar información sensible con Docker Secrets. Además, se resolvió un problema de conexión entre contenedores (pgAdmin ↔ Postgres) creando una red personalizada, lo que reforzó la importancia de la configuración de redes en entornos de contenedores.

Si solucionó un problema presentado al realizar la práctica también se debe documentar.
Esta documentado en la seccion 2-ejercicio.md


Consultar: Cómo se gestionan datos confidenciales con los secretos de Docker (Docker Secrets).
Docker Secrets permiten almacenar información sensible (contraseñas, claves SSH, certificados) de forma encriptada y segura dentro de un clúster Docker Swarm.

Características principales:

Encriptación: los secretos se guardan cifrados en reposo y en tránsito.

Acceso controlado: solo los servicios autorizados pueden leerlos.

Montaje seguro: se exponen como archivos de solo lectura dentro del contenedor, nunca en variables de entorno ni en logs.

Centralización: se gestionan desde el Swarm, evitando que credenciales queden en Dockerfiles o repositorios.