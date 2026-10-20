# 📼 RetroVideo - Videoclub Management System

**RetroVideo** es mi proyecto final intermodular de 1º de DAW (IES Severo Ochoa). Es una aplicación diseñada para gestionar un videoclub, permitiendo administrar el catálogo de películas y videojuegos, gestionar los socios y llevar el registro de los alquileres.

El objetivo de este proyecto es integrar todos los conocimientos adquiridos durante el curso en un único MVP (Producto Mínimo Viable), separando claramente la lógica de negocio, la persistencia de datos y la interfaz visual.

## 🛠️ Stack Tecnológico y Estructura

El repositorio está dividido en carpetas para separar las distintas responsabilidades del proyecto:

- **`/backend` (Java 21):** Contiene toda la lógica. Utiliza el patrón DAO para centralizar el acceso a datos y JPA (con Hibernate) para conectar con la base de datos mediante ORM.
- **`/database` (MySQL/MariaDB):** Aquí se encuentra el script `videoclub.sql` con la estructura de tablas y los datos de prueba.
- **`/frontend` (HTML5 & CSS3):** Prototipo visual de la interfaz web. Está maquetado de forma *responsive* utilizando CSS Grid y variables nativas. 
- **`/docs/api` (OpenAPI 3.0):** Documentación técnica (`openapi.yaml`) que define los *endpoints* y la estructura de una futura API REST, dejando preparada la base para conectar el frontend y el backend de forma asíncrona.

## 🚀 Cómo ejecutarlo en local

### 1. Base de Datos
1. Levanta tu servidor MySQL (por ejemplo, con XAMPP).
2. Importa el archivo `database/videoclub.sql` en tu gestor (phpMyAdmin, DBeaver, etc.) para crear la base de datos y cargar la información inicial.

### 2. Backend
1. Abre la carpeta `backend/` como un proyecto en tu IDE (IntelliJ IDEA o Eclipse).
2. Deja que Maven resuelva y descargue las dependencias del archivo `pom.xml`.
3. Ejecuta la clase `app.Main`. La aplicación se conectará a MySQL y lanzará la interfaz de consola.

### 3. Frontend
Simplemente abre el archivo `frontend/index.html` en tu navegador para ver la propuesta de maquetación de la versión web.

## 🔄 Metodología y Git
Aunque es un proyecto académico, el desarrollo se ha planteado simulando un entorno de trabajo colaborativo real:
- Estructura de repositorios modular.
- Control de versiones siguiendo un flujo basado en ramas para nuevas funcionalidades (`feature/...`) e integración mediante *Pull Requests* para proteger la rama `main`.

---
**Autor:** Adrián Martínez - 1º DAW (Curso 2025/2026) - IES Severo Ochoa.
