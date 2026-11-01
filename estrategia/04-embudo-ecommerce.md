# Mar i Río — Embudo de e-commerce: de la pauta a la venta

> Versión del 2026-10-31. Frente: joyas como producto (la colección en la web).
> El embudo de talleres (Joyas Vivas) se arma después, con la misma lógica.
> Base: 03-propuesta-de-valor.md (clienta, tono, quién no es clienta).

## Lo que dicen los números de la tienda (análisis de la sesión de UI/UX, últimos 120 días)

- **Catálogo:** 13 joyas, 8 son anillos.
- **Ventas:** 18 pedidos pagados (~4,5 al mes), ticket promedio de **$304.000**.
- **Delta y Limo venden casi el 60%** (24 de unas 40 unidades). Son las piezas que encabezan la campaña.
- **Pedidos pendientes:** de los 5, la mayoría eran pedidos de prueba y se borraron. Quedan 2 reales del 26 de julio (por confirmar si pagaron). Desde ahora, los pedidos sin pagar pasan solos a "abandonados" en el admin.
- **Dominio de la tienda:** mar-i-rio.com.

## El diagnóstico de vendedor

La tienda funciona y las fotos son lindas, pero nadie llega, y quien llega no conoce la marca. Con $400.000 al mes de pauta (~$13.000 al día) no se puede hacer lo que hacen las marcas grandes, que mandan desconocidas directo a comprar. Meta necesita unas 50 compras por semana para aprender a buscar compradoras, y Mar i Río está lejos de eso.

**La estrategia:** usar la plata para que mucha gente correcta **vea** la marca barato, y concentrar la venta en quien ya mostró interés. Primero te ven, después te visitan y al final te compran.

## El embudo en 3 etapas

| Etapa | A quién | Qué ve | Objetivo en Meta | % de la pauta |
|---|---|---|---|---|
| **1. Descubrir** | Mujeres de 22 a 40, Medellín y ciudades principales, intereses de moda de autor, joyería, diseño y estilo | Reels cortos de la firma: lo derretido de cerca, en la mano, el proceso, *"wow, es muy raro"* | Reproducciones de video / interacción | 40% (~$160.000) |
| **2. Visitar** | Quien vio el 50% o más de un video, o interactuó con Instagram en los últimos 30 días | La pieza con su precio visible, en la mano, y un llamado claro: *"Hecha a tu talla"* | Visitas a la página de destino (a la ficha del producto, no al inicio) | 30% (~$120.000) |
| **3. Comprar** | Quien visitó una ficha o inició el pago en los últimos 14 días y no compró | Testimonios reales, "hecha a tu talla", cambio de talla gratis, fecha límite de diciembre | Ventas (compras) | 30% (~$120.000) |

## El producto que abre la puerta

- **Ahora:** **Delta y Limo**, las más vendidas, cada una con su anuncio y llevando a su propia ficha (por ejemplo `/producto/delta-ring`).
- **Cuando esté listo el lote:** el **anillo de entrada de $150.000**. Es la primera compra de menor riesgo para una desconocida, y después se le muestra la colección.
- **Un solo producto por anuncio.** Nunca "mira toda la colección".

## La oferta de diciembre (sin descuentos agresivos)

- **Mensaje:** *"Regálatelo."*
- **Urgencia real:** *"Pide antes del [fecha] y te llega antes del 24, hecha a tu talla."* La fecha sale de los tiempos de vaciado y acabado.
- **Incentivo, si hace falta:** envío gratis. No descuentos sobre el precio.

## Lo que la ficha de producto debe tener (para la sesión de UI/UX)

