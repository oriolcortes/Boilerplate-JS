# Boilerplate de JS Vanilla 🚀

Este repositorio es tu punto de partida ideal para proyectos basados en JavaScript puro (Vanilla JS). Está equipado con herramientas modernas para optimizar y mejorar tu experiencia de desarrollo.

## 🌟 Características

- **Vite ⚡**: Un build tool diseñado para ofrecerte un desarrollo veloz y construcciones de producción ultra-eficientes.

## 🚀 Configuración inicial

1. **Crea tu repositorio 🛠️**:

  En vez de clonar este repositorio directamente, haz clic en el botón "Use this template" (Usar esta plantilla) en la página principal del repositorio para crear un nuevo repositorio basado en esta plantilla.

2. **Node y NPM 📦**:

  Este proyecto utiliza **Node.js** y **NPM** para gestionar dependencias y scripts.
   - Asegúrate de instalar las dependencias del proyecto con:
     ```bash
     npm i
     ```
   - Usa los scripts definidos en `package.json` para tareas comunes, como desarrollo (`npm run dev`) o compilación (`npm run build`).

3. **Vite ⚡**:

  Vite ya está listo para usarse, pero puedes ajustar la configuración en `vite.config.js`.

4. **GitHub Actions 🤖**:

  Las acciones ya están preconfiguradas. Encuentra los detalles en `.github/workflows`.

5. **ESLint 🧹**:

  ESLint es una herramienta de análisis de código estático que identifica y reporta patrones encontrados en el código, ayudando a mantener un código de calidad y libre de errores.

6. **EditorConfig 📝**

  El plugin EditorConfig para VSCode asegura que todos los desarrolladores del proyecto sigan un estilo de codificación consistente. La configuración se define en el archivo `.editorconfig` en la raíz del proyecto.

7. **Prettier 🎨**

  Prettier es una herramienta de formateo de código que garantiza un estilo de código consistente en todo el proyecto. El plugin Prettier para VSCode ayuda a aplicar estas reglas automáticamente.

8. **Visual Studio Code 💻**:

  Este repositorio incluye un directorio `.vscode/` con:

  - **settings.json**: Configuración para formato automático, validación JS y aplicación de ESLint al guardar.
  - **extensions.json**: Lista de extensiones recomendadas.

  👉 De esta forma, cualquiera que clone el repositorio tendrá el mismo entorno base en VS Code.

## 📜 Comandos npm

Aquí están los comandos npm configurados y su explicación:

1. **`npm run dev`**:

  - Inicia el servidor de desarrollo utilizando Vite. Esto permite que el servidor se reinicie automáticamente cuando se detectan cambios en los archivos del proyecto.
  - Comando: `vite`

2. **`npm run build`**:

   - Compila los archivos JavaScript usando `vite build`.
   - Comando: `vite build`

3. **`npm run preview`**:

   - Previsualiza la aplicación construida utilizando `vite preview`.
   - Comando: `vite preview`

4. **`npm run lint`**:

   - Analiza el código en el directorio `src` usando ESLint para detectar y reportar problemas de estilo y errores.
   - Comando: `eslint src`

5. **`npm run lint:fix`**:

   - Ejecuta ESLint en el directorio `src` y automáticamente corrige los problemas que pueden ser solucionados.
   - Comando: `eslint src --fix`

6. **`npm run format`**:
   - Formatea el código en el directorio `src` usando Prettier, asegurando un estilo de código consistente.
   - Comando: `prettier --write src`

## 📢 Reglas de Git

- **Nunca hagas push directamente a `main`**.
  Esta rama está protegida mediante la acción [`protect-main.yml`](.github/workflows/protect-main.yml).

- **Crea siempre una rama aparte** para tus cambios y características.

- **Abre un Pull Request (PR)** para integrar tus cambios.
  Los PRs:
  - Dispararán el linting ESLint.
  - Requerirán revisión del propietario para cambios críticos (vía [`require-owner-approval.yml`](.github/workflows/require-owner-approval.yml)).

