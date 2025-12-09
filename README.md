# Proyecto-completo-David-Baquero-
Proyecto Final SENA

el repositorio contiene el proyecto final desarrollado. El sistema está compuesto por tres partes principales: el backend desplegado en Render, el frontend desplegado en Netlify y la base de datos alojada en Railway.

Tecnologías Utilizadas
Frontend

HTML, CSS, JavaScript

Framework (según corresponda: React, Vue, Angular)

Despliegue en Netlify

Backend

Node.js con Express (o framework utilizado en el proyecto)

Autenticación con JWT

ORM (Sequelize, Prisma, Mongoose, etc.)

Despliegue en Render

Base de Datos

MySQL, PostgreSQL o MongoDB (según el proyecto)

Alojamiento en Railway

Arquitectura General

El proyecto se organiza de la siguiente manera:

Frontend (Netlify) → Backend API (Render) → Base de datos (Railway)

URLs del Proyecto
Componente	URL
Frontend (Netlify)	

Backend (Render)	

Base de datos	Conexión privada configurada desde Railway

Reemplazar las URLs por las definitivas una vez desplegadas.

Instalación y Ejecución en Local
Clonar el repositorio
git clone 
cd proyecto-sena

Configuración del Backend
Instalación de dependencias
npm install

Variables de entorno

Crear un archivo .env con los siguientes valores:

PORT=3000
DATABASE_URL="URL de conexión de Railway"
JWT_SECRET="clave_segura"

Ejecutar servidor en desarrollo
npm run dev

Configuración del Frontend

Si usa un framework:

npm install
npm run dev


Si es HTML/CSS/JS puro, solo abrir el archivo index.html.

Estructura de la Base de Datos (Railway)

Ejemplo de estructura (ajustar según el proyecto):

usuarios
  - id (PK)
  - nombre
  - email
  - contraseña

citas
  - id (PK)
  - fecha
  - usuario_id (FK)

Documentación de la API

Ejemplos de endpoints (completar según el backend real):

GET /api/usuarios

Devuelve la lista de usuarios.

POST /api/auth/login

Realiza el proceso de inicio de sesión y retorna un token JWT.

POST /api/registro

Crea un nuevo usuario.

Pruebas

Pruebas unitarias (si se implementaron)

Pruebas manuales mediante herramientas como Postman o Thunder Client

Despliegue
Backend en Render

Crear servicio web en Render

Conectar el repositorio

Configurar variables de entorno

Ejecutar el despliegue

Frontend en Netlify

Crear un nuevo sitio desde Git

Seleccionar el repositorio

Configurar comando de build (si aplica)

Desplegar

Base de Datos en Railway

Crear una instancia de base de datos

Obtener la URL de conexión

Configurarla en el backend como variable de entorno