# Backend

El backend del proyecto se va a implementar en Python, y consiste en:

* una API REST elaborada con FastAPI, que gestiona el acceso a todas las funciones de la aplicación
* un servidor web (uvicorn)
* una base de datos SQLite

<<<<<<< HEAD
=======
Está almacenado en DigitalOcean.

Para activar el servidor:
* Desarrollo: `uvicorn main:app --reload` (no accesible desde el exterior; incluye hot reload)
* Producción: `uvicorn main:app --host 0.0.0.0 --port 8000`

* Firewall activo, abrir el puerto con `ufw allow 8000/tcp` para poder acceder a estos enlaces desde fuera
* API: [134.209.89.62:8000]. Funciones implementadas:
    * "hola mundo" en `/`
    * Descripción en texto a partir de imagen en `/img2txt`
    * Transferencia de estilo en:
        * `blend_images`: transfiere el estilo de la segunda imagen a la primera
        * `blend_image_with_{style}`: transfiere el estilo a la imagen
    * Detección de estilo en `detect_style`
* Documentación autogenerada: [http://134.209.89.62:8000/docs]
>>>>>>> desarrollo-backend
