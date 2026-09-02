# Mapa ITC · INP · Atención Primaria (SMS)

Matriz interactiva de interconsultas de Atención Primaria por especialidad y área sanitaria del Servicio Murciano de Salud.

Cada casilla muestra tres cuadrados, uno por modalidad:

| Modalidad | Borde | Significado |
|---|---|---|
| **INP** | azul | Interconsulta no presencial (INPAP) |
| **ITC** | verde | Interconsulta presencial gestionada |
| **INPc** | morado | INP Citable, también llamada ITC abierta |

Relleno verde = abierta. Rojo con aspa = cerrada. Al pulsar un cuadrado se abre o cierra la modalidad y se registra fecha, usuario y observaciones.

## Estructura

- Rama `main`: `index.html`, la aplicación completa. No necesita servidor.
- Rama `datos`: `estado.json`, el estado compartido (cambios, fechas y reclasificaciones), cifrado con la contraseña de acceso.

## Publicar cambios para todo el equipo

La página guarda siempre en el navegador de cada persona. Para publicar hace falta un token de GitHub de grano fino con acceso solo a este repositorio y permiso `Contents: Read and write`. Se introduce una vez en la propia página, que lo guarda cifrado en ese navegador y nunca lo publica.

Publicado con GitHub Pages: https://idoctor2000.github.io/mapa-itc-inp/
