Sistema de Autenticación Completo (React + Flask)

# AUTOR : Diego Sanchez Chuquimango

Este proyecto implementa un sistema de autenticación completo que incluye registro, inicio de sesión y gestión de usuarios utilizando React para el frontend y Flask para el backend. Los tokens JWT se utilizan para manejar la autenticación segura.

Tabla de Contenidos

Requisitos

Estructura del Proyecto

Configuración del Backend

Configuración del Frontend

Uso

Rutas del Backend

Tecnologías Utilizadas

Mejoras Futuras

Requisitos

Python 3.8 o superior

Node.js 14.x o superior

npm o Yarn

SQLite (preinstalado con Python)

Flask y sus dependencias

Librerías de React como axios y react-router-dom

Estructura del Proyecto

/project
├── backend/                  # Código del backend en Flask
│   ├── app.py
│   ├── models.py
│   ├── extensions.py
│   ├── requirements.txt
├── frontend/                 # Código del frontend en React
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   ├── package.json
├── README.md

Configuración del Backend

Clona el repositorio y accede al directorio backend:

cd backend

Instala las dependencias:

pip install -r requirements.txt

Crea la base de datos:

python app.py create_db

Ejecuta el servidor Flask:

python app.py

El backend estará disponible en http://127.0.0.1:5000.

Configuración del Frontend

Accede al directorio frontend:

cd frontend

Instala las dependencias:

npm install

Inicia el servidor de desarrollo:

npm start

El frontend estará disponible en http://localhost:3000.

Uso

Registro

Accede a http://localhost:3000/register.

Ingresa tu email y contraseña para crear una cuenta.

Inicio de Sesión

Accede a http://localhost:3000/login.

Ingresa tus credenciales para obtener un token JWT.

Acceso Protegido

Usa el token JWT para realizar solicitudes autenticadas al backend.

Rutas del Backend

Método

Ruta

Descripción

POST

/auth/register

Registra un nuevo usuario

POST

/auth/login

Genera un token JWT para el usuario

GET

/protected

Ejemplo de ruta protegida

Tecnologías Utilizadas

Frontend

React

Axios

React Router DOM

jwt-decode

Backend

Flask

Flask-JWT-Extended

SQLAlchemy

SQLite

Mejoras Futuras

Implementar un sistema de recuperación de contraseñas.

Añadir validación más robusta en los formularios.

Implementar roles y permisos de usuario.

Mejorar la seguridad utilizando HTTPS y almacenamiento seguro de tokens.

