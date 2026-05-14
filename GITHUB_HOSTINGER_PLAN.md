# Plan GitHub + Hostinger

## Decision principal

Usar un solo repositorio principal para EthonFlow.

Nombre recomendado del repositorio:

```text
ethonflow
```

Este repositorio debe contener:

- Version publica lista para Hostinger en `deploy/`.
- Landing en `deploy/ethon/`.
- Tablero comercial en `deploy/ethonCOM/`.
- Tablero CEO/enterprise en `deploy/ethonCEO/`.
- Versiones historicas en `archive/versions/`.
- Assets fuente en `assets/source/`.

## Rutas publicas recomendadas

```text
https://glstrategic.cl/ethon/
https://glstrategic.cl/ethonCOM/
https://glstrategic.cl/ethonCEO/
```

## Regla de trabajo

1. El codigo fuente se modifica localmente.
2. Cada avance util se guarda con `git commit`.
3. GitHub guarda la historia y permite recuperar versiones.
4. Hostinger recibe solo lo que este dentro de `deploy/`.

## Ramas

- `main`: trabajo, documentacion, archivo historico y version publica en `deploy/`.
- `hostinger`: rama limpia para Hostinger; contiene solo lo que debe quedar en `public_html`.

## Limpieza de repos GitHub

No eliminar repositorios de inmediato. Primero clasificarlos:

- `KEEP`: repo vivo, fuente de verdad o producto activo.
- `MERGE`: repo repetido o version vieja que debe integrarse al principal.
- `ARCHIVE`: repo historico que conviene dejar solo lectura.
- `DELETE_CANDIDATE`: repo vacio, prueba descartable o duplicado confirmado.

Antes de borrar cualquier repo:

1. Confirmar que no tiene dominio, workflow, issue o secreto importante.
2. Confirmar que no contiene codigo unico.
3. Hacer backup o archive si hay duda.
4. Borrar solo con confirmacion explicita.

## Proximo paso tecnico

Conectar GitHub a esta sesion o instalar/autorizar GitHub CLI. Luego:

```powershell
git remote add origin https://github.com/CarlosVergaraChile/ethonflow.git
git push -u origin main
```

Si el repo ya existe, solo se agrega ese remoto. Si no existe, se crea primero en GitHub.
