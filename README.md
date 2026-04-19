# NEXUS · Evaluación FP

PWA de evaluación criterial para Formación Profesional de Soldadura y Calderería.
Diseñada para docentes de FP de Andalucía (CFGM CMSYC).

## Instalación en GitHub Pages

### Paso 1: Crear cuenta en GitHub (si no tienes)
Ve a https://github.com y regístrate. Basta con tu email educaAnd o personal.

### Paso 2: Crear un repositorio nuevo
1. Pulsa el botón **+** arriba a la derecha → **New repository**
2. Nombre: `nexus` (o el que prefieras — saldrá en la URL final)
3. Descripción: lo que quieras
4. **Elige Private o Public** según prefieras (Public funciona bien, Private también)
5. Marca **Add a README file** (opcional)
6. Pulsa **Create repository**

### Paso 3: Subir los archivos
Tienes dos formas:

**A) Desde la web de GitHub (más fácil):**
1. En el repositorio pulsa **Add file** → **Upload files**
2. Arrastra TODOS estos archivos del paquete:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
3. Abajo escribe "Subida inicial" y pulsa **Commit changes**

**B) Con Git desde terminal (si sabes):**
```bash
git clone https://github.com/TUUSUARIO/nexus.git
cd nexus
# copia aquí los 5 archivos
git add .
git commit -m "Subida inicial"
git push
```

### Paso 4: Activar GitHub Pages
1. En el repositorio ve a **Settings** (rueda arriba)
2. En el menú lateral busca **Pages**
3. En **Source** elige: **Deploy from a branch**
4. En **Branch** elige: **main** y carpeta **/ (root)**
5. Pulsa **Save**
6. Espera 1-2 minutos

### Paso 5: Usar la app
Tu URL será algo como:
```
https://TUUSUARIO.github.io/nexus/
```

Abre esa URL en Chrome/Edge (PC) o Safari/Chrome (móvil) y verás la app funcionando. Desde ahí puedes:
- **PC (Chrome/Edge):** botón "Instalar" en la barra de direcciones
- **iPhone (Safari):** Compartir → Añadir a pantalla de inicio
- **Android (Chrome):** menú ⋮ → Instalar aplicación

Una vez instalada funciona sin conexión y los datos son persistentes.

## Privacidad

Esta app no envía datos a ningún servidor. Todo se guarda en IndexedDB del navegador del dispositivo. GitHub solo aloja el código, no ve los datos de evaluación.

## Actualizaciones

Cuando recibas una versión nueva del `index.html`:
1. En tu repositorio, entra en `index.html`
2. Pulsa el lápiz ✏ de arriba a la derecha
3. Borra el contenido y pega el nuevo
4. Abajo "Commit changes"
5. La app se actualiza sola en 1-2 minutos (el Service Worker detecta el cambio)

## Archivos del paquete

- `index.html` — aplicación completa (HTML + CSS + JS todo en uno)
- `manifest.json` — metadatos PWA para instalación
- `sw.js` — Service Worker para funcionamiento offline
- `icon-192.png` — icono 192×192 (PWA estándar)
- `icon-512.png` — icono 512×512 (PWA estándar)

## Licencia

Uso personal docente. Autor: Xurxo.
