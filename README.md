# 🏆 Quiniela Frontend – Astro
Frontend de la plataforma Quiniela, una aplicación web para crear y participar en quinielas deportivas, consumiendo datos desde una API externa y conectándose a un backend desarrollado con FastAPI.

Este proyecto se encarga de toda la interfaz de usuario, navegación, visualización de partidos y captura de predicciones.


## 🚀 Tecnologías utilizadas

- Astro – Framework frontend moderno y rápido
- JavaScript / TypeScript (según configuración)
- CSS / Styles globales
- Componentes reutilizables
- Integración futura con React (para partes interactivas)
- Comunicación con API REST (FastAPI)

## 🎯 Objetivo del Frontend
El fontend tiene como propósito:

- Mostrar quinielas disponibles
- Permitir crear nuevas quinielas
- Visualziar partidos por liga, temporada y jornada
- Permitir a los usuarios registrar sus predicciones
- Mopstrar resultados y puntajes
- Consumir datos desde el backend (FastAPI)

## 🧭 Flujo general de la aplicación

1. El usuario accede a la plataforma
2. Visualiza quinielas públicas o propias
3. Crea una nueva quiniela seleccionando:
    - Deporte
    - País 
    - Liga 
    - Temporada / Jornada
4. Visualiza los partidos de esa jornada
5. Ingresa sus predicciones
6. Consulta resultados y tabla de posiciones

## 🚀 Estructura de proyecto

Dentro de tu proyecto Astro, verás las siguientes carpetas y archivos:

```text
/
├── public/
│   └── favicon.svg              # Archivos públicos
├── src
│   ├── assets/                  # Imágenes, íconos, fuentes
│   ├── components/              # Componentes reutilizables
│   ├── layouts/                 # Layouts base del sitio
│   ├── pages/                   # Rutas de la aplicación
│   └── styles/                  # Estilos globales
├── astro.config.mjs             # Configuración de Astro
└── package.json                 # Dependencias y scripts
```

## 🧩 Carpetas clave
🔹 pages/
Define las rutas del sitio:
- / → Página principal
- /quinielas
- /quiniela/[id]
- /login, /register (futuro)
🔹 components/
Componentes reutilizables como:
- Cards de partidos
- Formularios
- Tablas de posiciones
- Botones
- Modales
🔹 layouts/
Layouts base para mantener una estructura consistente:
- Header
- Footer
- Contenido principal

## 🔌 Comunicación con el Backend
El frontend se comunica con el backend mediante API REST, por ejemplo:
- GET /quinielas
- POST /quinielas
- GET /quinielas/{id}/matches
- POST /predictions

El backend se encarga de:
- Autenticación
- Consumo de API deportiva
- Lógica de negocio
- Base de datos

## 🧞 Comandos

Todos los comandos se ejecutan desde la raíz del proyecto, desde una terminal:
| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Instalaciones dependencias                            |
| `npm run dev`             | Inicia el servidor de desarrollo local en `localhost:4321`      |
| `npm run build`           | Construya su sitio de producción para `./dist/`          |
| `npm run preview`         | Obtenga una vista previa de su compilación localmente, antes de implementarla     |
| `npm run astro ...`       | Ejecute comandos CLI como `astro add`, `astro check` |
| `npm run astro -- --help` | Obtenga ayuda para utilizar la CLI de Astro                     |

## 🛠️ Instalación y ejecución
````
npm install
npm run dev
````

Luego abre:
````
http://localhost:4321
````

## 📌 Estado del proyecto
🚧 En desarrollo
📈 Arquitectura preparada para escalar
🔌 Integración con backend FastAPI

## ✍️ Autor
Proyecto personal desarrollado por **Wilver Ixcot**
Enfocado en mejorar habilidades de arquitectura, backend y frontend moderno.
