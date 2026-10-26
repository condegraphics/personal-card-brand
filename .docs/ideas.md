# Personal Brand Bard — Especificación visual de referencia

## Referencia de ground truth

La URL de referencia es `https://tarjetas-visuales.randstad.com.ar/tarjeta/92dde839-04aa-4140-9d38-faf37fe84f66`. Esta demo reproduce su front como patrón visual: fondo azul marino a pantalla completa, tarjeta blanca de lectura, composición editorial asimétrica, fuente Graphik, datos de contacto en filas con iconos, bloque de acciones y recursos gráficos corporativos. Se reemplazará la identidad Randstad por la identidad demo Personal Brand Bard cuando el usuario entregue los datos reales.

## Alcance confirmado

El proyecto es una demo de presentación. Debe tomar los datos, imagen de perfil, iconos y recursos gráficos visibles en la URL original como contenido temporal. La interfaz se implementará solo con HTML y CSS moderno, sin JavaScript propio ni librerías de interacción. Las acciones que no pueden ejecutarse sin JavaScript se conservarán como enlaces HTML o botones visuales con destinos explícitos cuando corresponda.

## Dirección elegida: réplica editorial corporativa de tarjeta digital

### Design Movement

Contemporary Swiss corporate editorial design: composición modular, jerarquía tipográfica precisa, color institucional fuerte y geometría abstracta como sistema de marca.

### Core Principles

La lectura debe ser inmediata y lineal. La información se organiza en una tarjeta blanca de alto contraste sobre un campo azul marino. Los elementos gráficos no compiten con los datos. Cada acción debe tener una affordance clara y un estado de foco visible.

### Color Philosophy

El azul marino funciona como campo institucional y reduce el ruido visual. El blanco crea una superficie de lectura limpia. El azul vivo se reserva para enlaces, iconos activos y llamadas a la acción. El gris medio se usa en metadatos y labels para mantener jerarquía sin perder accesibilidad.

### Layout Paradigm

Una composición en dos columnas sobre desktop: perfil y datos en una tarjeta blanca a la izquierda, superficie gráfica y acciones a la derecha. En móvil se transforma en una sola columna, manteniendo la tarjeta como unidad de lectura y trasladando la imagen decorativa debajo de los datos.

### Signature Elements

1. Tarjeta blanca con esquinas suavemente redondeadas y sombra contenida.
2. Logotipo/wordmark de referencia en la cabecera y formas circulares abstractas como marco visual.
3. Filas de contacto con icono grande, label pequeño y valor legible.

### Interaction Philosophy

La demo no depende de JavaScript. Los enlaces reales responden de forma nativa a click y teclado. Los botones tienen transición breve de color, desplazamiento y escala al presionar. Los reveals de scroll son progresivos y no ocultan información si el navegador no soporta scroll-driven animations.

### Animation

Usar solo `opacity` y `transform`, con duraciones menores a 300 ms. Aplicar `animation-timeline: view()` dentro de `@supports` para revelar suavemente secciones mientras entran al viewport, con estado visible por defecto como fallback. Desactivar el movimiento no esencial con `prefers-reduced-motion: reduce`.

### Typography System

Usar Graphik desde el CDN público detectado en la referencia (`https://fonts.cdnfonts.com/css/graphik`) como fuente principal de la demo. La jerarquía conserva pesos 300 para valores, 400 para body, 500 para nombre y marca, y una escala fluida con `clamp()` para títulos. La fuente del sistema queda como fallback operativo.

### Brand Essence

Una tarjeta digital B2B para presentar una identidad profesional de estrategia, marketing y presencia digital con una experiencia breve, clara y accionable. Personalidad: precisa, confiable, contemporánea.

### Brand Voice

Los títulos son directos y profesionales. Las etiquetas son cortas. Los CTA describen la acción sin exageraciones. Ejemplos temporales: “Conectemos con claridad.” y “Ver perfil profesional”.

### Wordmark & Logo

Usar el nombre “Personal Brand Bard” como wordmark tipográfico de demo y un símbolo gráfico abstracto propio como marca auxiliar. No reutilizar el logo Randstad como identidad de la demo.

### Signature Brand Color

Azul institucional profundo `#0F1940`, inspirado en la superficie principal de la referencia y reservado para el fondo, cabecera y panel de acciones.

## Reglas por archivo

Todo archivo de página o estilo debe comenzar con un comentario que recuerde la dirección “réplica editorial corporativa de tarjeta digital” y la restricción “solo HTML/CSS, sin JavaScript propio”.
