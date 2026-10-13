# Hello World

Página web estática sencilla que muestra "Hello World", lista para desplegar en Netlify.

## Estructura

```
public/
  index.html   # Página principal
  404.html     # Página de error 404
netlify.toml   # Configuración de Netlify
```

## Desplegar en Netlify

### Opción 1: Desde GitHub (recomendado)
1. Entra en [app.netlify.com](https://app.netlify.com) → **Add new site** → **Import an existing project**.
2. Conecta GitHub y elige este repositorio.
3. Netlify leerá `netlify.toml` automáticamente (directorio de publicación: `public`, sin comando de build).
4. Pulsa **Deploy**.

### Opción 2: Arrastrar y soltar
Arrastra la carpeta `public/` a [app.netlify.com/drop](https://app.netlify.com/drop).

### Opción 3: Netlify CLI
```bash
npm install -g netlify-cli
netlify deploy --prod --dir=public
```

## Ver en local
```bash
npx serve public
# o
python3 -m http.server -d public 8000
```
