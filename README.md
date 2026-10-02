# Interconsultas SMS

Cuadro de las interconsultas del Servicio Murciano de Salud. Dos ámbitos:

**Atención Primaria.** Matriz por especialidad y área sanitaria con cuatro modalidades por casilla: **CM** (cita mostrador, la vía analógica), **INP** (no presencial), **ITC** (presencial por gestor) e **ITCa** (ITC abierta). El relleno identifica la modalidad y el aspa el estado; la CM se tiñe según su uso en 2026. Una segunda vista, **Buzones INP**, cruza lo que ofrece la primaria con el buzón de cada hospital en Selene y con el destino que marca el COMPAS.

**Hospital.** Vista **ITC-R**, las interconsultas entre hospitales, con sus dos vías: la actual entre Selenes y la nueva por el Gestor de Peticiones, el hospital que atiende, la llamada telefónica obligatoria y la cita en destino.

Al pulsar una casilla se cambia su estado y se registra fecha, usuario y observaciones. Cada especialidad y cada prueba llevan su resumen, su ficha y su circuito dibujado.

## Estructura

- Rama `main`: `index.html`, la aplicación completa. No necesita servidor.
- Rama `datos`: `estado.json`, el estado compartido (cambios, fechas, notas y reclasificaciones), cifrado con la contraseña de acceso.

## Publicar cambios para todo el equipo

La página guarda siempre en el navegador de cada persona. Para publicar hace falta un token de GitHub de grano fino con acceso solo a este repositorio y permiso `Contents: Read and write`. Se introduce una vez en la propia página, que lo guarda cifrado en ese navegador y nunca lo publica.

Publicado con GitHub Pages: https://idoctor2000.github.io/mapa-itc-inp/
