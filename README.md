# Testing Iconos SVG
### https://lifeomic.github.io/chromicons.com/

pruebas cómo usar iconos SVG definidos en una zona del HTMl y usados en otra, para un mayor orden del código.

- Se le pone un ID a cada icono
- Con CSS se modifica el fill y stroke
- Los SVG llevan parámetros que definen el objeto y son importantes

```
width="24" 
height="24"
stroke="currentColor"
fill="none"
stroke-linecap="round"
stroke-linejoin="round"
stroke-width="2"
viewBox="0 0 24 24"
data-icon="SvgAnchor"
aria-hidden="true"

```

## Propiedades de SVG
```width="24" y height="24"```

- Descripción: Especifican el ancho y alto del área en la que se mostrará el SVG. Estos valores se definen en unidades CSS, por lo general en píxeles (px).
- Uso: Determina las dimensiones finales del SVG en la página, afectando su tamaño visual.

```stroke="currentColor"```

- Descripción: Define el color de la línea (trazo) del SVG. Usando currentColor, el SVG hereda el color actual del texto o el color definido por el CSS del elemento contenedor.
- Uso: Facilita la integración del SVG en diseños responsivos al heredar el color de su entorno.
```fill="none"```

- Descripción: Establece que el interior de las formas en el SVG no se rellene con color (es transparente).
- Uso: Útil para íconos o gráficos que solo deben mostrar líneas o bordes sin relleno.
```stroke-linecap="round"```

- Descripción: Especifica la forma de los extremos de las líneas (trazos) en el SVG. round redondea los extremos de las líneas.
- Opciones: butt (plano, por defecto), round (redondeado), square (extiende la línea más allá de su extremo).
- Uso: Mejora la apariencia de los extremos de las líneas en gráficos donde se desea un acabado suave.
```stroke-linejoin="round"```

- Descripción: Define la forma de las uniones entre segmentos de línea en el SVG. round redondea las esquinas de las uniones.
- Opciones: miter (esquinas puntiagudas, por defecto), round (redondeado), bevel (biselado).
- Uso: Asegura que las uniones de líneas tengan un acabado suave en esquinas y uniones.
```stroke-width="2"```

- Descripción: Establece el grosor de las líneas (trazos) en el SVG. El valor 2 representa el grosor en unidades CSS (normalmente píxeles).
- Uso: Define la anchura de las líneas, lo que puede afectar la visibilidad y el estilo del SVG.
```viewBox="0 0 24 24"```

- Descripción: Define el área visible del SVG y establece la relación entre el sistema de coordenadas del SVG y su tamaño en pantalla. Los valores 0 0 24 24 indican que el área visible empieza en (0,0) y se extiende a 24 unidades de ancho y alto.
- Uso: Permite que el SVG se escale correctamente al mantener la proporción de su contenido, independientemente del tamaño especificado por width y height.
```data-icon="SvgAnchor"```

- Descripción: Es un atributo personalizado (no estándar) utilizado para almacenar información adicional sobre el SVG. En este caso, podría estar indicando un identificador o tipo de ícono (por ejemplo, SvgAnchor).
- Uso: Útil para fines de desarrollo, como identificación, selección en scripts o estilos, sin afectar la visualización del SVG.
```aria-hidden="true"```

- Descripción: Indica que el SVG es decorativo y no debería ser anunciado por tecnologías de asistencia, como lectores de pantalla.
- Uso: Mejora la accesibilidad al ocultar elementos decorativos del flujo de navegación asistido, evitando información redundante para usuarios de tecnologías de asistencia.