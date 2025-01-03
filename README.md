# Sistema de Autenticación Completo (React + Flask)

Este proyecto implementa un sistema de autenticación con registro, inicio de sesión y manejo de usuarios, utilizando **React** para el frontend y **Flask** para el backend, con autenticación JWT.

## Requisitos

- Python 3.8+
- Node.js 14+
- SQLite (incluido con Python)
- Flask y React con sus dependencias

## Configuración Rápida

### Backend
1. Instala dependencias:
   ```bash
   cd backend
   pip install -r requirements.txt
   ```
2. Crea la base de datos:
   ```bash
   python app.py create_db
   ```
3. Inicia el servidor:
   ```bash
   python app.py
   ```

### Frontend
1. Instala dependencias:
   ```bash
   cd frontend
   npm install
   ```
2. Inicia el servidor:
   ```bash
   npm start
   ```

## Uso

- Registro: `http://localhost:3000/register`
- Inicio de Sesión: `http://localhost:3000/login`
- Ruta Protegida: `http://127.0.0.1:5000/protected` (requiere JWT).

## Tecnologías

- **Frontend:** React, Axios, jwt-decode
- **Backend:** Flask, Flask-JWT-Extended, SQLAlchemy
