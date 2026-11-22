# 14 · Plan de prueba: qué anuncio y qué web venden más

*15 nov 2026. Decidido con Mariana. Corre del 19 nov al 5 dic, incluida Black Week.*

## Qué queremos saber
1. **Formato:** ¿vende más la foto, el video real o el video hecho con IA?
2. **Web:** ¿vende más la ficha de producto actual (A) o una página de un solo producto (B)?
3. **Producto:** ¿qué pieza responde mejor a los anuncios: Delta, Astro o Limo?

Lo que gane se usa para la temporada de Navidad, con pedidos hasta el 5 de diciembre.

## Lo decidido
| Tema | Decisión |
|---|---|
| Presupuesto | Hasta **$100.000 al día** |
| Productos | **Limo** ($350.000, el que más presupuesto lleva), **Delta** ($200.000), **Astro** ($200.000) |
| Formatos | Foto · video real · video con IA. Los 3 llevan a comprar en la web |
| Prueba de la web | **La web reparte sola:** todos los anuncios llevan al mismo enlace y la web le muestra la A a la mitad de las personas y la B a la otra mitad. Cada persona ve siempre la misma versión |
| Web B | Página de un solo producto, sin menú, con un solo botón de comprar |
| Precio del Delta | **$200.000 en todo**: anuncio, web y WhatsApp |
| Calendario | Montamos todo del 16 al 18, lanzamos el 19 y seguimos en Black Week (20 al 30) |

## Cómo se arma en Meta
**Una campaña nueva de Ventas:** «MIR | Ventas | Prueba formatos | Nov 2026». La campaña Delta-Astro actual se apaga el día que arranca esta.

**9 conjuntos de anuncios**, uno por producto y formato. Cada formato tiene su propio presupuesto, así Meta no le da todo al que arranque mejor el primer día y la comparación es justa.

| Producto | Foto | Video real | Video IA | Total al día |
|---|---|---|---|---|
| Limo | $13.000 | $13.000 | $13.000 | $39.000 |
| Delta | $10.000 | $10.000 | $10.000 | $30.000 |
| Astro | $10.000 | $10.000 | $10.000 | $30.000 |
| | | | | **$99.000** |

- **Igual en los 9:** público (Colombia, mujeres, edad amplia y segmentación Advantage+), ubicaciones, horario y texto del anuncio por producto. **Lo único que cambia es la imagen o el video.** Si cambiamos más cosas, no sabremos qué hizo la diferencia.
- **Qué optimiza Meta:** «Agregar al carrito» y no «Ver contenido», que trae gente que mira y no compra. Para optimizar por «Compra», Meta necesita unas 50 compras a la semana; cuando pasemos de 15 o 20, lo cambiamos.
- **No editar los anuncios una vez arrancan.** Cada edición hace que Meta vuelva a aprender y la comparación se daña. Si algo está mal, se apaga y se crea otro.
- **Etiquetas del enlace** para saber de qué anuncio vino cada visita y cada pedido:
  `utm_source=meta&utm_medium=paid&utm_campaign=prueba-nov26&utm_content=<producto>-<formato>`
  Ejemplo: `utm_content=delta-video-ia`. Formatos: `foto`, `video-real`, `video-ia`.

## Las dos webs
- **A · la de hoy:** la ficha de producto normal, con menú, galería y el resto de la tienda.
- **B · página de un solo producto.** De arriba hacia abajo:
  1. Foto o video de la joya **puesta**, con el precio y el botón de comprar a la vista sin bajar.
  2. Color y talla ahí mismo. Para la talla, «cómo medirla con un hilo» con dibujos, y la opción de «no sé mi talla».
  3. Por qué confiar: hecha a mano en plata 925, pago seguro con Bold, garantía de 3 meses y 5 días para devolverla.
  4. **Prueba de clientas:** fotos o mensajes reales. *(Necesito tu material.)*
  5. Entrega: de 10 a 15 días; si pides antes del 5 de diciembre, llega antes de Navidad.
  6. Preguntas frecuentes cortas y WhatsApp.
  7. Botón de comprar fijo abajo en el celular. **Sin menú ni salidas** hacia otras piezas, salvo el paño Cauce como complemento.
