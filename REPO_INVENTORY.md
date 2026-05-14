# Inventario GitHub

Fuente: API publica de GitHub para `CarlosVergaraChile`, revisada el 2026-05-14.

No borrar repositorios todavia. Primero archivar o fusionar solo con confirmacion explicita.

## Reglas de decision

- `KEEP`: repositorio activo o fuente oficial.
- `MERGE`: contiene material util que debe integrarse a otro repo.
- `ARCHIVE`: conservar como historico, solo lectura.
- `DELETE_CANDIDATE`: posible eliminacion solo despues de confirmar que no contiene material unico.
- `REVIEW`: requiere inspeccion de contenido antes de decidir.

## Repos publicos

| Repo | Lenguaje | Ultima actualizacion | Estado sugerido | Motivo |
| --- | --- | --- | --- | --- |
| `ethonflow` | n/d | 2026-05-14 | `KEEP` | Fuente oficial de EthonFlow. |
| `ai-pr-orchestrator` | n/d | 2026-05-07 | `REVIEW` | Orquestador multi-IA; posible utilidad transversal. |
| `coipo-orchestrator` | n/d | 2026-05-07 | `REVIEW` | Orquestador COIPO/n8n; revisar si sigue activo. |
| `shared-libs` | Python | 2026-05-06 | `KEEP` | Librerias compartidas del ecosistema. |
| `coipo-stuff` | TypeScript | 2026-05-06 | `REVIEW` | Modulo upload; revisar si pertenece a COIPO. |
| `payment-gateway-standard` | n/d | 2026-05-05 | `KEEP` | Estandar reusable de pagos. |
| `Sam-app` | TypeScript | 2026-05-05 | `KEEP` | App SAM principal probable. |
| `prisma` | HTML | 2026-05-02 | `REVIEW` | Sin descripcion; revisar contenido. |
| `gl-strategic-engine` | HTML | 2026-04-29 | `MERGE` | Probable relacion con Ethon/GL; revisar integracion. |
| `NovisEye` | PHP | 2026-04-03 | `REVIEW` | Producto/dashboard independiente. |
| `sam-app-mvp` | TypeScript | 2026-01-25 | `MERGE` | Probable version anterior de `Sam-app`. |
| `audio-compressor-notebooklm` | Python | 2026-01-13 | `KEEP` | Herramienta puntual y clara. |
| `SAM` | HTML | 2026-01-11 | `MERGE` | Probable version HTML/historica de SAM. |
| `documentation-hub` | n/d | 2026-01-10 | `KEEP` | Hub documental transversal. |
| `gem-auditor-deploy` | n/d | 2026-01-10 | `REVIEW` | Auditoria convergente; puede ser util transversal. |
| `dashboard-proyectos` | HTML | 2026-01-10 | `REVIEW` | Puede ayudar al inventario; revisar antes de archivar. |
| `sam-landing-page` | HTML | 2026-01-09 | `MERGE` | Probable landing anterior de SAM. |
| `GL-Strategic-Web-Site` | HTML | 2025-12-25 | `MERGE` | Posible duplicado web GL. |
| `Image_enhancement` | Python | 2025-12-25 | `ARCHIVE` | Script puntual; archivar si no se usa. |
| `GL-Strategic` | n/d | 2025-12-20 | `KEEP` | Probable repo web corporativo principal GL. |
| `portfolio-carlosv` | HTML | 2025-12-19 | `KEEP` | Sitio profesional personal. |
| `ecosystem-standards` | n/d | 2025-12-17 | `KEEP` | Estandares reutilizables. |
| `flipbook-pwa-template` | HTML | 2025-12-17 | `KEEP` | Template reusable claro. |
| `Proyecto-Sence-2026` | n/d | 2025-12-17 | `KEEP` | Proyecto activo/nominal 2026. |
| `cosas-i-doodle-shop` | JavaScript | 2025-12-17 | `KEEP` | Producto e-commerce independiente. |
| `deploy-guide` | n/d | 2025-12-16 | `MERGE` | Podria integrarse a `documentation-hub`. |
| `seasonal-market-standard` | n/d | 2025-12-16 | `MERGE` | Podria integrarse a `ecosystem-standards`. |
| `course-module-standard` | n/d | 2025-12-16 | `MERGE` | Podria integrarse a `ecosystem-standards`. |
| `marketing-digital-standard` | n/d | 2025-12-16 | `MERGE` | Podria integrarse a `ecosystem-standards`. |
| `maquina-orquestadora-gl-strategic` | Python | 2025-12-15 | `REVIEW` | Relacionado a GL; revisar si reemplaza otros orquestadores. |
| `gl-strategic-mvp` | n/d | 2025-12-15 | `MERGE` | Posible version anterior de GL Strategic. |
| `lean-healthcare-manual` | HTML | 2025-04-29 | `ARCHIVE` | Manual puntual antiguo; archivar si no esta activo. |

## Acciones recomendadas

1. Mantener como oficiales: `ethonflow`, `GL-Strategic`, `Sam-app`, `shared-libs`, `documentation-hub`, `ecosystem-standards`.
2. Fusionar familias duplicadas:
   - Familia GL: `GL-Strategic`, `GL-Strategic-Web-Site`, `gl-strategic-engine`, `gl-strategic-mvp`.
   - Familia SAM: `Sam-app`, `SAM`, `sam-app-mvp`, `sam-landing-page`.
   - Familia standards: `ecosystem-standards`, `marketing-digital-standard`, `course-module-standard`, `seasonal-market-standard`.
3. Archivar candidatos de bajo riesgo despues de revisar contenido: `Image_enhancement`, `lean-healthcare-manual`.
4. No eliminar nada hasta confirmar que no hay dominios, secrets, workflows, datos o codigo unico.

## Pendiente con permisos privados

Cuando el conector GitHub tenga permisos completos, levantar tambien:

- Repos privados.
- Secrets/actions/domains/GitHub Pages.
- Ultimo commit real por rama.
- Tamano del repo.
- Issues/PRs abiertos.
