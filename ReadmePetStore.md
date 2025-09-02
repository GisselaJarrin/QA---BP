¡Perfecto! Aquí tienes los **3 archivos solicitados** para la **opción 1 del proyecto de pruebas E2E con Cypress**. Solo copia el contenido de cada uno en su respectivo archivo dentro de tu carpeta del proyecto (`petstore`).

---

## ✅ `README.md`

```markdown
# Proyecto E2E Testing con Cypress - Demoblaze

Este proyecto realiza pruebas E2E (End to End) sobre la API de [Demoblaze](https://api.demoblaze.com) utilizando el framework **Cypress**.

## 📁 Estructura del proyecto

```

petstore/
├── cypress/
│   └── e2e/
│       └── spec-copy-1.cy.js
├── node\_modules/
├── README.md
├── package.json
├── cypress.config.js
├── instrucciones.txt
└── conclusiones.txt

````

## 🔧 Instalación

1. Clona o descarga el proyecto.
2. Abre una terminal y ve al directorio del proyecto:

```bash
cd petstore
````

3. Instala las dependencias:

```bash
npm install
```

## 🚀 Ejecutar Cypress

Para abrir la interfaz de Cypress:

```bash
npx cypress open
```

1. Selecciona **E2E Testing**.
2. Elige un navegador (Chrome, Edge, Firefox, etc).
3. Ejecuta el archivo `spec-copy-1.cy.js`.

## 🧪 Descripción de las pruebas

### ✅ Crear usuario

Hace una petición POST a `/signup` para crear un nuevo usuario con un nombre único.

### ✅ Login correcto

Hace una petición POST a `/login` con el usuario recién creado.

## 📌 Requisitos

* Node.js >= 18
* Cypress >= 12

## 👨‍💻 Autor

Proyecto realizado por \[Tu Nombre Aquí]

````


