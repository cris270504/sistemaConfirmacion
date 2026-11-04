> ⚠️ **Versión anterior, ya no se mantiene.** La versión actual está en [Sistema-de-gesti-n-de-Programa-de-Confirmaci-n-Fronted-](https://github.com/cris270504/Sistema-de-gesti-n-de-Programa-de-Confirmaci-n-Fronted-).

# ⛪ Sistema de Gestión de Asistencias - Frontend

Este repositorio contiene la capa de presentación (Frontend) del **Sistema Institucional de Gestión de Asistencias y Control Documental**, desarrollado como parte del proyecto de prácticas preprofesionales en **T3M E.I.R.L.** La aplicación ha sido construida como una **SPA (Single Page Application)** utilizando tecnologías reactivas modernas para garantizar una experiencia de usuario fluida y eficiente.

## 🚀 Tecnologías Utilizadas

*   **Framework:** [Vue.js 3](https://vuejs.org/) (Composition API).
*   **Bundler:** [Vite](https://vitejs.dev/) (Para un entorno de desarrollo ultrarrápido).
*   **Estilos:** [Tailwind CSS](https://tailwindcss.com/) (Diseño responsivo y utilitario).
*   **Cliente HTTP:** [Axios](https://axios-http.com/) (Consumo de servicios API REST).
*   **Iconografía:** [Lucide Vue](https://lucide.dev/) / Heroicons.

## 📦 Requisitos Previos

Antes de iniciar la instalación, asegúrate de tener instalado:
*   [Node.js](https://nodejs.org/) (Versión 18.x o superior recomendada).
*   [NPM](https://www.npmjs.com/) o [Yarn].
*   El backend (`sistemaConfirmacionApi`) debe estar configurado y corriendo para el consumo de datos.

## 🛠️ Instalación y Configuración

Siga estos pasos para levantar el entorno de desarrollo local:

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/cris270504/sistemaConfirmacion.git](https://github.com/cris270504/sistemaConfirmacion.git)
    cd sistemaConfirmacion
    ```

2.  **Instalar dependencias:**
    ```bash
    npm install
    ```

3.  **Configurar variables de entorno:**
    Crea un archivo `.env` en la raíz del proyecto y define la URL de acceso a la API:
    ```env
    VITE_API_BASE_URL=http://localhost:8000/api
    ```

4.  **Iniciar el servidor de desarrollo:**
    ```bash
    npm run dev
    ```
    La aplicación estará disponible por defecto en `http://localhost:5173`.

## 📂 Estructura del Proyecto

```text
src/
├── assets/         # Recursos estáticos (Imágenes, estilos globales)
├── components/     # Componentes de UI reutilizables (Botones, Modales, Tablas)
├── layouts/        # Estructuras de página (Navegación, Sidebar)
├── services/       # Clientes de Axios y lógica de comunicación con la API
├── views/          # Páginas principales (Login, Dashboard, Asistencias)
├── App.vue         # Componente raíz
└── main.js         # Configuración e inicialización de la instancia de Vue