1. **Precio visible** arriba, junto a la foto.
2. **Foto en la mano** y un video corto, además de las fotos de estudio.
3. **"Hecha a tu talla"** con la guía para medirse ahí mismo.
4. **Tiempos claros:** *"La hacemos para ti; te llega en X días."*
5. **Cambio de talla gratis**, escrito cerca del botón de compra.
6. **Testimonios** con las palabras reales de las clientas.
7. **Botón de compra visible** sin tener que bajar, y pago con Bold.
8. **Botón de WhatsApp** para dudas, que no reemplaza el botón de compra.
9. **Píxel de Meta:** ✅ instalado en mar-i-rio.com (ID terminado en 4398). Registra ver página, ver producto, agregar al carrito, iniciar pago, compra, contacto por WhatsApp y registro del popup. **Falta:** la API de Conversiones (sin ella Meta pierde compras, sobre todo en iPhone) y el catálogo de productos para anuncios dinámicos. PostHog tampoco mide todavía: falta su clave en Vercel.
10. **Barra fija abajo en celular** con precio y botón "elegir talla / agregar". Hoy el botón queda a unos 3 pantallazos. Es el cambio que más mueve la conversión.
11. **Etiqueta "la más vendida"** en Delta y Limo, y colecciones ordenadas por más vendidas.
12. **Popup del 10% apagado para quien llega de la campaña,** para que no choque con la oferta del anuncio ni enseñe a esperar descuento.

## Reglas del tráfico

- **Anuncio de una pieza →** la ficha de esa pieza.
- **Carrusel de anillos →** colecciones filtradas (`/colecciones?categoria=anillos`).
- **Retargeting →** la ficha exacta que vio (con el catálogo de Meta).
- **Marca o historia →** el inicio. **Nunca la campaña de ventas al inicio.**
- **Todos los enlaces con UTM,** por ejemplo `?utm_source=meta&utm_campaign=navidad&utm_content=delta-video`, para saber qué anuncio vende.

## Recuperar los pedidos pendientes

El admin ya tiene el filtro "Abandonados", con nombre, teléfono y pieza. Mariana les escribe por WhatsApp al día siguiente. Más adelante, un correo automático a la hora.

## Tráfico gratis que se suma

- Link en la bio de Instagram directo a la pieza del momento, no al inicio.
- Historias con sticker de enlace cada vez que se publique una pieza.
- Mensaje directo a la lista cercana (familia, amigas, clientas anteriores) con el link.
- QR en la feria hacia la web.

## Los números para saber si funciona (revisión del lunes)

| Paso | Qué medir | Referencia inicial (a validar) |
|---|---|---|
| Anuncio | Clics sobre quienes lo ven (CTR) | Más de 1% |
| Visita | Costo por visita a la ficha | Por debajo de ~$800 |
| Ficha | Quienes agregan al carrito o inician pago | Más de 5% de las visitas |
| Compra | Compras sobre visitas | 1% a 2% |

**Cuentas rápidas:** con ~$400.000 al mes y visitas de $400 a $800, llegan entre 500 y 1.000 visitas. Con 1% de conversión son de 5 a 10 ventas, entre $800.000 y $1,6 millones de margen. Es poco al principio, pero cada mes la etapa 1 deja más gente para la etapa 3, y la venta se abarata.

**Regla:** no se sube la pauta hasta que la etapa 3 traiga compras. Si la gente visita y no compra, el problema es la ficha o la oferta, no la pauta.

## Orden para dejarlo funcionando

1. Confirmar que el píxel registra eventos en el Administrador de eventos de Meta.
2. Ajustar la ficha del producto con la lista de arriba (sesión de UI/UX).
3. Grabar 3 o 4 reels de la firma (la agencia, con la nueva línea).
4. Crear las 3 campañas con los públicos de arriba.
5. Revisar los números cada lunes.

---

## Montaje de la pauta, versión 1 (prueba de 7 días, desde el 2026-10-31)

**La idea en una línea:** 1 campaña de ventas, 2 conjuntos de anuncios (gente nueva y gente que ya conoce la marca) y 5 anuncios de Delta y Limo, cada uno llevando a su ficha.

