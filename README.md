# Express MongoDB Authentication API

API REST desarrollada con Node.js, Express y MongoDB Atlas, implementando el patrón de arquitectura MVC/Repository, autenticación basada en JWT (JSON Web Token) y pipeline de integración y despliegue continuo (CI/CD) con GitHub Actions y Render.

## 🔗 Enlaces del Proyecto

- **API en Producción (Render):** [https://express-mongo-auth-r41b.onrender.com/api/users/](https://express-mongo-auth-r41b.onrender.com/api/users/)
- **Repositorio de GitHub:** [https://github.com/CalepNeyra/express-mongo-auth-](https://github.com/CalepNeyra/express-mongo-auth-)

---

## 🔑 Credenciales de Prueba

Para probar los endpoints autenticados y protegidos con JWT desde **Postman** o **Thunder Client**, utilice las siguientes credenciales:

- **Email:** `neyrataype@tecsup.edu.pe`
- **Password:** `123456`

---

## 🧪 Guía de Pruebas de Endpoints

### 1. Obtener Lista de Usuarios / Estado del Servicio
- **Método:** `GET`
- **URL:** `https://express-mongo-auth-r41b.onrender.com/api/users/`
- **Respuesta:** Status `200 OK` con la lista de usuarios en formato JSON.

### 2. Autenticación / Login (Obtener JWT Token)
- **Método:** `POST`
- **URL:** `https://express-mongo-auth-r41b.onrender.com/api/users/login`
- **Headers:** `Content-Type: application/json`
- **Body (raw JSON):**
  ```json
  {
    "email": "neyrataype@tecsup.edu.pe",
    "password": "123456"
  }
