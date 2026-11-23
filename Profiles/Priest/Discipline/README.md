# Sacerdote – Disciplina (leveo 1–80)

**Estado:** base inicial generada; pendiente de auditoría y pruebas en WoW 3.3.5a.

Archivos: `PRIEST_Abilities.xml` y `PRIEST_Rotations.xml`.

- PQR con estructura DarhangeR.
- Omite hechizos no aprendidos según el libro esES.
- CTRL izquierdo: pausa/reanuda.
- SHIFT: habilita las habilidades AoE listadas.
- Perfil de sanación: requiere seleccionar manualmente un aliado; no automatiza selección de grupo ni prioridades por porcentaje de vida.


## Prioridad inicial
1. Penitencia
2. Palabra de poder: escudo
3. Rezo de alivio
4. Sanación relámpago
5. Sanación superior


**Advertencia:** las prioridades son un punto de partida, no una rotación optimizada. Revisar traducciones, requisitos de talentos, recursos, armas, formas, rango y APIs del ejecutor. No usar como validado hasta probarlo en cliente 3.3.5a.


## Actualización: sanación inteligente

# Sacerdote Disciplina – leveo 1–80

**Estado:** base de sanación inteligente añadida; pendiente de pruebas reales en WoW 3.3.5a.

- Recorre automáticamente miembros de raid o grupo (y al jugador).
- Prioriza al aliado con menor porcentaje de vida dentro de rango.
- No requiere cambiar el target manualmente.
- CTRL izquierdo pausa/reanuda.


**Sanación inteligente de grupo/banda:** el perfil busca automáticamente aliados vivos y conectados en el grupo, evalúa su porcentaje de vida y lanza la curación elegida sin cambiar manualmente el objetivo. El tanque debe estar configurado como foco para la Señal de la Luz (Paladín). Los umbrales son valores iniciales y requieren calibración. La selección automática, el casteo por unidad y el comportamiento en PQR deben verificarse en el cliente 3.3.5a; no está validado todavía.

## Hechizos configurados
- Penitencia: umbral inicial 65%
- Sanación relámpago: umbral inicial 60%
- Sanación superior: umbral inicial 82%
