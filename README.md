# 📘 API JSON Server - Agenda ADSO

## 🧾 Descripción del proyecto

Esta es una API REST simulada creada con **JSON Server**, diseñada para gestionar una agenda básica. Permite almacenar y consultar información como usuarios, tareas u otros datos de forma rápida y sencilla sin necesidad de una base de datos real.

Este proyecto es ideal para prácticas de desarrollo frontend y backend, pruebas de consumo de APIs o como base para proyectos más grandes.

---

## 🚀 Tecnologías utilizadas

* Node.js
* JSON Server
* JavaScript
* Git y GitHub

---

## 📁 Estructura del proyecto

```
Local/
│
├── db.json        # Base de datos en formato JSON
├── server.js      # Configuración del servidor (opcional)
├── package.json   # Configuración del proyecto y dependencias
└── README.md      # Documentación del proyecto
```

---

## ⚙️ Instalación y ejecución

### 1. Clonar el repositorio

```bash
git clone https://github.com/esneiderj159-ai/Local-agenda-adso-Api.git
```

### 2. Entrar a la carpeta del proyecto

```bash
cd Local-agenda-adso-Api
```

### 3. Instalar dependencias

```bash
npm install
```

### 4. Ejecutar el servidor

```bash
npx json-server --watch db.json
```

---

## 🌐 Uso de la API

Una vez ejecutado el servidor, la API estará disponible en:

```
http://localhost:3000
```

---

## 📌 Endpoints disponibles (ejemplo)

Si tu `db.json` tiene esta estructura:

```json
{
  "usuarios": [
    { "id": 1, "nombre": "Juan" }
  ],
  "tareas": [
    { "id": 1, "titulo": "Estudiar", "completado": false }
  ]
}
```

### 🔹 Usuarios

* GET `/usuarios` → Obtener todos los usuarios
* GET `/usuarios/1` → Obtener un usuario por ID
* POST `/usuarios` → Crear usuario
* PUT `/usuarios/1` → Actualizar usuario
* DELETE `/usuarios/1` → Eliminar usuario

### 🔹 Tareas

* GET `/tareas`
* POST `/tareas`
* PUT `/tareas/1`
* DELETE `/tareas/1`

---

## 🧪 Ejemplo de petición POST

```json
POST /usuarios
Content-Type: application/json

{
  "nombre": "Carlos"
}
```

---

## 💡 Notas importantes

* JSON Server simula una API REST completa automáticamente.
* Los datos se guardan directamente en el archivo `db.json`.
* No requiere base de datos externa.

---

## 👨‍💻 Autor

Proyecto desarrollado por **Sneider Jiménez** como práctica de desarrollo de APIs.

---

## 📈 Posibles mejoras

* Agregar autenticación
* Conectar con una base de datos real
* Desplegar la API en la nube
* Crear un frontend que consuma esta API

---

## 📬 Contacto

Si deseas mejorar este proyecto o tienes dudas, puedes contribuir o contactarme a través de GitHub.

---

⭐ Si este proyecto te fue útil, ¡no olvides darle una estrella!
