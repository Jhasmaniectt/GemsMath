# Gemas · Multijugador

Prototipo de juego educativo de valor posicional (unidades, decenas y centenas) para dos jugadores.
11 niveles: componer y descomponer, sumar y restar con reagrupación.

## Cómo jugar
1. Abre la página. Se crea una partida con un código (en el enlace: `?g=CÓDIGO`).
2. Pulsa **Copiar enlace** y envíaselo a tu compañero.
3. Cada uno elige **Jugador 1** (plano A) o **Jugador 2** (plano B).
4. Niveles 1 y 2: cada uno resuelve el mismo problema; el juego espera a que los dos abran su candado.
5. Niveles 3 a 11: el Jugador 1 tiene el primer número y el Jugador 2 el segundo.
   - Para enviar una gema o un grupo al compañero, arrástralo hasta el borde de arriba.
   - El candado es compartido: cualquiera de los dos puede girar los diales y abrirlo.
   - En la esquina se ve el plano del compañero (sin números).

## Técnica
- Un solo archivo `index.html`, sin servidor propio.
- Los dos navegadores se conectan directamente con WebRTC mediante [PeerJS](https://peerjs.com) (servidor gratuito de PeerJS para el emparejamiento).
- Algunas redes de colegios o empresas bloquean WebRTC; en ese caso se puede pasar a un servidor propio.
- Para pruebas locales: `?srv=host:puerto` usa un servidor PeerJS propio.
