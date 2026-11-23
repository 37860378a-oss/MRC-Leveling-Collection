# Perfiles MRC – formato DarhangeR

Los perfiles de MRC se desarrollan para **PQR en WoW 3.3.5a**, respetando la estructura original de DarhangeR.

## Convenciones

- Los archivos del perfil se ubican en la carpeta `Profiles` del ejecutor.
- Se mantiene la separación habitual entre `*_Abilities.xml` y `*_Rotations.xml`.
- No usar carpetas inventadas como `PQR_Abilities` o `PQR_Rotations`.
- Antes de adaptar un perfil existente, conservar y revisar sus funciones auxiliares, condiciones, objetivos y tiempos de reutilización.
- Priorizar el lanzamiento por nombre de hechizo cuando la estructura y el código del perfil lo permitan.
- Toda habilidad debe comprobarse antes de usarla: si el personaje aún no la aprendió, se omite sin bloquear el resto de la rotación.

## Estructura XML de referencia

Los archivos de habilidades DarhangeR usan una raíz por clase (por ejemplo, `<WARRIOR>`) y entradas `<Ability>` con campos como:

- `Name`, `Default`, `SpellID`, `Actions`, `Lua`
- `RecastDelay`, `Target`, `CancelChannel`
- `LuaBefore`, `LuaAfter`

Los archivos de rotaciones definen, entre otros campos, `RotationName`, `RotationDefault`, `RotationList`, `RequireCombat` y `RotationNotes`.

Esta lista documenta la estructura conocida; el XML real de cada perfil debe tomarse como referencia antes de generar archivos nuevos.

## Organización de MRC

Cada clase y árbol tendrá su propia carpeta dentro de `Profiles`. Cada perfil incluirá:

- XML de habilidades.
- XML de rotaciones.
- README con compatibilidad, nivel, talentos, habilidades y controles.
- Registro de pruebas y cambios relevantes.

No se agregan perfiles vacíos como si estuvieran terminados. Un perfil solo se considera validado después de probarlo en el cliente 3.3.5a.
