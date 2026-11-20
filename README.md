# Ruleta Slash

Ruleta rompehielos para las reuniones online del equipo de Slash. Tiene categorías de preguntas, desafíos con temporizador, una casilla grupal, comodines al azar (1 por turno), puntos de regalo (4 por persona, máximo 1 por turno), marcador y podio.

## Páginas

- `index.html`: vista del moderador, la que se comparte en pantalla durante la videollamada.
- `jugar.html`: abre la vista de jugador (`index.html#jugar`).

## Cómo funciona aquí y en Claude

El modo multijugador (unirse con el link, girar desde el propio dispositivo y regalar puntos) usa el almacenamiento compartido de los Artifacts de Claude. Por eso:

- **En Claude** funciona todo: https://claude.ai/artifact/ByGb4w8QU43T9dy2DeXjSC (moderador) y https://claude.ai/artifact/ByGb4w8QU43T9dy2DeXjSC#jugar (jugadores). Cada jugador necesita acceso como Colaborador.
- **En GitHub Pages** los jugadores se conectan directo al navegador del moderador con [PeerJS](https://peerjs.com/), usando un código de sala de 4 caracteres. No necesitan cuenta.

## Cómo jugar en GitHub Pages

1. Quien modera abre `index.html` y comparte la pestaña en la videollamada. Arriba aparece el código de sala.
2. Con **Link para jugadores** copia el link (`jugar.html?sala=CÓDIGO`) y lo envía al equipo.
3. Cada jugador abre el link, escribe su nombre y entra. Si su nombre coincide con uno del marcador, ocupa ese lugar.
4. La pestaña del moderador debe quedar abierta todo el juego: es la que conecta a todos. Si se recarga, los jugadores se reconectan solos.
5. Si alguien no puede entrar, quien modera opera su turno desde su pantalla.

La conexión directa puede fallar en redes muy restringidas (algunas VPN o redes corporativas). En ese caso, esa persona juega a través del moderador.
