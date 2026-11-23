# Cazador – Bestias (leveo 1–80)

**Estado:** recuperado como base heredada; pendiente de auditoría y pruebas en WoW 3.3.5a.

## Archivos
- `HUNTER_Abilities.xml`
- `HUNTER_Rotations.xml`

## Comportamiento heredado
- Busca habilidades por nombre en el libro de hechizos del cliente esES.
- Omite habilidades que no estén aprendidas.
- Mantiene la mascota, aplica Marca del cazador y usa prioridades de Bestias.
- Incluye modo de área y controles manuales.

## Controles heredados
- CTRL izquierdo: pausar/reanudar.
- ALT derecho: activar/desactivar modo de área (Multidisparo y habilidades AoE incluidas).

## Importante
Esta es una recuperación del XML anterior, no una versión validada. Antes de declararlo listo se revisarán las llamadas de API, condiciones de cooldown/GCD, casteos por nombre, manejo de mascota, traducciones exactas y controles. Luego se probará en cliente 3.3.5a.
