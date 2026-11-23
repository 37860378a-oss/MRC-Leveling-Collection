# MRC – Modular Rotation Collection

Colección modular de perfiles de rotación para **World of Warcraft 3.3.5a (Wrath of the Lich King)**, orientada al leveo y adaptable al progreso del personaje entre los niveles **1 y 80**.

> MRC no es una rotación única: cada clase y árbol de talentos tendrá su propio perfil, con prioridades y modos de combate configurables.

## Objetivos

- Perfiles independientes para los **30 árboles de talentos oficiales** de WotLK.
- Adaptación al nivel, talentos y hechizos realmente aprendidos.
- Modo **Unitarget** como comportamiento normal y modo **AoE** activado mediante tecla modificadora.
- Controles opcionales para defensivos, interrupciones y cooldowns.
- Documentación clara de prioridades, controles y requisitos.
- Desarrollo incremental, pruebas en cliente 3.3.5a y cambios versionados en GitHub.

## Ejecutor y formato de perfiles

MRC utilizará **PQR con la estructura de perfiles de DarhangeR** que veníamos usando. PQR es el ejecutor; MRC es la colección que organiza y mantiene los perfiles.

- Los perfiles respetarán la estructura original de DarhangeR dentro de la carpeta `Profiles`.
- Se conservará la separación entre archivos de habilidades (`*_Abilities.xml`) y rotaciones (`*_Rotations.xml`) cuando corresponda al perfil.
- No se crearán carpetas alternativas como `PQR_Abilities` o `PQR_Rotations`.
- Antes de incorporar un perfil antiguo, se revisará su XML y sus funciones auxiliares para mantener compatibilidad.
- Los perfiles se adaptarán para no intentar lanzar habilidades que el personaje todavía no aprendió.

## Clases y perfiles

| Clase | Árboles |
|---|---|
| Guerrero | Armas · Furia · Protección |
| Paladín | Sagrado · Protección · Reprensión |
| Cazador | Bestias · Puntería · Supervivencia |
| Pícaro | Asesinato · Combate · Sutileza |
| Sacerdote | Disciplina · Sagrado · Sombras |
| Caballero de la Muerte | Sangre · Escarcha · Profano |
| Chamán | Elemental · Mejora · Restauración |
| Mago | Arcano · Fuego · Escarcha |
| Brujo | Aflicción · Demonología · Destrucción |
| Druida | Equilibrio · Feral · Restauración |

**Nota sobre Druida:** en 3.3.5a no existe Guardián como árbol separado. El árbol Feral contempla tanto el estilo DPS como el de tanque; podremos documentarlos como variantes sin presentarlos como especializaciones oficiales distintas.

## Controles

La propuesta inicial es mantener Unitarget sin modificador y activar AoE al mantener una tecla (por ejemplo, SHIFT). Las teclas definitivas y las prioridades por clase se documentarán en [docs/KEYBINDS.md](docs/KEYBINDS.md).

## Estructura

- `Profiles/`: archivos compatibles con la estructura de perfiles DarhangeR.
- `docs/`: controles, matriz de perfiles y guías de pruebas.
- Cada perfil incluirá su documentación y requisitos de nivel/habilidades.

## Estado del proyecto

**Fase 2 – Estructura inicial de las 30 especializaciones creada.** Cada especialización tiene su carpeta, XML de habilidades, XML de rotación y README. Hunter Bestias conserva su base heredada recuperada. Las demás bases son esqueletos funcionales de estructura y prioridades iniciales, todavía pendientes de auditoría técnica, corrección de nombres localizados y pruebas en cliente. Ningún perfil se considera validado hasta probarlo en WoW 3.3.5a.

## Compatibilidad y uso

- Cliente objetivo: WoW 3.3.5a.
- Ejecutor: PQR, estructura de perfiles DarhangeR.
- Antes de ejecutar cualquier perfil, revisá sus instrucciones y requisitos.
- Probá primero en un entorno seguro y reportá errores con clase, nivel, talentos, objetivo y mensaje de error.

## Desarrollo

Se priorizará recuperar y revisar los trabajos previos de Hunter y Warrior. No se dará por hecho que código antiguo es compatible hasta inspeccionarlo y probarlo.
