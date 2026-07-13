# Galactifun2-drake

[![Rama](https://img.shields.io/badge/branch-1.21--latin-2ea44f)](https://github.com/DrakesCraft-Labs/Galactifun2-drake/tree/1.21-latin)
[![Licencia](https://img.shields.io/github/license/DrakesCraft-Labs/Galactifun2-drake)](https://github.com/DrakesCraft-Labs/Galactifun2-drake/blob/1.21-latin/LICENSE)
[![Ultimo commit](https://img.shields.io/github/last-commit/DrakesCraft-Labs/Galactifun2-drake/1.21-latin)](https://github.com/DrakesCraft-Labs/Galactifun2-drake/commits/1.21-latin)

Galactifun2 Drake es un addon espacial para Slimefun Drake con planetas,
exploración y componentes de progresión avanzada.

## Qué añade a Slimefun
- Expansión de contenido end-game con enfoque de exploración espacial.
- Recetas y componentes para progresión extendida.
- Eventos/entornos dedicados para gameplay temático.

## Características principales
- Mundo(s) espaciales y progresión por etapas.
- Ítems/máquinas temáticas para cadena tecnológica de late-game.
- Integración con utilidades internas de Drake para mantenimiento.

## Matriz de compatibilidad
| Componente | Estado |
|---|---|
| Minecraft / Paper / Purpur | **1.21.11** |
| Slimefun Core Drake | **11** (línea `1.21-latin`) |
| Java | 21 |

## Instalación
1. Construye el artefacto sombreado de la rama `1.21-latin`.
2. Respalda el JAR y `plugins/Galactifun2/` antes de una actualización.
3. Instala un único JAR durante una ventana de reinicio.
4. Valida en staging un menú, una receta y una interacción de mundo existente.

## Build local
```bash
./gradlew :plugin:shadowJar
```

Artefacto esperado:
- `plugin/build/libs/galactifun2-*-all.jar`

## Flujo de release
1. Crear branch de cambios (`feature/*` o `fix/*`).
2. Abrir PR hacia `1.21-latin` con plan de pruebas.
3. Al mergear, crear tag/release y publicar jar compilado.

Publicar el artefacto `-all.jar` y validar carga en Paper/Purpur antes del
release. El addon no descarga binarios ni aplica actualizaciones en caliente.

## Relación con el monorepo
Este repositorio es la fuente de desarrollo aislado por addon y despliegues
independientes. Sus cambios deben preservar IDs, recetas, mundos y datos de
jugadores existentes.
