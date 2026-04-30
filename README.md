# PARASITE RUN

**PARASITE RUN** es un prototipo web 2D estilo indie oscuro, biopunk y pixel-art, ambientado en un laboratorio abandonado. El jugador controla un parasito experimental que no puede sobrevivir mucho tiempo sin cuerpo y debe infectar distintos huespedes para escapar.

## Estado

Build V1.6 / Bloque A.

## Jugar

Abre `index.html` en el navegador o sirve el proyecto con un servidor local:

```bash
python3 -m http.server 5173
```

Luego entra a:

```text
http://127.0.0.1:5173/
```

## Controles

- `A / D` o flechas: moverse
- `W` o flecha arriba: saltar
- `E`: infectar huesped cercano o activar panel
- `Shift`: habilidad especial
- `Q`: abandonar cuerpo actual
- `R`: reiniciar nivel
- `Esc`: pausar

## Concepto

El jugador no es un humano. Es un parasito experimental que escapó de una capsula rota. Fuera de un cuerpo pierde vida parasitaria rapidamente, asi que debe tomar control de enemigos y usar sus habilidades antes de que el huesped se deteriore.

## Loop principal

1. Empiezas como parasito debil.
2. Buscas un huesped infectable.
3. Infectas guardias, perros mutados o robots.
4. Cada cuerpo cambia la forma de jugar.
5. La estabilidad del cuerpo baja con el tiempo.
6. Cambias de huesped antes de colapsar.
7. Escapas por la salida de contencion.

## Huespedes

### Parasito

- Pequeno, rapido y fragil.
- Vida parasitaria limitada.
- Dash corto para infectar.
- Animacion nerviosa, organica y viscosa.

### Guardia

- Movimiento equilibrado.
- Puede disparar con `Shift`.
- Puede activar paneles de seguridad con `E`.
- Visor azul y silueta humana clara.

### Perro mutado

- Muy rapido.
- Salto largo.
- Puede pasar por tuneles bajos.
- Estetica verde toxica, baja y agresiva.

### Robot pesado

- Lento y resistente.
- Salto corto.
- Puede romper paredes fragiles con `Shift`.
- Silueta cuadrada con luces rojas.

## Primer nivel: Bloque A - Despertar

El primer nivel funciona como tutorial jugable dentro de una fuga real de laboratorio. El jugador despierta en una capsula rota y avanza por secciones que ensenan las mecanicas sin pausar la accion:

- movimiento y salto,
- infeccion,
- estabilidad y deterioro,
- paneles de seguridad,
- Bioalerta por camaras y drones,
- cambio de cuerpo,
- tuneles bajos,
- saltos largos,
- torre laser con aviso previo,
- muro rompible,
- alarma final con drones activos,
- teaser del Cazador de Contencion,
- charcos toxicos y lasers,
- puerta final y victoria.

## Caracteristicas actuales

- Juego completo en un solo `index.html`.
- Sin assets externos pesados.
- Canvas 2D puro.
- Menu principal con seccion `Jugar Tutorial`.
- Espacio preparado para futura tienda.
- Sistema de infeccion.
- Tres huespedes infectables.
- Barra de estabilidad / vida parasitaria.
- Tutorial paso a paso.
- Obstaculos y peligros.
- Sistema de Bioalerta por vigilancia.
- Camaras fijas y drones con cono visible.
- Torre laser con fase de carga y disparo.
- Mini escape final al romper el muro industrial.
- Victoria, muerte y reinicio.
- Efectos de particulas.
- Screen shake e hit-stop sutil.
- Sonidos simples con Web Audio API.
- Sprites generados por codigo con contornos, rim light y animaciones.
- Compatible con Netlify como sitio estatico.

## Estilo visual

La direccion artistica mezcla:

- laboratorio biopunk,
- pixel-art oscuro,
- indie atmosferico,
- luces frias,
- sangre/neon biologico,
- particulas tipo spray,
- claridad visual inspirada en juegos sandbox de cuerpos/objetos con fisicas.

No usa assets oficiales ni copiados de otros juegos.

## Tecnologia

- HTML
- CSS
- JavaScript
- Canvas 2D
- Web Audio API

## Deploy en Netlify

Este proyecto se puede subir directamente como sitio estatico. El archivo principal es:

```text
index.html
```

No requiere build step.

## Roadmap

- Tienda/cosmeticos.
- Mas niveles.
- Nuevos huespedes.
- Mas peligros.
- Mejor sistema de checkpoints.
- Version mobile/touch.
- Musica y sonido mas completos.
- Guardado de progreso.
