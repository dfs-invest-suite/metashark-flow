# Metashark.Tech - PWA de MetaShark Tech

Bienvenido al repositorio de la Progressive Web App (PWA) Test de **MetaShark Tech**.

## Visión General del Proyecto

`metashark.tech` es la aplicación central de nuestra presencia web, construida con Next.js dentro de un monorepo Nx para optimizar el desarrollo, las pruebas y el build.

## Primeros Pasos

### Prerrequisitos

Asegúrate de tener instalado [Node.js](https://nodejs.org/) (versión 20.x recomendada) y [pnpm](https://pnpm.io/) (versión 10.x o la especificada en `package.json`).

### Instalación de Dependencias

Desde la raíz del proyecto, ejecuta:

```bash
pnpm install

```

Tareas Comunes de Desarrollo
Este workspace utiliza Nx para gestionar las tareas del proyecto.
Iniciar el Servidor de Desarrollo
Para ejecutar la aplicación metashark.tech en modo de desarrollo con hot-reloading:
pnpm nx dev metashark.tech

O simplemente (si nx está accesible globalmente o a través de npx):
```bash
nx dev metashark.tech

```
La aplicación estará disponible generalmente en http://localhost:3000 (o el puerto que Next.js/Nx asigne).
Crear un Bundle de Producción
Para generar una compilación optimizada para producción de metashark.tech:
pnpm nx build metashark.tech

O:
```bash
nx build metashark.tech

```
La salida del build se encontrará en dist/apps/metashark.tech o, para el caso específico de Next.js, los artefactos principales estarán en apps/metashark.tech/.next.

Ejecutar Pruebas Unitarias
```bash
pnpm nx test metashark.tech

```
Ejecutar Pruebas End-to-End (E2E)
```bash
pnpm nx e2e metashark.tech-e2e

```
Ver Todos los Targets Disponibles
Para ver todas las tareas (targets) que puedes ejecutar para la aplicación metashark.tech:
```bash
pnpm nx show project metashark.tech

```
Estructura del Proyecto
apps/metashark.tech/: Código fuente principal de la PWA.
apps/metashark.tech-e2e/: Pruebas End-to-End para la PWA.
libs/: (Si existen) Librerías compartidas dentro del workspace.
tools/: (Si existen) Herramientas y scripts de desarrollo.
Visualizar el Grafo de Dependencias del Proyecto
Para entender mejor cómo están interconectados los proyectos y librerías dentro de este workspace Nx:
```bash
pnpm nx graph
```
Despliegue
Esta aplicación está configurada para ser desplegada en Vercel. Los despliegues a producción se activan automáticamente con los pushes a la rama main.
Herramientas y Extensiones Útiles
Nx Console: Una extensión para VS Code e IntelliJ que facilita la ejecución de tareas y la generación de código con Nx.
Instalar Nx Console


Desarrollado por el equipo de MetaShark Tech.
