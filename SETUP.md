# 🚀 Guía Completa de Instalación y Deployment

## ⚠️ IMPORTANTE: Este es un proyecto React

**NO puedes abrir el archivo `index.html` directamente en el navegador**. Necesitas compilar la aplicación primero.

---

## 📋 Pre-requisitos

### Instalar Node.js y npm

1. Ve a [https://nodejs.org/](https://nodejs.org/)
2. Descarga la versión **LTS** (recomendada)
3. Instala el archivo descargado
4. Verifica la instalación abriendo PowerShell:
   ```bash
   node --version
   npm --version
   ```

---

## 💻 Ejecución Local (Desarrollo)

### Opción 1: Desde la carpeta completa

```bash
# 1. Abre PowerShell en la carpeta del proyecto
cd C:\Users\cueva\Downloads\Emergent-main\Emergent-main\frontend

# 2. Instala las dependencias (solo la primera vez)
npm install

# 3. Inicia el servidor de desarrollo
npm start
```

**La aplicación se abrirá automáticamente en tu navegador en `http://localhost:3000`**

### Opción 2: Build de producción local

```bash
# 1. Crea el build de producción
npm run build

# 2. Instala un servidor local simple
npm install -g serve

# 3. Sirve la aplicación
serve -s build
```

---

## 🌐 Deploy en Netlify (GRATIS)

### Método 1: Deploy desde GitHub (Recomendado)

1. **Sube tu código a GitHub:**
   ```bash
   # Inicializa git (si no lo has hecho)
   cd C:\Users\cueva\Downloads\Emergent-main\Emergent-main
   git init
   git add .
   git commit -m "Initial commit"
   
   # Crea un repositorio en GitHub y conecta
   git remote add origin https://github.com/TU-USUARIO/solar-system-3d.git
   git push -u origin main
   ```

2. **Conecta Netlify:**
   - Ve a [https://www.netlify.com/](https://www.netlify.com/)
   - Crea una cuenta (gratis)
   - Click en "Add new site" → "Import an existing project"
   - Selecciona GitHub y autoriza
   - Selecciona tu repositorio

3. **Configura el build:**
   - Base directory: `frontend`
   - Build command: `npm run build`
   - Publish directory: `frontend/build`
   - Click "Deploy site"

✅ **¡Listo! Tu sitio estará en vivo en una URL como `https://tu-sitio.netlify.app`**

### Método 2: Deploy Manual (Drag & Drop)

1. **Crea el build localmente:**
   ```bash
   cd frontend
   npm install
   npm run build
   ```

2. **Sube a Netlify:**
   - Ve a [https://app.netlify.com/drop](https://app.netlify.com/drop)
   - Arrastra la carpeta `build` a la página
   - ¡Tu sitio estará en vivo inmediatamente!

---

## 📁 Estructura del Proyecto Limpio

```
Emergent-main/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   └── SolarSystem.jsx
│   │   ├── data/
│   │   │   └── planets.js
│   │   ├── App.js
│   │   └── index.js
│   ├── package.json
│   └── ...
├── netlify.toml
├── README.md
└── .gitignore
```

---

## 🐛 Solución de Problemas

### Error: "npm no se reconoce"
- **Solución:** Instala Node.js desde [nodejs.org](https://nodejs.org/)

### Error: "Cannot find module"
- **Solución:** Ejecuta `npm install` en la carpeta `frontend`

### La página está en blanco
- **Solución:** Abre la consola del navegador (F12) para ver errores
- Verifica que ejecutaste `npm start` en la carpeta correcta

### El CSS no se carga
- **Solución:** Limpia la caché del navegador y recarga con Ctrl+Shift+R

---

## 📝 Cambios Realizados al Proyecto

### Archivos Eliminados:
- ✅ `.emergent/` - Configuración de Emerge.ia
- ✅ `test_result.md` - Protocolo de testing de IA
- ✅ `.gitconfig` - Config específica de IA
- ✅ `backend/` - No necesario para este proyecto
- ✅ `tests/` - Tests vacíos
- ✅ `mockData.js` - Movido a `data/planets.js`

### Código Limpiado:
- ✅ Eliminados comentarios tipo "Enhanced...", "Individual Component", etc.
- ✅ Removidos comentarios obvios y descriptivos de IA
- ✅ Reorganizada estructura de carpetas (`data/planets.js`)
- ✅ Simplificado sin perder funcionalidad

### Archivos Nuevos/Actualizados:
- ✅ `README.md` - Documentación profesional
- ✅ `netlify.toml` - Configuración para deployment
- ✅ `.gitignore` - Gitignore limpio
- ✅ `SETUP.md` - Esta guía

---

## 🎯 ¿Qué hacer ahora?

1. **Instala Node.js** si no lo tienes
2. **Ejecuta localmente** con `npm install` y `npm start`
3. **Súbelo a GitHub** para control de versiones
4. **Despliega en Netlify** para tenerlo en vivo

¡Tu proyecto está 100% limpio y listo para publicar! 🎉
