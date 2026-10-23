# Misión Marte

> Juego de consola en C++ donde aterrizas una nave en Marte esquivando meteoritos y luego manejas un rover para recolectar cristales. Incluye modo manual, modo automático y una simulación controlada por la computadora.

## Sobre el proyecto

**Misión Marte** es un juego de arcade en consola, hecho en una **game jam**. Tiene dos niveles: primero hay que descender hasta la superficie de Marte sin que los meteoritos destruyan la nave, y luego un pequeño rover debe recolectar todos los cristales y volver a la nave.

## Cómo se juega

### Menú principal

| Opción | Acción |
|---|---|
| `1` | Jugar (jugar tú o ver la simulación) |
| `2` | Instrucciones |
| `3` | Créditos |
| `4` | Salir |

### Nivel 1: aterrizaje

- Desciendes desde **700 km** de altura y tienes **5 vidas**.
- Esquiva los meteoritos que cruzan la pantalla. Cada choque te quita una vida.
- Cuando te acercas a la superficie aparece el mensaje *"Hora de aterrizar!"*. Al tocar el suelo ganas el nivel.
- Un panel muestra estado, altura, número de meteoritos, tiempo aproximado de llegada y nombre del operador.

### Nivel 2: rover

- El rover empieza junto a la nave. Recoge los **5 cristales** repartidos por el mapa.
- Hay **14 meteoritos** fijos en el terreno; chocar con ellos te quita una vida.
- Cuando tengas todos los cristales, regresa a la nave para terminar la misión.

### Controles

| Tecla | Acción |
|---|---|
| ← ↑ → ↓ | Mover nave / rover |
| `A` | Activar o desactivar el **modo automático** (nivel 1): la nave sigue moviéndose en la última dirección elegida |

### Modos de juego

- **Jugar juego:** escribes tu nombre y controlas la misión.
- **Ver simulación:** la computadora (operador "NASA") juega sola y esquiva los meteoritos en el nivel 1.

## Características

- Dos niveles con mecánicas distintas.
- Gráficos en consola con caracteres ASCII extendidos (cielo, suelo, sol, nave, rover, meteoritos y cristales de colores).
- Fondo de estrellas aleatorio y arte ASCII del sistema solar en la intro y la despedida.
- Texto que aparece letra por letra.
- Modo manual, automático y simulación.

## Requisitos

- Windows
- Visual Studio con soporte de **C++/CLI** (usa `System::Console` y `pch.h`). Se crea como proyecto *CLR Console App*. TODO: indicar versión de Visual Studio / .NET Framework.
- Consola de al menos **120 × 30** caracteres. El programa ajusta el tamaño al iniciar.
- Recomendado: `cmd.exe` o la consola clásica de Windows. TODO: confirmar que se ve bien en Windows Terminal.

## Cómo ejecutarlo

1. Abre la solución en Visual Studio.
2. Compila en modo **Release** (o Debug).
3. Ejecuta el `.exe` y deja que la ventana se ajuste a 120 × 30.

## Estructura

```
.
├── main.cpp        # TODO: ajustar al nombre real del archivo
├── pch.h
└── README.md
```
