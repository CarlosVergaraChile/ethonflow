# Inventario GitHub

Estado inicial: pendiente de auditoria completa con permisos API o revision manual.

## Reglas de decision

- `KEEP`: repositorio activo o fuente oficial.
- `MERGE`: contiene material util que debe integrarse a otro repo.
- `ARCHIVE`: conservar como historico, solo lectura.
- `DELETE_CANDIDATE`: posible eliminacion solo despues de confirmar que no contiene material unico.

## Repos conocidos por GitHub Desktop

| Repo | Estado sugerido | Motivo |
| --- | --- | --- |
| `CarlosVergaraChile/ethonflow` | `KEEP` | Fuente oficial de EthonFlow. |
| `CarlosVergaraChile/GL-Strategic` | `REVIEW` | Posible repo relacionado al sitio/empresa. |
| `CarlosVergaraChile/GL-Strategic-Web-Site` | `REVIEW` | Posible duplicado web. |
| `CarlosVergaraChile/GL-Web-Master` | `REVIEW` | Posible version antigua o master web. |
| `CarlosVergaraChile/Doodle` | `REVIEW` | Revisar si es prueba o producto. |
| `CarlosVergaraChile/Image_enhancement` | `REVIEW` | Revisar si es util o experimento. |
| `CarlosVergaraChile/NovisEye` | `REVIEW` | Revisar estado/producto. |
| `CarlosVergaraChile/Proyecto-Sence-2026` | `REVIEW` | Mantener si esta activo. |
| `CarlosVergaraChile/SAM` | `REVIEW` | Posible duplicado con `Sam-app`. |
| `CarlosVergaraChile/Sam-app` | `REVIEW` | Posible duplicado con `SAM`. |
| `CarlosVergaraChile/ai-pr-orchestrator` | `REVIEW` | Revisar uso actual. |

## Siguiente auditoria

Cuando el conector GitHub tenga permisos, levantar para cada repo:

- Ultimo commit.
- Lenguaje/framework.
- Tamano.
- README.
- Dominio o GitHub Pages.
- Issues/PRs abiertos.
- Posibles secretos o datos sensibles.
