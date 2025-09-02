Proyecto de pruebas E2E con Cypress sobre el flujo de compra en **Demoblaze**:

---

```markdown
# 🧪 Test Automatizado E2E - Flujo de Compra en Demoblaze

Este proyecto utiliza **Cypress** para automatizar el flujo completo de compra de productos en la tienda web [Demoblaze](https://www.demoblaze.com/).

## 📋 Objetivo

Automatizar el siguiente flujo:

1. Ingresar a la página de Demoblaze.
2. Agregar dos productos al carrito.
3. Visualizar el carrito y confirmar que los productos estén agregados.
4. Completar el formulario de compra.
5. Verificar el mensaje de confirmación de compra.

---

## 🛠 Herramientas utilizadas

- [Cypress 12+](https://docs.cypress.io/)
- Node.js
- Visual Studio Code (opcional)
- Sistema operativo: Windows 10

---

## 🧩 Estructura del proyecto

```

📁 cypress/
└── e2e/
└── spec-copy-1.cy.js   # Archivo con los casos de prueba
README.md                    # Este archivo
package.json                 # Dependencias y configuración de Cypress

````

---

## 🚀 Instalación y ejecución

1. **Clona este repositorio:**
   ```bash
   git clone https://github.com/GisselaJarrin/QA---BP/demoblaze-cypress-test.git
   cd demoblaze-cypress-test
````

2. **Instala las dependencias:**

   ```bash
   npm install
   ```

3. **Ejecuta Cypress:**

   ```bash
   npx cypress open
   ```

   Luego selecciona el archivo `spec-copy-1.cy.js` desde la interfaz gráfica de Cypress.

---

## ✅ Casos de prueba

| Caso                               | Descripción                                              |
| ---------------------------------- | -------------------------------------------------------- |
| `Agrega dos productos al carrito`  | Navega y agrega 2 laptops al carrito                     |
| `Visualiza el carrito`             | Abre el carrito y verifica que haya al menos 2 productos |
| `Completa el formulario de compra` | Llena el formulario de orden con datos simulados         |
| `Finaliza la compra`               | Verifica que el mensaje de confirmación sea visible      |

---

## 🧪 Capturas de prueba (Opcional)

Puedes agregar aquí capturas de pantalla de los tests pasando o del resumen final de Cypress si se requiere evidencia visual.

---

## 📌 Notas importantes

* El botón `Cart` fue accedido por su ID (`#cartur`) ya que `cy.contains('Cart')` fallaba por mayúsculas o timing.
* El mensaje de confirmación **no** es un `alert`, sino un modal en `.modal-content`, por eso se cambió la forma de verificación.
* Se recomienda tener conexión a internet ya que el sitio Demoblaze es una demo pública y puede variar en disponibilidad.

---

## ✍️ Autor

**Gissela Jarrín** - *Tester QA Cypress*

---



¿Deseas también el archivo `conclusiones.txt` para acompañar la entrega?
```
