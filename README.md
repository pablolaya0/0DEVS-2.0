# 0Devs — Web

Web estática de 0Devs, en español, con diseño glassmorphism minimalista, fondo blanco y color principal **#89ADC5**.

Incluye las secciones de soluciones, proceso, ventaja, equipo y contacto. Los botones enlazan a https://cal.com/0devs y a info@0devs.es.

## Abrir la web

Abre `index.html` en un navegador. No requiere instalar dependencias ni ejecutar un proceso de compilación.

Para servirla localmente, de forma opcional:

```sh
python3 -m http.server 3000
```

Visita http://localhost:3000.

## Archivos

- `index.html`: página completa con HTML, CSS, JavaScript, fuentes y logos integrados. Es el único archivo necesario para mostrar la web.
- `.nojekyll`: desactiva el procesamiento de Jekyll en GitHub Pages.
- `.gitignore`: excluye archivos temporales y credenciales locales.

Los cambios de textos, enlaces y estilos se realizan directamente en `index.html`. La ilustración de automatización es un ejemplo visual, no un servicio de automatización conectado.

## Subir a GitHub desde el navegador

1. Crea un repositorio en https://github.com/new o abre uno existente.
2. En el repositorio, selecciona **Add file → Upload files**.
3. Extrae el ZIP y sube sus archivos, no el ZIP. `index.html` debe quedar en la raíz del repositorio.
4. Confirma los cambios con **Commit changes**.

## Publicar con GitHub Pages

En un repositorio público, o en uno privado si tu plan lo permite:

1. Abre **Settings → Pages**.
2. En **Build and deployment**, selecciona **Deploy from a branch**.
3. Selecciona la rama que contiene los archivos (normalmente `main`) y la carpeta **/ (root)**.
4. Pulsa **Save**. GitHub mostrará la URL cuando finalice la publicación.

No se incluye un dominio personalizado. Para utilizar `0devs.es`, configura el dominio en GitHub Pages y sus registros DNS después de publicar.

## Subir desde la terminal

Autentícate primero en GitHub desde tu equipo. Después, en la carpeta extraída, ejecuta:

```sh
git init -b main
git add .
git commit -m "Añadir web de 0Devs"
git remote add origin https://github.com/TU_USUARIO/TU_REPOSITORIO.git
git push -u origin main
```

Sustituye `TU_USUARIO` y `TU_REPOSITORIO`. Estos comandos están pensados para un repositorio remoto nuevo y vacío. No incluyas contraseñas ni tokens en los archivos.
