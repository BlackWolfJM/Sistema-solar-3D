# 🚀 Setup and Deployment Guide / Guía de Instalación y Despliegue

[English](#english) | [Español](#español)

---

<a name="english"></a>
## 🇬🇧 English

### ⚠️ IMPORTANT: This is a React Project

**You CANNOT open the `index.html` file directly in your browser.** You need to build the application first.

### 📋 Prerequisites

#### Install Node.js and npm

1. Go to [https://nodejs.org/](https://nodejs.org/)
2. Download the **LTS** version (recommended)
3. Install the downloaded file
4. Verify the installation by opening your terminal/PowerShell:
   ```bash
   node --version
   npm --version
   ```

### 💻 Local Execution (Development)

1. **Open your terminal in the project folder:**
   ```bash
   cd path/to/project/frontend
   ```

2. **Install dependencies (first time only):**
   ```bash
   npm install --legacy-peer-deps
   ```

3. **Start the development server:**
   ```bash
   npm start
   ```

**The application will automatically open in your browser at `http://localhost:3000`**

### 🌐 Deploy to Netlify (FREE)

#### Method 1: Deploy from GitHub (Recommended)

1. **Upload your code to GitHub:**
   ```bash
   # Initialize git (if you haven't already)
   git init
   git add .
   git commit -m "Initial commit"
   
   # Create a repository on GitHub and connect it
   git remote add origin https://github.com/YOUR-USERNAME/solar-system-3d.git
   git push -u origin main
   ```

2. **Connect Netlify:**
   - Go to [https://www.netlify.com/](https://www.netlify.com/)
   - Create an account (free)
   - Click "Add new site" → "Import an existing project"
   - Select GitHub and authorize
   - Select your repository

3. **Configure the build:**
   - Base directory: `frontend`
   - Build command: `npm run build`
   - Publish directory: `frontend/build` (or just `build` if base directory is set)
   - Click "Deploy site"

✅ **Done! Your site will be live on a URL like `https://your-site.netlify.app`**

#### Method 2: Manual Deploy (Drag & Drop)

1. **Build locally:**
   ```bash
   cd frontend
   npm install --legacy-peer-deps
   npm run build
   ```

2. **Upload to Netlify:**
   - Go to [https://app.netlify.com/drop](https://app.netlify.com/drop)
   - Drag and drop the `build` folder onto the page
   - Your site will be live immediately!

---

<a name="español"></a>
## 🇪🇸 Español

### ⚠️ IMPORTANTE: Este es un proyecto React

**NO puedes abrir el archivo `index.html` directamente en el navegador**. Necesitas compilar la aplicación primero.

### 📋 Pre-requisitos

#### Instalar Node.js y npm

1. Ve a [https://nodejs.org/](https://nodejs.org/)
2. Descarga la versión **LTS** (recomendada)
3. Instala el archivo descargado
4. Verifica la instalación abriendo tu terminal/PowerShell:
   ```bash
   node --version
   npm --version
   ```

### 💻 Ejecución Local (Desarrollo)

1. **Abre tu terminal en la carpeta del proyecto:**
   ```bash
   cd ruta/al/proyecto/frontend
   ```

2. **Instala las dependencias (solo la primera vez):**
   ```bash
   npm install --legacy-peer-deps
   ```

3. **Inicia el servidor de desarrollo:**
   ```bash
   npm start
   ```

**La aplicación se abrirá automáticamente en tu navegador en `http://localhost:3000`**

### 🌐 Deploy en Netlify (GRATIS)

#### Método 1: Deploy desde GitHub (Recomendado)

1. **Sube tu código a GitHub:**
   ```bash
   # Inicializa git (si no lo has hecho)
   git init
   git add .
   git commit -m "Initial commit"
   
   # Crea un repositorio en GitHub y conéctalo
   git remote add origin https://github.com/TU-USUARIO/solar-system-3d.git
   git push -u origin main
   ```

2. **Conecta Netlify:**
   - Ve a [https://www.netlify.com/](https://www.netlify.com/)
   - Crea una cuenta (gratis)
   - Haz clic en "Add new site" → "Import an existing project"
   - Selecciona GitHub y autoriza
   - Selecciona tu repositorio

3. **Configura el build:**
   - Base directory: `frontend`
   - Build command: `npm run build`
   - Publish directory: `frontend/build` (o solo `build` si el base directory está configurado)
   - Haz clic en "Deploy site"

✅ **¡Listo! Tu sitio estará en vivo en una URL como `https://tu-sitio.netlify.app`**

#### Método 2: Deploy Manual (Drag & Drop)

1. **Crea el build localmente:**
   ```bash
   cd frontend
   npm install --legacy-peer-deps
   npm run build
   ```

2. **Sube a Netlify:**
   - Ve a [https://app.netlify.com/drop](https://app.netlify.com/drop)
   - Arrastra la carpeta `build` a la página
   - ¡Tu sitio estará en vivo inmediatamente!