### Campaña
- **Nombre:** `MIR | Ventas | Delta-Limo | v1`
- **Objetivo:** Ventas. **Evento:** Compra, con el píxel terminado en 4398.
- **Presupuesto por conjunto**, no por campaña, para que el conjunto pequeño reciba plata.
- **Total: $60.000 al día durante 7 días (~$420.000).** Se puede llegar a $100.000 al día, pero solo después de ver los números del día 7. Primero se prueba y después se escala.

### Conjunto 1: Descubrir (gente nueva), $45.000 al día
- **Ubicación:** Colombia, ciudades principales (Medellín, Bogotá, Cali, Barranquilla, Bucaramanga, Pereira).
- **Público:** mujeres de 22 a 40, con público Advantage+ y sugerencias de intereses: joyería artesanal, joyería de plata, diseño independiente, moda de autor.
- **Excluir:** compradoras de los últimos 30 días.
- **Ubicaciones:** solo Instagram (feed, historias, reels y explorar). Ahí vive la clienta, y el material es vertical.

### Conjunto 2: Calientes (ya conocen la marca), $15.000 al día
- **Público:** quienes interactuaron con Instagram en los últimos 365 días, visitantes de la web de los últimos 30 días y la lista de clientas e inscritas (CSV `publico-meta-todos`, ~62 personas).
- **Excluir:** compradoras de los últimos 30 días.
- **Nota:** la lista tiene menos de 100 personas, así que todavía no sirve para un público similar (lookalike). Sí sirve para mostrarles anuncios.

### Los 5 anuncios (los mismos en ambos conjuntos)

| # | Formato | Pieza | Lleva a |
|---|---|---|---|
| 1 | Reel 9:16, 8–15 s, la pieza en la mano y de cerca | Delta | `/producto/delta-ring` |
| 2 | Reel 9:16, 8–15 s | Limo | `/producto/limo-ring` |
| 3 | Foto 4:5 en la mano | Delta | `/producto/delta-ring` |
| 4 | Foto 4:5 en la mano | Limo | `/producto/limo-ring` |
| 5 | Carrusel: Delta, Limo y 2 anillos más | Anillos | `/colecciones?categoria=anillos` |

En el conjunto 2 se puede sumar un sexto anuncio: foto de una clienta con su frase (*"me encanta ponérmelo, no me lo quito"*).

**Texto base (se ajusta por pieza):**
> Delta. Plata derretida, hecha a tu talla. $[precio].
> Una pieza que habla por ti, imposible de confundir.
> 🎁 Pide antes del [fecha límite] y te llega antes del 24.

**Título:** "Hecha a tu talla". **Botón:** "Comprar".

**UTM de cada anuncio:** `?utm_source=meta&utm_medium=paid&utm_campaign=ventas-v1&utm_content=delta-reel` (cambiando `utm_content` por anuncio).

### Navidad, sin complicarse
No es otra campaña. Es **una línea en el texto** del anuncio, porque la campaña corre en temporada de regalos y la web ya muestra la franja de Navidad. La fecha del anuncio y la de la web tienen que ser la misma (hoy la web dice 5 de diciembre; la recomendación era el 3).

### Reglas de los 7 días
- **Días 1 a 3: no tocar nada.** Meta está aprendiendo.
- **Día 4:** apagar los anuncios con menos de 0,7% de clics después de ~3.000 impresiones.
- **Día 7, revisión:**
  - Si hay compras a menos de ~$120.000 cada una: subir 20% cada 3 días, hasta $100.000 al día.
  - Si hay visitas y carritos pero no compras: el problema es la ficha o la oferta, no la pauta.
  - Si casi no hay clics: el problema es el material (los reels).

### Antes de encender (pendientes en la web)
- [ ] Apagar el popup del 10% para quien llega de la campaña (`utm_source=meta`).
- [ ] Decidir el envío gratis para todos durante la campaña (hoy es con 2 productos o desde $400.000).
- [ ] Unificar la fecha límite de Navidad entre web y anuncio.
