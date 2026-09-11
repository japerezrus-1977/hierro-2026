# El Hierro 2026 · Diario de viaje

Álbum web del viaje a El Hierro (18–24 de agosto de 2026): 70 fotos seleccionadas de entre las originales, organizadas día a día con una breve descripción de cada una.

## Ver la web en local

Al ser un sitio estático, basta con abrir `index.html` en el navegador, o servirlo con cualquier servidor estático, por ejemplo:

```
python3 -m http.server 8000
```

y abrir `http://localhost:8000`.

## Publicarla en GitHub Pages

1. Crea el repositorio y sube este contenido (sustituye `TU-USUARIO` y el nombre que quieras darle):

   ```
   git init
   git add .
   git commit -m "Diario de viaje: El Hierro 2026"
   gh repo create TU-USUARIO/hierro-2026 --public --source=. --remote=origin --push
   ```

   (`--public` lo hace visible a cualquiera con el enlace; usa `--private` si prefieres restringirlo — ten en cuenta que GitHub Pages solo funciona con repos privados en planes GitHub Pro/Team/Enterprise).

2. Activa GitHub Pages: en la página del repo en GitHub, ve a **Settings → Pages**, y en "Build and deployment" elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`. Guarda.

3. Al cabo de uno o dos minutos, la web estará disponible en:

   ```
   https://TU-USUARIO.github.io/hierro-2026/
   ```

## Estructura

```
index.html       página principal (generada)
css/style.css     estilos
js/main.js        navegación y visor de fotos (lightbox)
img/dia1..dia7/   fotos optimizadas para web, una carpeta por día
```
