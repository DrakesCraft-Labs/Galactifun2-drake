# Galactifun2-drake

[![Rama](https://img.shields.io/badge/branch-1.21--latin-2ea44f)](https://github.com/DrakesCraft-Labs/Galactifun2-drake/tree/1.21-latin)
[![Licencia](https://img.shields.io/github/license/DrakesCraft-Labs/Galactifun2-drake)](https://github.com/DrakesCraft-Labs/Galactifun2-drake/blob/1.21-latin/LICENSE)
[![Ultimo commit](https://img.shields.io/github/last-commit/DrakesCraft-Labs/Galactifun2-drake/1.21-latin)](https://github.com/DrakesCraft-Labs/Galactifun2-drake/commits/1.21-latin)

## Descripción técnica
Addon espacial para Slimefun con planetas, contenido de exploración y componentes avanzados.

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
| Minecraft | 1.21.x |
| Paper/Purpur | 1.21.x |
| Slimefun Core Drake | 11.x (línea `1.21-latin`) |
| Java | 21 |

## Instalación
1. Descarga el `.jar` de Releases del repositorio.
2. Copia el archivo en la carpeta `plugins/` del servidor.
3. Asegura dependencias (`Slimefun`, `ProtocolLib` u otras según addon).
4. Reinicia el servidor y revisa `logs/latest.log` para validar carga.

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

Publicar artefacto `-all.jar` y validar carga en Purpur antes del release.

## Relación con el monorepo
Este repositorio se mantiene en paralelo con `drakes-slimefun-labs` para desarrollo aislado por addon y despliegues independientes.