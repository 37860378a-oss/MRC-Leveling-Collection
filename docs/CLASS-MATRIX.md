# Matriz de perfiles MRC – WoW 3.3.5a

Estado inicial: **pendiente de desarrollo y pruebas**.

| Clase | Árbol | Carpeta prevista |
|---|---|---|
| Guerrero | Armas | profiles/Warrior/Arms |
| Guerrero | Furia | profiles/Warrior/Fury |
| Guerrero | Protección | profiles/Warrior/Protection |
| Paladín | Sagrado | profiles/Paladin/Holy |
| Paladín | Protección | profiles/Paladin/Protection |
| Paladín | Reprensión | profiles/Paladin/Retribution |
| Cazador | Bestias | profiles/Hunter/Beast-Mastery |
| Cazador | Puntería | profiles/Hunter/Marksmanship |
| Cazador | Supervivencia | profiles/Hunter/Survival |
| Pícaro | Asesinato | profiles/Rogue/Assassination |
| Pícaro | Combate | profiles/Rogue/Combat |
| Pícaro | Sutileza | profiles/Rogue/Subtlety |
| Sacerdote | Disciplina | profiles/Priest/Discipline |
| Sacerdote | Sagrado | profiles/Priest/Holy |
| Sacerdote | Sombras | profiles/Priest/Shadow |
| Caballero de la Muerte | Sangre | profiles/Death-Knight/Blood |
| Caballero de la Muerte | Escarcha | profiles/Death-Knight/Frost |
| Caballero de la Muerte | Profano | profiles/Death-Knight/Unholy |
| Chamán | Elemental | profiles/Shaman/Elemental |
| Chamán | Mejora | profiles/Shaman/Enhancement |
| Chamán | Restauración | profiles/Shaman/Restoration |
| Mago | Arcano | profiles/Mage/Arcane |
| Mago | Fuego | profiles/Mage/Fire |
| Mago | Escarcha | profiles/Mage/Frost |
| Brujo | Aflicción | profiles/Warlock/Affliction |
| Brujo | Demonología | profiles/Warlock/Demonology |
| Brujo | Destrucción | profiles/Warlock/Destruction |
| Druida | Equilibrio | profiles/Druid/Balance |
| Druida | Feral | profiles/Druid/Feral |
| Druida | Restauración | profiles/Druid/Restoration |

## Variantes de Feral

El perfil Feral podrá documentar dos estilos configurables: DPS y tanque. Son variantes del mismo árbol en WotLK, no árboles separados.


## Estado de implementación

Se creó una base inicial para las 30 especializaciones en `Profiles/`. Cada carpeta incluye los XML de habilidades y rotación y un README. **Estado global: pendiente de auditoría y pruebas en WoW 3.3.5a.** La creación de archivos no implica que las rotaciones estén optimizadas ni verificadas en el cliente. Hunter Bestias es una base heredada recuperada; el resto son bases iniciales generadas para revisión.
