# QA---BP
Frameware Selenium WebDriver
# **README: Instrucciones para Ejecutar el Script de Automatización**

Este archivo contiene las instrucciones para ejecutar el script de prueba de automatización del flujo de compra en **Demoblaze** usando **Python** y **Selenium WebDriver**.

---

## **Requisitos Previos**

Antes de ejecutar el script, asegúrate de tener lo siguiente instalado en tu máquina:

1. **Python 3.x**
   Si aún no tienes Python, puedes descargarlo desde:
   [https://www.python.org/downloads/](https://www.python.org/downloads/)

2. **Selenium WebDriver**
   Selenium es necesario para interactuar con el navegador de forma automatizada. Puedes instalar Selenium usando el siguiente comando en tu terminal:

   ```bash
   pip install selenium
   ```

3. **WebDriver para tu Navegador (ChromeDriver)**
   Selenium necesita un controlador para interactuar con el navegador. En este ejemplo, utilizamos **Google Chrome**, por lo que necesitas **ChromeDriver**.
   Para instalar automáticamente ChromeDriver, utilizamos la biblioteca `webdriver_manager`:

   ```bash
   pip install webdriver-manager
   ```
## **Pasos para Ejecutar el Script**

### 1. **Clonar o Descargar el Proyecto**
* Si tienes Git instalado, puedes clonar el repositorio utilizando el siguiente comando:

  ```bash
  git clone <URL del repositorio en GitHub>
  ```

* Si no tienes Git, puedes descargar los archivos del repositorio en formato **ZIP** y descomprimirlos.

### 2. **Preparación del Entorno**
* Asegúrate de tener Python y las dependencias necesarias instaladas. Para instalar las dependencias requeridas, abre una terminal o línea de comandos y navega hasta el directorio del proyecto.

* Ejecuta el siguiente comando para instalar **Selenium** y **WebDriver Manager**:

  ```bash
  pip install selenium webdriver-manager
  ```

### 3. **Revisar el Código**
* Abre el archivo `compra.py` con el editor de código de Visual Studio Code).

* **Código principal**: El script está diseñado para automatizar un flujo de compra en la página web **Demoblaze**. El flujo incluye agregar productos al carrito, rellenar el formulario de compra, y finalizar la compra.

### 4. **Ejecutar el Script**
* Para ejecutar el script de prueba se abre una terminal o línea de comandos en la carpeta con el archivo `compra.py` y se escribe:

  ```bash
  python compra.py
  ```

### 5. **Verificación del Resultado**
* El script abrirá automáticamente **Google Chrome** (asegúrate de tenerlo instalado).
* Navegará por la página **Demoblaze**, agregará dos productos al carrito, completará el formulario de compra, y finalizará el proceso.
* Finalmente, el script buscará el mensaje de confirmación **"Thank you for your purchase!"** y lo imprimirá en la terminal.
* El navegador se cerrará automáticamente después de unos segundos.

### 6. **Archivos Generados**
* **test\_compra.py**: El archivo de prueba automatizada.
* **readme.txt**: Este archivo con las instrucciones de uso.
* **conclusiones.txt**: (Opcional) Archivo donde puedes colocar los hallazgos y comentarios sobre la ejecución de la prueba.

---

## **Consideraciones Finales**
* Si experimentas algún error con la versión de **ChromeDriver**, asegúrate de que **ChromeDriver** sea compatible con la versión de **Google Chrome** que tienes instalada.
* Si el script no encuentra los elementos correctamente, puedes tener que actualizar los selectores (por ejemplo, `XPath` o `ID`) según los cambios en la página web.

---

¡Eso es todo! Si tienes algún problema o pregunta sobre la ejecución del script, no dudes en consultar los logs de errores o contactarme para más ayuda.

---




