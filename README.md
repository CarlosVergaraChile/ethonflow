# Ethon

Sitio estatico listo para publicar en GitHub y Hostinger.

## Configuracion recomendada

Este repositorio debe ser la fuente unica de verdad para EthonFlow. Hostinger queda como servidor publico y GitHub como historial/versionado.

Flujo recomendado:

1. Editar siempre en esta carpeta local.
2. Revisar el sitio localmente.
3. Guardar cambios en Git con un commit.
4. Subir a GitHub.
5. Publicar en Hostinger subiendo el contenido de `deploy` a `public_html`.

## Estructura publica

- `deploy/index.html`: portada principal si se publica en la raiz del dominio.
- `deploy/ethon/index.html`: landing recomendada para `https://glstrategic.cl/ethon/`.
- `deploy/ethonCOM/index.html`: version comercial.
- `deploy/ethonCEO/index.html`: version enterprise/CEO.
- Archivos HTML originales en la raiz: versiones historicas de trabajo.

## Publicar en Hostinger

1. Entra a hPanel de Hostinger.
2. Abre el administrador de archivos del dominio.
3. Entra a `public_html`.
4. Sube el contenido de la carpeta `deploy`, no la carpeta completa.
5. Verifica que `public_html/index.html` exista.
6. Las rutas quedaran asi:
   - `/`
   - `/ethon/`
   - `/ethonCOM/`
   - `/ethonCEO/`

Si no quieres reemplazar la home principal de `glstrategic.cl`, sube solo la carpeta `deploy/ethon` como `public_html/ethon`.

## Publicar con GitHub Pages

1. Crea un repositorio en GitHub.
2. Sube este proyecto al repositorio.
3. En GitHub, abre `Settings > Pages`.
4. En `Build and deployment`, selecciona `Deploy from a branch`.
5. Elige la rama `main` y la carpeta `/deploy`.
6. Guarda los cambios.

## Comandos Git sugeridos

```powershell
git init
git add .
git commit -m "Initial static site setup"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/TU_REPOSITORIO.git
git push -u origin main
```
