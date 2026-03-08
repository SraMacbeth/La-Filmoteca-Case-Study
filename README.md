# 🎬 La Filmoteca - React Case Study

Este repositorio documenta el desarrollo de **La Filmoteca**, una WebApp diseñada para la exploración y gestión de contenidos cinematográficos. El proyecto se centra en ofrecer una experiencia de usuario fluida, utilizando **React** para la lógica de componentes y **Bootstrap** para un diseño responsivo y profesional.

> **Nota de la desarrolladora:** Actualmente el código fuente en un repositorio privado durante un proceso de refactorización de la capa de servicios, con el objetivo de integrar exclusivamente APIs de contenido legal (YouTube SDK).
---

## 🛠️ Stack Tecnológico

* **Frontend:** React.js (Hooks, Props, State Management).
* **Estilos:** Bootstrap 5 & CSS Modules.
* **Consumo de Datos:** Fetch API / Axios para integración con TMDb.
* **Despliegue previo:** Netlify.

---

## 💡 Retos Técnicos y Soluciones

### 1. Arquitectura de Componentes Reutilizables

En lugar de crear estructuras repetitivas, diseñé componentes modulares como `MovieCard`, `SearchBar` y `CategoryFilter`. Esto permitió mantener un código limpio (DRY - Don't Repeat Yourself) y facilitar la escalabilidad del sitio.

### 2. Seguridad de las API Keys

Implementación de variables de entorno (.env) para la gestión segura de claves de API, siguiendo las mejores prácticas de seguridad en el frontend". Esto demuestra que tienes conciencia de ciberseguridad básica.

### 3. Gestión de Estados con Hooks

Utilicé `useState` y `useEffect` para manejar el ciclo de vida de los datos. La aplicación sincroniza la búsqueda del usuario con los resultados de la API de forma dinámica, asegurando que la interfaz se actualice instantáneamente sin recargar la página.

### 4. Diseño Responsivo (Mobile First)

Gracias a la implementación estratégica de las **Grid Systems de Bootstrap**, la aplicación ofrece una experiencia óptima tanto en monitores de escritorio como en dispositivos móviles, adaptando el número de columnas y el tamaño de los elementos automáticamente.

---

## 📸 Vista Previa del Proyecto

Aquí puedes ver cómo luce la interfaz y la organización de la información:

*()*

1. **Dashboard Principal:** Vista de películas en tendencia con cards interactivas.
2. **Buscador Dinámico:** Filtrado en tiempo real por título o categoría.
3. **Detalle de Película:** Modal informativo con sinopsis y metadata obtenida de la API.

---

## 🚀 Próximos Pasos Técnicos

* **Integración de YouTube SDK:** Implementación de un reproductor oficial para trailers.
* **Custom Hooks:** Extracción de la lógica de llamadas a la API en un hook personalizado `useMovies` para mejorar la legibilidad.
* **Optimización de Imágenes:** Implementación de *lazy loading* para mejorar el tiempo de carga inicial.