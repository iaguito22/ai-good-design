---
name: good-design
description: >-
  Suelo de calidad para cualquier web: lo que delata que una pagina la ha hecho
  una IA y lo que la IA siempre se salta (accesibilidad, semantica, meta,
  rendimiento, movil, estados, seguridad, modales, i18n, tipografia moderna,
  tarjetas y bloques de producto). Usala SIEMPRE que construyas o retoques una
  landing, un portfolio, un panel, una tienda o cualquier interfaz que una
  persona vaya a mirar. Tambien cuando el usuario diga "parece hecho con IA",
  "parece vibecoded", "es generico", "es slop" o "no me gusta como queda".
---

# Suelo de calidad: lo que la IA siempre se salta

Una web hecha por IA se reconoce a tres metros: colores genericos, degradados
morados/azules difuminados ("AI slop"), modales rotos en movil, texto que baila
al cargar fuentes, modales sin escape, formularios sin estados de carga, y
tarjetas de producto con fotos gigantescas y datos ocultos en hover.

Esta skill fija el **minimo no negociable** para cualquier pagina. No es para
hacer cosas complejas: es para que lo basico este bien hecho a la primera.

## 1. El test delator: lo que NO debes hacer NUNCA

- **NO metas bloques de "beneficios / garantias" genericos, tarjetas de caracteristicas en cajas ("3-card feature grid") ni triadas de metricas flotantes ("3 vanity stats")**: Bloques de 3 números con etiqueta debajo ("24mm / ±0.5dB / 10 años", "99% satisfacción / 24/7 / 10k clientes") puestos en el hero o centro de la página son el cliché clásico de IA. Los datos reales van en la ficha de especificaciones, en la tabla técnica o dentro del texto explicativo.
- **NO uses sombras gigantescas desenfocadas**: `box-shadow: 0 20px 60px rgba(0,0,0,0.3)`
  hace que todo flote sin gravedad. Sombras cortas y definidas (ej. `0 2px 8px rgba(0,0,0,0.06)`).
- **NO ocultes informacion critica en hover**: Los precios, botones de compra y tallas
  deben ser visibles y clicables en movil sin necesidad de pasar el raton por encima.
- **NO uses imagenes con rectangulos grises descompensados**: Si usas graficos vectoriales,
  que tengan escala y proporcion coherentes con el texto que los rodea.

## 2. Tipografía y lectura

- `text-wrap: balance` en todos los titulares (`h1`, `h2`, `h3`) para evitar lineas viudas.
- `text-wrap: pretty` en los parrafos de cuerpo para evitar palabras huerfanas al final.
- Medida de linea de 60-75 caracteres (`max-width: 65ch`) e interlineado 1.5 en parrafos.
- `font-variant-numeric: tabular-nums` en precios, contadores, fechas y tablas para evitar bailes.

## 3. Dispositivos móviles y ergonomía

- `100dvh` en lugar de `100vh` para evitar que la barra de direcciones de Safari/Chrome movil tape contenido.
- `env(safe-area-inset-bottom)` en barras fijas y botones inferiores (soporte iPhone notch y barra home).
- Tap targets de 44x44px minimo en botones, iconos y elementos tactiles interactivos.

## 4. Modales y overlays

- Cierre con tecla `Escape`.
- `focus trap`: el foco no debe escapar del modal abierto al pulsar Tabulador.
- `overscroll-behavior: contain` en el contenedor del modal para evitar scroll involuntario del fondo.

## 5. Accesibilidad y contraste

- Contraste minimo 4.5:1 en cuerpo y 3:1 en texto grande.
- Soporte nativo para modo claro y oscuro con transiciones suaves en variables CSS.
