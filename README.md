# Hundir la flota

Juego de **Hundir la flota** hecho en Python con NumPy. Se juega contra la máquina, que dispara de forma aleatoria.

![Foto Hundir la Flota](istockphoto-1337405629-612x612.jpg)
## Reglas

- Cada jugador tiene dos tableros: uno con sus barcos y otro donde anota sus disparos.
- Cada jugador coloca 6 barcos: 3 de tamaño 2, 2 de tamaño 3 y 1 de tamaño 4.
- Los barcos no pueden salirse del tablero ni solaparse.
- Si aciertas, repites turno. Si fallas, dispara el otro.
- Gana quien hunde antes todos los barcos del rival.

## Símbolos

| Símbolo | Significado |
|---------|-------------|
| `O` | Barco |
| `X` | Tocado |
| `-` | Agua |
| ` ` | Casilla vacía |

## Cómo jugar

1. Instala lo necesario: `pip install numpy notebook`
2. Abre el notebook y ejecuta las celdas en orden.
3. El tamaño del tablero será 10 automaticamente.
4. Coloca tus barcos indicando fila, columna y orientación (N, S, E, O).
5. Dispara escribiendo fila y columna (empiezan en 0). Escribe `salir` para terminar.

## Funciones principales

- `crea_tablero`: crea un tablero vacío.
- `coloca_barco_plus`: coloca un barco si cabe y no se solapa.
- `crea_barco_aleatorio` y `crea_barco_jugador`: colocan un barco al azar o a mano.
- `recibir_disparo`: procesa un disparo (tocado, agua o repetido).
- `turnos`: bucle principal de la partida.
