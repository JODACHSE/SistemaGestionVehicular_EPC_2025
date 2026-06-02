<p align="center">
  <a href="https://laravel.com" target="_blank">
    <img src="public/assets/HolaEpc.png" width="400" alt="Logo HolaEpc">
  </a>
</p>

<p align="center">
  <a href="https://laravel.com" target="_blank"><img src="https://img.shields.io/badge/framework-laravel-red" alt="Laravel Framework"></a>
  <a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
  <a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

# Sistema de Gestión Vehicular 🚗📋

Un sistema automatizado de control y gestión de vehículos en tiempo real desarrollado para optimizar los procesos de Recursos Humanos (RRHH). Esta plataforma reemplaza por completo el flujo de trabajo obsoleto basado en formularios de Google Forms y el volcado manual de información a hojas de cálculo de Excel, eliminando la carga administrativa extra y permitiendo una distribución eficiente del tiempo del personal.

## 🚀 Propósito del Proyecto

En muchas organizaciones, el control de los vehículos corporativos se realiza mediante registros manuales o formularios aislados, lo que genera retrasos, pérdida de información y un esfuerzo duplicado al centralizar los datos en Excel. 

Este **Sistema de Gestión Vehicular** centraliza la operación en tiempo real, garantizando que RRHH cuente con datos precisos sobre la disponibilidad de la flota, el estado de los vehículos antes de su uso y la asignación del recurso humano sin procesos burocráticos ni cargas de trabajo adicionales.

## ✨ Características Principales

* **Gestión en Tiempo Real:** Visualización y actualización instantánea de los datos sin necesidad de sincronizaciones manuales.
* **Inventario de Vehículos:** Control centralizado de toda la flota automotriz de la organización (marca, modelo, placas, estado actual).
* **Inspección Pre-Uso (Checklist):** Actualización obligatoria del estado del vehículo antes de cada uso, asegurando la trazabilidad de fallas, kilometraje y condiciones de entrega.
* **Gestión de Recurso Humano:** Control y asignación de conductores, historial de usos y responsabilidades asociadas a cada vehículo.
* **Dashboard Automatizado:** Panel de control intuitivo para RRHH que elimina la dependencia de archivos Excel externos.

## 🛠️ Tecnologías Utilizadas

El proyecto se construyó utilizando un stack moderno, robusto y de rápido despliegue:

* **Backend:** [Laravel](https://laravel.com/) (Framework PHP) - Arquitectura MVC, migraciones de base de datos y validación robusta.
* **Lenguaje principal:** PHP
* **Frontend:** [Bootstrap](https://getbootstrap.com/) & **SCSS** - Diseño adaptivo (Mobile-First) y estilos modulares estructurados.
* **Interactividad:** JavaScript (JS) para actualizaciones dinámicas en la interfaz.
* **Arquitectura de UI:** Componentes y componentes parciales reutilizables de Blade para mantener un código limpio y mantenible (DRY - *Don't Repeat Yourself*).

## 📋 Requisitos del Sistema

Antes de instalar el proyecto, asegúrate de cumplir con los siguientes requisitos:

* PHP >= 8.1
* Composer
* MySQL o PostgreSQL
* Node.js & NPM

## 🔧 Instalación y Configuración

Sigue estos pasos para levantar el proyecto en tu entorno local:

1. **Clonar el repositorio:**
	```
	git clone https://github.com/JODACHSE/SistemaGestionVehicular_EPC_2025.git
    cd SistemaGestionVehicular_EPC_2025
	```
	
2.  **Instalar dependencias de PHP:**
    ```
    composer install
    ```
    
3.  **Instalar dependencias de Frontend:**    
    ```
    npm install && npm run dev
    ```
    
5.  **Configurar el archivo de entorno:** Copia el archivo de ejemplo y configura tus credenciales de base de datos:
    ```
    cp .env.example .env
    ```
    
    Abre el archivo `.env` y edita las siguientes líneas con la configuración de tu servidor local:
    
    Fragmento de código
    
    ```
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=sistema_vehicular
    DB_USERNAME=tu_usuario
    DB_PASSWORD=tu_contrasena
    ```
    
6.  **Generar la clave de la aplicación:**
    ```
    php artisan key:generate
    ```
    
7.  **Ejecutar las migraciones (y seeders si aplican):**
    ```
    php artisan migrate
    ```
    
8.  **Iniciar el servidor de desarrollo:**
    ```
    php artisan serve
    ```
    Visita `http://127.0.0.1:8000` en tu navegador.
    

## 📐 Estructura de Componentes UI

El frontend está altamente modularizado a través del motor de plantillas Blade de Laravel:

-   `resources/views/components/`: Componentes globales reutilizables (botones personalizados, alertas, tarjetas de estado).
    
-   `resources/views/partials/`: Secciones parciales de la página (Navbar, Sidebar, Footer) para evitar la duplicación de código en el diseño base.
    

## 👥 Contribuciones

Si deseas mejorar este sistema, siéntete libre de abrir un _Pull Request_ o reportar un _Issue_.

1.  Haz un Fork del proyecto.
    
2.  Crea una rama con tu nueva característica (`git checkout -b feature/NuevaCaracteristica`).
    
3.  Haz un commit de tus cambios (`git commit -am 'Añade una nueva característica'`).
    
4.  Empuja la rama (`git push origin feature/NuevaCaracteristica`).
    
5.  Abre un Pull Request.

 ---
Desarrollado como solución tecnológica eficiente para la optimización de procesos logísticos y de RRHH.
