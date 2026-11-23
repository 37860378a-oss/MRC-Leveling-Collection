# Paladín – Sagrado (leveo 1–80)

**Estado:** prototipo de sanación automática implementado en GitHub; pendiente de pruebas reales en WoW 3.3.5a con PQR.

## Funcionamiento
- El motor recorre automáticamente al jugador y los miembros de grupo o banda.
- Selecciona al aliado vivo con menor porcentaje de vida que esté dentro de rango.
- Guarda la unidad elegida en `PQR_CustomTarget` y su vida en `PQR_CustomTargetHP`, siguiendo el mecanismo del perfil DarhangeR.
- Lanza las curas sobre esa unidad sin exigir que el jugador la seleccione manualmente.
- Si hay un tanque válido en `focus`, intenta mantener Señal de la Luz y Escudo Sagrado cuando esos hechizos estén aprendidos y disponibles.
- CTRL izquierdo pausa/reanuda.

## Hechizos de curación
Se usan los identificadores de hechizos de la versión 3.3.5a para obtener el nombre localizado y lanzar el rango más alto aprendido:
- Choque Sagrado: umbral inicial 75%.
- Destello de Luz: umbral inicial 58%.
- Luz Sagrada: umbral inicial 88%.

Los umbrales son provisionales y necesitan calibración en combate real. Los hechizos no aprendidos o fuera de rango se omiten.

## Prueba pendiente
1. Entrar al juego con el perfil cargado en PQR.
2. Configurar el tanque como foco.
3. Agruparse con al menos otro jugador herido.
4. Iniciar la rotación y comprobar que mantiene los buffs en focus y cura al miembro herido sin cambiar el target manual.
5. Probar también sin grupo y en banda.

**Importante:** el código está actualizado, pero todavía no está validado en el cliente. La compatibilidad de `CastSpellByName(nombre, unidad)`, los nombres localizados y el comportamiento de `PQR_CustomTarget` deben confirmarse en juego.


## Objetivo enemigo y Sentencia de Luz
- Mantener un enemigo hostil en `target` durante el combate.
- La habilidad MRC revisa si ese enemigo tiene Sentencia de Luz (debuff 20185 aplicado por el jugador).
- Si falta, está en rango y el hechizo está disponible, lanza Sentencia de Luz sobre `target`.
- El motor de curación sigue usando `PQR_CustomTarget`, por lo que no necesita reemplazar el enemigo seleccionado para curar.
- El perfil no cambia automáticamente de enemigo: el jugador conserva el control del `target`.
