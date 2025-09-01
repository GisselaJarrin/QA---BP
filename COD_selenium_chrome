!pip install selenium
!pip install webdriver_manager
!apt-get update # Actualiza la lista de paquetes
!apt install -y chromium-chromedriver # Instala Chrome y ChromeDriver
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
from selenium.webdriver.common.alert import Alert
from selenium.webdriver.chrome.service import Service
from webdriver_manager.chrome import ChromeDriverManager
from selenium.webdriver.chrome.options import Options
import time

# Configuración de las opciones de Chrome
chrome_options = Options()
chrome_options.add_argument("--headless")  # Ejecutar sin abrir una ventana de navegador
chrome_options.add_argument("--no-sandbox")
chrome_options.add_argument("--disable-dev-shm-usage")

# Configuración del WebDriver
driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=chrome_options)

# Paso 1: Navegar a la página de Demoblaze
driver.get("https://www.demoblaze.com/")

# Paso 2: Agregar productos al carrito (Ejemplo: MacBook air)
driver.find_element(By.XPATH, "//a[text()='MacBook air']").click()
driver.find_element(By.XPATH, "//a[text()='Add to cart']").click()

# Aceptar la alerta (que aparece al agregar el producto)
alert = Alert(driver)
alert.accept()

# Agregar otro producto (Ejemplo: Sony vaio)
driver.find_element(By.XPATH, "//a[text()='Sony vaio i7']").click()
driver.find_element(By.XPATH, "//a[text()='Add to cart']").click()

# Aceptar la alerta nuevamente
alert = Alert(driver)
alert.accept()

# Paso 3: Ir al carrito de compras
driver.find_element(By.ID, "cartur").click()

# Paso 4: Completar la compra
# Hacer clic en "Place Order"
driver.find_element(By.XPATH, "//button[text()='Place Order']").click()

# Rellenar la información del formulario
driver.find_element(By.ID, "name").send_keys("Gisela Jarrín")
driver.find_element(By.ID, "country").send_keys("Ecuador")
driver.find_element(By.ID, "city").send_keys("Quito")
driver.find_element(By.ID, "card").send_keys("135798654136")
driver.find_element(By.ID, "month").send_keys("12")
driver.find_element(By.ID, "year").send_keys("2025")

# Hacer clic en "Purchase"
driver.find_element(By.XPATH, "//button[text()='Purchase']").click()

# Paso 5: Verificar la confirmación de la compra
time.sleep(2)  # Esperar a que se muestre la confirmación

# Asegurarse de que el mensaje "Thank you for your purchase!" esté presente
confirmation_message = driver.find_element(By.XPATH, "//h2[text()='Thank you for your purchase!']").text
print(confirmation_message)

# Paso 6: Cerrar el navegador
time.sleep(3)  # Dejar la confirmación por unos segundos
driver.quit()
