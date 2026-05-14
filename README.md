# Ethon

Sitio estatico listo para publicar en GitHub y Hostinger.

## Estructura

- `deploy/index.html`: portada principal con accesos a las versiones disponibles.
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
   - `/ethonCOM/`
   - `/ethonCEO/`

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