- Mismos colores y tipografía de la marca. Si además cambiamos el look, no sabríamos si ganó la estructura o los colores. El look se prueba después, en otra ronda.
- **Cómo se reparte:** con PostHog. Cada persona queda en A o en B la primera vez que entra, y eso queda guardado en sus eventos y en su pedido. En el admin, cada pedido dice qué web vio.

## Qué medimos y cuándo decidimos
| Paso | Métrica | Para qué |
|---|---|---|
| El anuncio | Costo por cada 1.000 vistas · % de clics · costo por visita | ¿El formato llama la atención? |
| La web | % que agrega al carrito · % que va a pagar | ¿La página convence? |
| La venta | Ventas · costo por venta · valor promedio | La respuesta final |

**Reglas para decidir.** Se escriben antes de arrancar para no decidir por corazonadas:
- **Apagar un formato** cuando lleve $40.000 gastados y su costo por visita sea el doble del promedio del producto, o no tenga ningún carrito.
- **Leer los formatos el 25 de nov.** El presupuesto de los perdedores pasa al ganador de cada producto. El resto de Black Week se queda en 1 o 2 formatos por producto.
- **Leer la web el 1 de dic.** Gana la versión que tenga claramente más «agregar al carrito» y más pagos por visita. Si la diferencia es pequeña, lo decimos tal cual: la prueba no definió, y seguimos con la más simple.
- **Ventas:** con pocas ventas, una venta suelta no decide nada. Las ventas confirman lo que digan los clics y los carritos.

## Black Week dentro de la prueba
- Del 20 al 30 de noviembre, los mismos 9 anuncios con su versión Black: precio tachado y el mismo descuento en las dos webs. El porcentaje no se anuncia antes del 20.
- El precio tachado es el precio real de antes: Delta $200.000, Astro $200.000 y Limo $350.000.
- El 1 de diciembre vuelve el precio lleno con «Regálatelo» y el corte del 5 de diciembre para que llegue en Navidad.

## Calendario
| Día | Qué | Quién |
|---|---|---|
| 16 nov | Delta a $200.000 en la web | Lolita |
| 16 nov | Cambiar el precio en el anuncio actual del Delta | Mariana |
| 16–17 nov | Mandar fotos, videos y pruebas de clientas de Delta, Astro y Limo | Mariana |
| 16–18 nov | Montar la web B y el reparto 50/50 | Lolita |
| 17–18 nov | Hacer las fotos de anuncio, editar los videos reales y generar los videos con IA | Lolita |
| 18 nov | Revisar y aprobar los 9 anuncios y la web B | Mariana |
| 19 nov | Crear la campaña en Meta, siguiendo una guía paso a paso que te doy | Mariana |
| 19 nov | Apagar la campaña Delta-Astro | Mariana |
| 20 nov | Versión Black de los anuncios y de las dos webs | Lolita + Mariana |
| 22 nov | Primera lectura: ¿algún formato para apagar? | Lolita |
| 25 nov | Lectura de formatos y mover el presupuesto | Lolita propone, Mariana aprueba |
| 1 dic | Lectura de la web y plan de Navidad | Lolita |
| 6 dic | Informe final: qué formato, qué web y qué producto | Lolita |

## Lo que necesito de ti
1. **Material por producto** (Delta, Astro, Limo): las mejores fotos puestas, los videos que ya tengas y, si puedes, un video nuevo de cada uno puesto en la mano, con luz de día y de 10 a 20 segundos.
2. **Prueba de clientas:** fotos que te hayan mandado, capturas de mensajes o reseñas, con su permiso.
3. **Descuento de Black Week:** el porcentaje o el precio final de cada pieza. Lo necesito antes del 19 para preparar los anuncios.

## Riesgos a cuidar
- **Astro no ha vendido nunca.** Entra en la prueba, pero si el 25 sigue sin carritos, su presupuesto pasa al Delta.
- **Black Week cambia el comportamiento**: la gente compra más por el descuento. Por eso las dos webs y los tres formatos tienen el mismo descuento, y la comparación entre ellos sigue siendo justa.
- **Poca gente.** Con $100.000 al día llegan unas 200 a 300 visitas diarias. Alcanza para comparar formatos. Para la web puede que solo veamos diferencias grandes.
