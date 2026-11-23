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

- profiles/: perfiles por clase y árbol de talentos.
- docs/: controles, matriz de perfiles y guías de pruebas.
- Cada perfil incluirá su documentación y requisitos de nivel/habilidades.

## Estado del proyecto

**Fase 0 – Base del repositorio.** La estructura y las convenciones se están preparando. Los perfiles se incorporarán de forma gradual; ningún perfil se considerará validado hasta probarlo en el cliente objetivo.

## Compatibilidad y uso

- Cliente objetivo: WoW 3.3.5a.
- Antes de ejecutar cualquier perfil, revisá sus instrucciones y requisitos.
- Probá primero en un entorno seguro y reportá errores con clase, nivel, talentos, objetivo y mensaje de error.

## Desarrollo

Se priorizará recuperar y revisar los trabajos previos de Hunter y Warrior antes de implementar nuevas rotaciones. No se dará por hecho que código antiguo es compatible hasta inspeccionarlo y probarlo.
