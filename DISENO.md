# DISENO DEL JUEGO

## 1. Información general

**Género:** Juego multijugador 2D de laberinto.

**Plataforma:** Navegador web.

**Número de jugadores:** De 2 a 4 jugadores por partida.

**Tecnologías:**
- HTML, CSS y JavaScript.
- Canvas para dibujar el juego.
- Node.js y Express para el servidor.
- Socket.IO para la comunicación en tiempo real.

## 2. Idea principal

El juego consiste en un laberinto donde varios jugadores compiten para encontrar llaves y escapar antes que los demás.

Cada jugador tendrá un número, un color y una forma diferente para poder distinguirlo fácilmente.

Durante la partida tendrán que explorar el laberinto, evitar trampas, utilizar potenciadores y tener cuidado con los enemigos.

## 3. Objetivo del juego

El objetivo es conseguir 3 llaves y llegar a la salida del laberinto.

Habrá 8 llaves repartidas por el mapa y la salida estará situada en el centro.

El primer jugador que consiga las 3 llaves y llegue a la salida será el ganador.

La partida tendrá un límite de 5 minutos. Si nadie consigue escapar, ganará el jugador que tenga más llaves.

## 4. Cómo funciona una partida

1. Un jugador crea una sala y recibe un código.
2. Los demás jugadores entran utilizando ese código.
3. Todos esperan en una sala de espera hasta que el anfitrión comienza la partida.
4. Se genera un laberinto aleatorio y cada jugador aparece en una zona diferente.
5. Los jugadores empiezan a buscar las llaves y a evitar los peligros.
6. El primero que consigue 3 llaves y llega a la salida gana.
7. El servidor anuncia el resultado a todos los jugadores.

## 5. Elementos del juego

### Trampas

**Pinchos:** Aparecen y desaparecen. Si un jugador los pisa, queda inmovilizado durante 2 segundos.

**Barro:** Reduce la velocidad del jugador a la mitad mientras está encima.

### Potenciadores

**Botas rápidas:** Aumentan la velocidad durante 5 segundos.

**Escudo:** Protege al jugador de las trampas y los guardianes durante 5 segundos.

**Brújula:** Muestra una flecha hacia la llave más cercana. Si el jugador ya tiene 3 llaves, señala la salida. Dura 8 segundos.

### Enemigos

**Guardianes:** Son enemigos que patrullan por los pasillos del laberinto.

Si un guardián toca a un jugador, este pierde una llave. La llave cae al suelo y otro jugador puede recogerla. Después, el jugador vuelve a aparecer en un lugar cercano.

## 6. Reglas de la partida

- Cada jugador necesita 3 llaves para poder escapar.
- Las llaves pueden ser recogidas por cualquier jugador.
- Si un jugador pierde una llave por culpa de un guardián, otro puede recogerla.
- Si un jugador se desconecta, sus llaves caen al suelo.
- Si solo queda un jugador conectado, gana automáticamente.
- La partida termina cuando alguien escapa o cuando se acaba el tiempo.

## 7. Orden de desarrollo

Para no complicar demasiado el proyecto, se desarrollará por etapas:

1. Crear el laberinto y permitir el movimiento de los jugadores.
2. Añadir las llaves, la salida y el sistema para determinar al ganador.
3. Crear las salas, el código de acceso y la sala de espera.
4. Añadir las trampas.
5. Añadir los potenciadores.
6. Añadir los guardianes.
7. Mejorar el diseño, la accesibilidad y probar el juego con varios jugadores.
8. Terminar la documentación y preparar la presentación.

## 8. Objetivo final del proyecto

Crear un juego multijugador 2D divertido, sencillo de utilizar y que funcione correctamente desde el navegador.

El desarrollo se hará poco a poco, comprobando cada parte antes de añadir nuevas funciones.