# Ruleta Slash

Ruleta rompehielos para las reuniones online del equipo de Slash. Tiene categorías de preguntas, desafíos con temporizador, una casilla grupal, comodines al azar (1 por turno), puntos de regalo (4 por persona, máximo 1 por turno), marcador y podio.

## Páginas

- `index.html`: vista del moderador, la que se comparte en pantalla durante la videollamada.
- `jugar.html`: abre la vista de jugador (`index.html#jugar`).

## Cómo funciona aquí y en Claude

El modo multijugador (unirse con el link, girar desde el propio dispositivo y regalar puntos) usa el almacenamiento compartido de los Artifacts de Claude. Por eso:

- **En Claude** funciona todo: https://claude.ai/artifact/ByGb4w8QU43T9dy2DeXjSC (moderador) y https://claude.ai/artifact/ByGb4w8QU43T9dy2DeXjSC#jugar (jugadores). Cada jugador necesita acceso como Colaborador.
- **En GitHub Pages** solo funciona la vista del moderador, en modo local: quien modera gira por todos, marca los resultados y maneja el marcador desde su pantalla. La vista de jugador no se puede conectar al juego.

## Uso en modo local

1. Abre `index.html` y comparte la pestaña en la videollamada.
2. Gira con el botón central o con la barra espaciadora.
3. Marca si la persona respondió o logró el desafío; el turno pasa solo al siguiente.
4. Usa **Reiniciar** para empezar una partida nueva y **Ver podio** para cerrar el juego.
