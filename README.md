# 🖥️ Backend Node.js — Todo List API REST

API REST desarrollada con Node.js y Express que sirve como backend
para la aplicación de lista de tareas. Gestiona tareas con CRUD completo,
soft delete, autenticación con JWT y conexión a base de datos MySQL.

## 🚀 Tecnologías utilizadas

- Node.js
- Express 5
- MySQL2
- JSON Web Token (JWT)
- bcryptjs (encriptación de contraseñas)
- dotenv
- ULID (generación de IDs únicos)
- Nodemon (desarrollo)

## ✨ Funcionalidades

- 🔐 Autenticación con JWT
- 🔒 Encriptación de contraseñas con bcryptjs
- ✅ CRUD completo de tareas
- 🗑️ Soft delete de tareas
- 🗄️ Migraciones propias de base de datos
- 🌐 CORS configurado para consumo desde frontends

## 📁 Estructura del proyecto

proyecto-backend-node/
├── src/
│   ├── index.js          # Punto de entrada
│   ├── db/
│   │   └── run_migrations.js  # Migraciones
│   └── ...
├── .env.example
└── package.json

## ⚙️ Instalación y configuración

1. Clona el repositorio
```bash
git clone https://github.com/ctq1279/proyecto-backend-node.git
cd proyecto-backend-node
```

2. Instala dependencias
```bash
npm install
```

3. Configura las variables de entorno
```bash
cp .env.example .env
```
Edita el `.env` con tus credenciales de MySQL y tu JWT secret.

4. Ejecuta las migraciones
```bash
npm run db:migrate
```

5. Inicia el servidor
```bash
# Desarrollo
npm run dev

# Producción
npm start
```

El servidor corre en `http://localhost:3000` (o el puerto configurado en `.env`)

## 🔗 Frontends que consumen esta API

- ⚛️ Frontend React: [enlace al repo react]
- 🖥️ Frontend Laravel: https://github.com/ctq1279/todo-list-official
