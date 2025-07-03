# Tarea_2_07_02_2025

ase 1 - Proyecto CRUD de Usuarios con MongoDB

Este proyecto es parte de la Fase 1 de la materia Ingeniería de Software. Se trata de una API REST construida con Node.js, Express y MongoDB, que permite crear, leer, actualizar, eliminar y autenticar usuarios. Incluye manejo seguro de contraseñas y generación de tokens con JWT.

Autor
Nombre: José Gerardo Avelar de León
Matrícula: AL03109294
Instructor: Guillermo Monroy Rodríguez

Objetivo del Proyecto
Desarrollar una API backend funcional para la gestión de usuarios, aplicando los principios de la ingeniería de software y metodologías ágiles. El objetivo es cubrir funciones básicas de autenticación y CRUD, fundamentales en cualquier sistema moderno.

Tecnologías utilizadas

Node.js

Express

MongoDB Atlas

Mongoose

JWT (jsonwebtoken)

bcrypt

dotenv

Instalación y ejecución

Clonar el repositorio:
git clone https://github.com/Geragdl/Fase1_07_02_2025.git
cd Fase1_07_02_2025

Instalar dependencias:
npm install

Crear el archivo .env a partir de .env.example:
cp .env.example .env

Llenar el archivo .env con los siguientes datos:
PORT=5000
MONGO_URI=mongodb+srv://<usuario>:<contraseña>@<cluster>.mongodb.net/fase1
JWT_SECRET=clave-super-secreta

Iniciar el servidor:
npm start

Endpoints disponibles

Método: POST
Ruta: /users
Descripción: Crear nuevo usuario

Método: GET
Ruta: /users
Descripción: Obtener todos los usuarios

Método: GET
Ruta: /users/:id
Descripción: Obtener usuario por ID

Método: PUT
Ruta: /users/:id
Descripción: Actualizar usuario por ID

Método: DELETE
Ruta: /users/:id
Descripción: Eliminar usuario por ID

Método: POST
Ruta: /login
Descripción: Iniciar sesión y obtener token JWT

Seguridad

Las contraseñas se cifran con bcrypt.

Los tokens JWT generados son válidos por 1 hora.

Las contraseñas no se exponen en las respuestas de la API.

Pruebas realizadas
Se utilizaron comandos curl para probar todas las rutas:

Crear usuarios

Consultar todos los usuarios

Obtener usuario por ID

Actualizar usuario por ID

Eliminar usuario por ID

Iniciar sesión con JWT

Manejo de errores como correo duplicado, ID inválido, y credenciales incorrectas

Recursos utilizados

GitHub

Codespaces

MongoDB Atlas

Terminal y curl

Licencia
Proyecto creado con fines educativos para la materia Ingeniería de Software. Puede ser reutilizado y adaptado libremente.

Contacto
Correo: AL03109294@tecmilenio.mx

