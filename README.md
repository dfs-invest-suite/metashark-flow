# Metashark.Tech - PWA de MetasharkTech

Bienvenido al repositorio de la Progressive Web App (PWA) Test de **MetaShark Inova**.

## Visión General del Proyecto

`metashark.tech` es la aplicación central de nuestra presencia web, construida con Next.js dentro de un monorepo Nx para optimizar el desarrollo, las pruebas y el build.

## Primeros Pasos

### Prerrequisitos

Asegúrate de tener instalado [Node.js](https://nodejs.org/) (versión 20.x recomendada) y [pnpm](https://pnpm.io/) (versión 10.x o la especificada en `package.json`).

### Instalación de Dependencias

Desde la raíz del proyecto, ejecuta:

```bash
pnpm install

Tareas Comunes de Desarrollo
Este workspace utiliza Nx para gestionar las tareas del proyecto.
Iniciar el Servidor de Desarrollo
Para ejecutar la aplicación metashark.tech en modo de desarrollo con hot-reloading:
pnpm nx dev metashark.tech

O simplemente (si nx está accesible globalmente o a través de npx):
nx dev metashark.tech

La aplicación estará disponible generalmente en http://localhost:3000 (o el puerto que Next.js/Nx asigne).
Crear un Bundle de Producción
Para generar una compilación optimizada para producción de metashark.tech:
pnpm nx build metashark.tech

O:

nx build metashark.tech

La salida del build se encontrará en dist/apps/metashark.tech o, para el caso específico de Next.js, los artefactos principales estarán en apps/metashark.tech/.next.

Ejecutar Pruebas Unitarias
pnpm nx test metashark.tech

Ejecutar Pruebas End-to-End (E2E)
pnpm nx e2e metashark.tech-e2e

Ver Todos los Targets Disponibles
Para ver todas las tareas (targets) que puedes ejecutar para la aplicación metashark.tech:
pnpm nx show project metashark.tech

Estructura del Proyecto
apps/metashark.tech/: Código fuente principal de la PWA.
apps/metashark.tech-e2e/: Pruebas End-to-End para la PWA.
libs/: (Si existen) Librerías compartidas dentro del workspace.
tools/: (Si existen) Herramientas y scripts de desarrollo.
Visualizar el Grafo de Dependencias del Proyecto
Para entender mejor cómo están interconectados los proyectos y librerías dentro de este workspace Nx:
pnpm nx graph

Despliegue
Esta aplicación está configurada para ser desplegada en Vercel. Los despliegues a producción se activan automáticamente con los pushes a la rama main.
Herramientas y Extensiones Útiles
Nx Console: Una extensión para VS Code e IntelliJ que facilita la ejecución de tareas y la generación de código con Nx.
Instalar Nx Console
Contribuir
[Detalles sobre cómo contribuir al proyecto, guías de estilo, etc. - AÑADIR SI ES NECESARIO]
Enlaces Útiles de Nx
Documentación de Nx
Nx y Next.js
Comunidad de Nx en Discord
Desarrollado por el equipo de MetasharkTech.
**Cambios y Porqués:**

1.  **Título:** Cambiado a `# Metashark.Tech - PWA de MetasharkTech` para ser específico.
2.  **Logo:** Añadí un placeholder para el logo de tu empresa. Reemplaza `URL_DE_TU_LOGO_AQUI` con la URL real, o elimina la línea si no quieres un logo o prefieres mantener solo el de Nx.
3.  **Introducción:** Personalizada para indicar que es la PWA de MetasharkTech.
4.  **Sección "Visión General del Proyecto":** Añadida para dar un breve contexto.
5.  **Sección "Primeros Pasos":** Añadida con prerrequisitos e instalación de dependencias usando `pnpm`.
6.  **Comandos de Tareas:** Mantuve los comandos clave de Nx (`dev`, `build`, `test`, `e2e`, `show project`, `graph`), pero les puse el prefijo `pnpm` ya que es tu gestor de paquetes. También mencioné que `nx comando` a secas puede funcionar.
7.  **Salida del Build:** Clarifiqué dónde encontrar la salida del build para Next.js.
8.  **Estructura del Proyecto:** Mencioné las carpetas clave.
9.  **Sección "Despliegue":** Añadí una breve nota sobre Vercel.
10. **Sección "Contribuir":** Añadí un placeholder por si quieres añadir directrices de contribución.
11. **Pie de Página:** Añadido "Desarrollado por el equipo de MetasharkTech."
12. **Eliminación de Enlaces de CI de Nx Cloud (Opcional):** Quité el enlace de "Finish your CI setup" que apunta a Nx Cloud, ya que puede no ser relevante si no lo estás usando activamente o si ya está configurado. Si lo usas, puedes volver a añadirlo.
13. **Simplificación de "Add new projects":** Aunque es útil, si este repo es *solo* para la PWA `metashark.tech` y no planeas añadir muchas otras apps/libs dentro del mismo repo *inmediatamente*, esta sección podría ser menos prioritaria en el README principal. La he mantenido por ahora porque es una capacidad de Nx.
```
