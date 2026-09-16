# Eco Paper Kraft - Backend (Laravel / API)

¡Bienvenido al repositorio del Backend de **Eco Paper Kraft**!  
Este proyecto es el motor central de nuestra aplicación. Se encarga de procesar la lógica de negocio, gestionar la base de datos y proveer la API que consume la interfaz en React.

---

## Paso 1: Instalación de Herramientas (Solo se hace una vez)

Antes de empezar, asegúrate de tener instaladas las siguientes herramientas en tu computadora:

1. **Visual Studio Code (Editor de Código):**
   * Descárgalo e instálalo desde: [code.visualstudio.com](https://code.visualstudio.com/)
2. **Git (Control de Versiones):**
   * Descárgalo e instálalo desde: [git-scm.com](https://git-scm.com/)
3. **PHP (Versión 8.2 o superior):**
   * En Windows puedes usar [Laragon](https://laragon.org/) o [XAMPP](https://www.apachefriends.org/) para instalar PHP de forma sencilla.
4. **Composer (Gestor de paquetes de PHP):**
   * Descárgalo e instálalo desde: [getcomposer.org](https://getcomposer.org/)

---

## Paso 2: Clonar y Configurar el Proyecto

Abre la terminal de tu computadora (o la de Visual Studio Code) y ejecuta los siguientes comandos en orden:

### 1. Clonar el repositorio

`git clone https://github.com/TU-USUARIO/eco-paper-kraft-backend.git`

`cd eco-paper-kraft-backend`

### 2. Instalar las dependencias de PHP

`composer install`

### 3. Configurar las variables de entorno

Copia el archivo de ejemplo para crear tu propio archivo local de configuración:

`cp .env.example .env`

*(Abre el archivo `.env` resultante y asegúrate de pedir las llaves de acceso de desarrollo si necesitas conectarte a Supabase o servicios externos).*

### 4. Generar la clave de la aplicación

`php artisan key:generate`

### 5. Encender el servidor local de desarrollo

`php artisan serve`

*(Abre el enlace que te genere la terminal, normalmente `http://127.0.0.1:8000`, para comprobar que la API está respondiendo).*

---

## Reglas (Git & GitHub)
Para proteger la integridad del código en producción, **está prohibido hacer push directo a la rama main**.

### Flujo diario:

1. **Crear una rama propia para tu tarea:**

   `git checkout -b feature/nombre-de-tu-tarea`

   *Ejemplo:* `git checkout -b feature/EPK-2-api-productos`

2. **Guardar tus cambios:**

   `git add .`

   `git commit -m "Agrega endpoint para listar productos"`

3. **Subir tu rama a GitHub:**

   `git push origin feature/nombre-de-tu-tarea`

4. **Solicitar revisión:**
   * Entra al repositorio en GitHub y presiona el botón **"Compare & pull request"** para enviar tu código a revisión.
